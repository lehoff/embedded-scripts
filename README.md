embedded-scripts
================

A collection of small scripts that should make working with embedded
devices easier.

Developed on a Mac, but should be useful on other platforms as long as
you have a bash shell.

It is assumed that you are working with a git repo that you would like
to copy to an embedded device.

The scripts are very specific to working with Erlang on a
Raspberry-Pi, but the commands should be so general that it is easy to
tweak them to work in other settings.

Basically the scripts are wrappers for rsync which you need to have in
order to use the scripts.

Install
---------------------------------

Inside the directory of this repo just issue a
./install <dest-dir>

This will copy the files over and add them to the .gitignore file in
tha directory.

Functionality
---------------------------------
`dump_to_pi`: Will copy everything from your Erlang repo including the
deps directory.

`sync_to_pi`: More incremental copy. Just the changes in your code will
me transferred.


`dump_excludes` and `sync_excludes` determines which files _not_ to
copy over to the target device.

