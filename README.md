
Various utilities making use of Btrfs's capabilities.

Currently contains a more complete reimplementation of `btrfs find-new`.


# Dependencies

Install CFFI:

    pip install cffi

Get btrfs-progs (we need the headers at a known location):

    git submodule update --init

# Usage

    sudo ./btrfs-find-new PATH [GENERATION]

Where PATH is a mounted btrfs volume or subvolume, and GENERATION
is the minimum generation for entries to be considered new.

