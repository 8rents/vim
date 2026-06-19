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
   touch vimrc; mv vimrc init.lua
   vim README.md TODO.md CHANGELOG.md docs/configuration.md docs/commands.md init.vim
   ```

   Edit CHANGELOG and add a comment to the top of `vimrc` errr `init.lua`. I'm
   going to go with lua for my vimrc because it's an actual modern programming language and not vim script.

3. Initialize git repo and edit changelog
   ```
   vim CHAMGELOG.md init.lua
   git init
   git add -A
   git commit
   git remote add origin https://github.com/8rents/vim  
   git push origin android
   ```
 4. Google Essential Vim Configuration and edit `init.lua`
   ```
    
    ```
