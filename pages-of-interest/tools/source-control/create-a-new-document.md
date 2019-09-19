# Create a new document

To create a new document, simply take one of the other document repositories, such as converge-app/research and clone it

```bash
git clone https://github.com/converge-app/research # pulling the repository
cd research # enter folder
git submodule init # get any submodules if any
git submodule update # getting the contents of the submodules from remote
```

Now it's time to create a new repo, do this from github.com, lets cal it converge-app/new-docs

```bash
cd .. # Go back to root 
mv research new-docs # rename research folder to new-docs
cd new-docs # go into new folder
git remote rename origin old # rename the remote to make room for a new remote
git remote add origin https://github.com/converge-app/new-docs # add a new origin
git push -u origin master # reset origin to point to new repository
```

Now you should have an updated repository that is technically a clone of the old one. Now feel free to rename files that need renaming.

