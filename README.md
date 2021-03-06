# ncc_cli
NextCloud / ownCloud Command-Line Client

Overview
========
Just a basic command-line client for NextCloud and ownCloud based servers. This is my project with Python so if you notice any bugs or would like to provide help, please let me know!

Installation
===========
#### pip:
ncc_cli has been added to pip, so you can simply execute the following:
>    pip install ncc-cli

#### manual:
Alternatively, you can install the utility manually, but first you will need to install the following dependancies:
>humanize
>tzdm
>yaspin
>texttable
>pyocclient

Now you have all of the dependancies installed, you can simply clone the ncc_cli git repo and execute the following:
>    ./setup.py

Usage
=====
###### Syntax: ncc [command] <arguments>
ls (-l) <dir> - lists dir contents
put - [local file] <dest remote dir> - uploads file
putdir - [local dir] <dest remote dir> - uploads dir
get - [remote file] <dest local dir> - downloads file
getdir - [remote dir] <dest local dir> - downloads dir as zip
mkdir - [dir name] - creates new dir
rm - [dir/file name] - deletes files or dirs
mkshare - [dir/file name] - creates new share w/link
lsshare - [dir name] - lists shares in dir
rmshare - [dir/file name] - deletes share
cp - [source] [destination] - copies files on server
mv - [source] [destination] - moves files on server

To Do
=====
- Find a way of tracking upload progress and counting with tqdm instead of using indefinite spinner.

Libraries
=========
This utility uses the pyocclient library and a couple of other libraries for visual indications, human readable numbers, progress bars etc. Much thanks to all of the developers of their respective libraries.

> pyocclient - https://github.com/owncloud/pyocclient

> humanize - https://github.com/jmoiron/humanize

> tqdm - https://github.com/tqdm/tqdm

> yaspin - https://github.com/pavdmyt/yaspin

> texttable - https://github.com/foutaise/texttable

License
=======
This utility is licensed under the GNU GPLv3
https://www.gnu.org/licenses/gpl-3.0.en.html
