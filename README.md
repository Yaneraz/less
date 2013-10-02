LESS boilerplate
================

Creating awesome LESS CSS boilerplate.

#### How to start?

Simply:

    git clone https://github.com/Yaneraz/less.git <project name>

To remove unnecessary  .git folder type

    rm -rf <project name>/.git

or

    rm -rf !$/.git

`!$` is for previous argument right after git clone has been completed.

File structure
--------------

TODO: add file structure description

Watchers/Compilers
------------------

### Using Webstorm (or other JetBrains IDE) - *recommended*
-----------------------------------------------------

See Webstorm file watcher settings.
![alt tag][1]

##### Scope
Scope should contain all less files we want to work with. For most projects should be enough
to include all files in /less folder (better with file extension)

##### Program
Path to less executable file

##### Arguments
File(s) or directory that will be passed to the transpiler. For now we should specify only style.less.

Later files with "_" in the beginning will be imported to main (style.less),
others will create css file with theirs filename.

##### Working directory
Specify the directory to which the transpiler will be applied. If not specified - working directory is the directory of the current file.

##### Output path to refresh
Specify the files where the transpiler stores its output. For now we should specify only style.css.\

### Using Koala (Cross platform)
--------------------------

[Download][2] Koala application, add project directory to program, choose only style.less file to autocompile, others will be watched automatically. Enjoy!

Feature: doesn't display less files that starts with "_" but watches them correctly.

### Using WinLESS (Windows only)
--------------------------

[Download][3] WinLESS, add project directory to program, check only style.less file to compile, others will be watched automatically. Enjoy!


[0]: https://www.dropbox.com/s/nnd0852697faae3/webstorm-file-watcher.png
[1]: https://photos-4.dropbox.com/t/0/AADgwYGO8a5bBcA6uDJ5InuZIqQDtlgJaMNktGAwODjEpA/12/40486094/png/1024x768/3/1380715200/0/2/webstorm-file-watcher.png/1BYUDbrikIqrnNKlhVesisGP3nEGBSJ_8xWil0H0-6k
[2]: http://koala-app.com/
[3]: http://winless.org/
