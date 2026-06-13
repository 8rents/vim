# Setting Vim up from Scratch

> *Building my set up*

---

## Make a configuration folder

Vim automatically looks in `.config/vim`. I renamed `.config` to `dotfiles`. 

1. I copy a project templat
   ```
   cp -r templates/project dotfiles/vim
   ```
2. cd into vim folder and make a vimrc
   ```
   cd dotfiles/vim
   touch vimrc
   vim README.md TODO.md CHANGELOG.md docs/configuration.md docs/commands.md vimrc
   ```

   Edit CHANGELOG and add a comment to the top of `vimrc`

3. Initialize git repo and edit changelog
   ```
   git init
   git add -A
   git commit
   git remote add origin https://github.com/8rents/vim  

   ```

