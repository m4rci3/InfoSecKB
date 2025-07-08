A Dockerfile is a text file containing instructions for building [Docker Images](https://github.com/m4rci3/InfoSecKB/blob/main/Docker/Docker%20Images.md) specifying the commands to run, files to copy, and other configuration details needed to create a containerized application

When creating a docker file name it `Dockerfile` 

The **FROM**
 instruction specifies the base image that the container will be built on top of. This instruction is typically the first one in a Dockerfile and is used to set the base image for the container. The format of the instruction is:

```docker
FROM <image>
```

#Optionally you can add the **MAINTAINER** line which is just metadata for crediting the author of the docker image 

```docker
MAINTAINER <email>
```

**WORKDIR**

In a Dockerfile, the **WORKDIR**
instruction sets the working directory for any command that follows it in the Dockerfile. This means that any commands that are run in the container will be executed relative to the specified directory. Below is the format of the instruction :

```docker
WORKDIR <directory>
```

Any subsequent commands in the Dockerfile, such as **`COPY`, `RUN`, or `CMD`,** will be executed in this directory.

**COPY**

In a Dockerfile, it will copy a file from the contectinto the container at location specified , otherwise will copy into the WORKDIR 

```docker
COPY <path> <dst>
```

**RUN**

Use the “**RUN”** instruction to execute commands that will run during the image build process, can be run multiple times. The format of instruction is :

```docker
RUN <command_name>
```

**CMD**
Lets you define the default program that is run once you start the container 

```docker
CMD ["<command>", "<arg1>"]
```

**EXPOSE**:

Use the **EXPOSE**  command to tell Docker which ports the container will listen on at 
runtime. For example, if your application listens on port 9000, you would use the following command:

```docker
EXPOSE 9000
```

This instruction isn't required, but it is a good practice and helps tools and team members understand what this application is doing.

References: 

https://docs.docker.com/get-started/docker-concepts/building-images/writing-a-dockerfile/

https://docs.docker.com/build/concepts/dockerfile/
