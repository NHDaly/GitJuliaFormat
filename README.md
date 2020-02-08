# git-julia-format

## Installation

Add the executable script `git-julia-format` to somewhere visible in your `PATH`:
 - either by adding this directory to your `PATH`, or
 - linking the executable script into a directory in your `PATH`:
 
    ```bash
    $ ln -s ~/.julia/dev/GitJuliaFormat/git-julia-format /usr/local/bin/git-julia-format
    ```
   
## Usage

From within a `git` repository, run `git julia-format`, and it will modify your files in-place, running [`DocumentFormat.format()`](https://github.com/julia-vscode/DocumentFormat.jl) on the modified lines.

## Warning

1. This will directly modify the files in your working tree. Be sure to stash your changes before running this command!
1. This repo is a very early work-in-progress, and very well might not work at all. :)

## Acknowledgments and references

The `git-julia-format` script is heavily inspired by ClangFormat's [`git-clang-format`](https://llvm.org/svn/llvm-project/cfe/trunk/tools/clang-format/git-clang-format) tool. That tool is distributed under the University of Illinois Open Source License. See their `LICENSE.TXT` for details: [`LICENSE.TXT`](https://llvm.org/svn/llvm-project/cfe/trunk/LICENSE.TXT).

The structure of this repo is inspired by https://github.com/audiohacked/git-clang-format.
