### Head (Attached & Detached)

`HEAD` is a pointer to the currently “checked out” branch or commit (refer to the “What is git?” for more details on a branch or commit). It essentially tells you where you are in the repository. 

The default state is *attached* , where any manipulation to the history is automatically recorded to the branch `HEAD` is referencing. 

In *detached* state, experimental changes can be made without impacting any existing branch. This means `HEAD` does not point to a branch, but instead points to a specific commit or the remote repository. 

---

References: 

https://stackoverflow.com/questions/3965676/why-did-my-git-repo-enter-a-detached-head-state

https://circleci.com/blog/git-detached-head-state/