zerohosts
=========

Simple script that fetches and updates your hosts file with zerohost data.
It fetches the hosts file from http://someonewhocares.org/hosts/zero/

The fetched hosts file is not modified or easily modifyable in any way as of now.
If you modify the result it will be overwritten on update.

The script inserts a BEGIN marker and an END marker. This way updates (re-running the script) will not append the remote file twice - if old data is found it will be removed (using the markers) before the new data is appended.

The script will ask for sudo privileges in order to perform the modifications of _/etc/hosts_.
_/etc/hosts_ will be backed up to _/tmp/_ in case of total disaster and other problems.

This script is distributed under the beerware license. Yay! :koala:
