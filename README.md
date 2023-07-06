# Unraid-Additional-Scripts
Just some helpful scripts.

#### `cpref`
Uses `--reflink` when copying files even when in `/mnt/user`. It figures out what disk a current file is located on and copies to the same disk. Using `--reflink` doesn't work by default because of the way Unraid sets up the shares to all merge together in the `/mnt/user` directory.
**Note: You must be using a file system that supports copy-on-write, otherwise it just copys as normal.**

#### `diskof`
Prints the full path of a file and shows which disk the file is located on. This is useful when browsing files under `/mnt/user`.