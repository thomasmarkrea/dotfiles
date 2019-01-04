# dotfiles

Setup and configure system.

## sections

These dotfiles are split into software based sections.

Each section contains an `install` file that handles the install and config of that software. These can be run individually or the top level `install` file can be run to install all sections.

## components

-   **install**: Shell scripts containing code to install and configure each section. The top level `install` file will find and run all others.
-   **.symlink**: Any file ending `.symlink` will be symlinked to `$HOME` (unless another destination is specified in the `install` file).
-   **.rep**: Any file ending `.rep` should contain code to add a new software repository.
-   **.list**: No code, just lists of files/packages to be downloaded/installed.
-   **resources/functions**: Helper functions used in the `install` files.

## install

```bash
git clone https://github.com/thomasmarkrea/dotfiles.git
bash dotfiles/install
```

## manual steps

-   Chrome
    -   set up Extensions (Authy, LastPass, etc.)
-   insync
    -   set folder, add accounts, start sync
-   rStudio ([no config file]( https://github.com/rstudio/rstudio/issues/1607))
    -   configure (save workspace, .RData, Pane Layout)

## thanks

[Zach Holman](https://github.com/holman/dotfiles) for ideas and some code.
