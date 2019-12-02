# dotfiles

Setup and configure system.

## sections

These dotfiles are split into software based sections.

Each section contains an `install` file that handles the install and config of that software. These can be run individually or the top level `install` file can be run to install all sections.

## components

### files

-   **install**: default instalation script, symlinks dot files and installs packages
-   **pre/post**: pre and post install scipts for anythig that needs to be run before or after the defult script
-   **. files**: Any file beggining with a `.` will be symlinked to `$HOME`
    **.rep**: script to add new external software repository
-   **package.list**: list of packages to be installed
-   **download.list**: list of packages (.deb files) to download and install

## install

```bash
git clone https://github.com/thomasmarkrea/dotfiles.git
bash dotfiles/install
```

## manual steps

-   Barve
    -   update settings
    -   set up Extensions (Authy, LastPass, Trello, Keep)
-   insync
    -   set folder, add accounts, start sync
-   RStudio ([no config file](https://github.com/rstudio/rstudio/issues/1607))
    -   configure (save workspace, .RData, Pane Layout)

## thanks

[Zach Holman](https://github.com/holman/dotfiles) for ideas and some code.
