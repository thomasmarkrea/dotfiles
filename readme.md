# dotfiles

Setup and configure system.

## sections

These dotfiles are split into software based sections.

Each section contains an `install` file that handles the install and config of that software. These can be run individually or the top level `install` file can be run to install all sections.

## components

-   **install**: Most important component. Each section has an `install` file that when run will install and configure the section. The top level `install` file will find and run all other `install` files.
-   **.rep**: Any file ending `.rep` should contain code to add a new software repository
-   **.symlink**: Any file ending `.symlink` will be symlinked to `$HOME` (unless another destination is specified in the `install` file)
-   **.list**: No code, just lists of files/packages to be downloaded/installed
-   **functions**: Helper functions used in the `install` files

## install

```bash
git pull https://github.com/thomasmarkrea/dotfiles.git
bash dotfiles/install
```

## thanks

[Zach Holman](https://github.com/holman/dotfiles)
