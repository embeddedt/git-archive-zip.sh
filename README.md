# git-archive-zip.sh
A bash shell script wrapper for git-archive that archives a git superproject and its submodules, if it has any.

The two scripts in my repository should be placed in the same folder, then you should run `./git-archive-zip.sh`, not `./git-archive-all.sh` to create a flattened ZIP file containing the repository plus it's submodules.

This is an extension of the original script which could not create a flat ZIP file. It works by making a TAR archive, then extracting it and putting the output into a ZIP.

Fancy filesystem features like symbolic links, etc. may not work properly. Use at your own risk!

`git-archive-all.sh` is distributed under it's original GPL3+ license, see https://github.com/meitar/git-archive-all.sh for details.

`git-archive-zip.sh` is distributed under the MIT license.
