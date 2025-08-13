### Head (Attached & Detached)

`HEAD` is a pointer to the currently “checked out” . It essentially tells you where you are in the repository.

The default state is _attached_ , where any manipulation to the history is automatically recorded to the branch `HEAD` is referencing.

In _detached_ state, experimental changes can be made without impacting any existing [[Branch]] . This means `HEAD` does not point to a branch but instead points to a specific [[Commit]] or the remote repository.

---

References:

[https://stackoverflow.com/questions/3965676/why-did-my-git-repo-enter-a-detached-head-state](https://stackoverflow.com/questions/3965676/why-did-my-git-repo-enter-a-detached-head-state)

[https://circleci.com/blog/git-detached-head-state/](https://circleci.com/blog/git-detached-head-state/)
