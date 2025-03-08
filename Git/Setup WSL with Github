# Do this if you want to push any commits to your own repos from the command line, or if you like to maintain other peoples repositories locally :

  

```bash

ssh-keygen -t {encryption, e.g. rsa} -b {bits, e.g.4096} -C {comment, email of git acc}

```

  

##### Add a passphrase that is easy to remember (but not overly simple) , store this in your favorite

  

##### This will generate a keypair , one for you to keep (private key) and the other for you to post to your GitHub account (public key)

  

##### I would recommend storing these keys inside of a password manager like Bitwarden,

  

##### Your public and private key will be stored in the file that is shown in the output , after entering the above comment:

  

`‘/home/username/.ssh’`

  

- Here you will have your public and private key

  

##### Go to GitHub account: *Settings* → *SSH and GPG Keys* → *New SSH key*

  

##### Title = WSL

  

##### Key type = *Authentication Key*

  

##### Key = *paste your public key here*

  

##### Enter your GitHub password if prompted

  

##### The key has been added

  

##### Now you can go back to your WSL terminal and enter :

  

```bash

ssh -T git@github.com

```

  

##### you will be prompted for the passphrase of your keypair

  

##### Now this will permanently add [github.com](http://github.com)  to the list of known_hosts , this can be found inside of this file directory:

  

##### `“/home/username/.ssh/known_hosts”` , there will also be a `known_hosts.old` file created, you can delete this if you want. This is also the place where you would confirm if the “host” you added was in fact the entity you want to add, this has the entities public key for you to use to confirm it is really them.

  

##### Configure Git with your identity

  

```bash

git config --global user.name "username"

git config --global user.mail "emailaddress@gmail.com"

# Neither of these should be in parentheses , this is purely for demonstration

```

  

##### Create a folder for projects on user’s home directory

  

- This folder will contain all your projects , name it `git` , `projects` , `code`  or whatever

  

```bash

mkdir ~/git

```

  

##### You can move into this directory , from this point, you can now clone your and other's repositories into your newly created folder, obviously if you named it differently replace it in this next command, what follows the `clone` keyword you will find in the <>code button then SSH dropdown on the repository you want to copy :

  
  

```bash

git clone git@github.com:m4rci3/somethingsomethingrepository

# not what you would paste in exactly , purely for demonstration purposes

```

  

##### You will need to enter the passphrase for your SSH keypair

  

##### When you go into the newly cloned git repo , you can see all the files and folder inside of that repo , if you want to

  

##### Make sure to run the following to ensure your “local branch” is up to date