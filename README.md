# git manifest

This a little command line tool that helps port directories of Git repositories between machines.

## Installation

Clone the repository and (optionally) make `gitmanifest` available to your `$PATH`.

## Export

To create an export file, run `gitmanifest` from the directory you want to "copy".  It will recurse through all of the child git directories and create a file called `gitmanifest.json`.  Any repositories that don't have remotes will be skipped.

## Import

Run `gitmanifest /path/to/gitmanifest.json` and it will recreate the directory structure of your repositories.  Any repositories that conflict with pre-existing directories will be skipped.
