# Warning

This code is **unmaintained and left behind**. This is a _backup_ of the original
source as it was removed from Debian in 2017.

There may be commits. Who knows?

# Original ReadMe

## Audio Tag Tool


### DESCRIPTION

  Audio Tag Tool is a program to manage the information fields in MP3 and 
Ogg Vorbis files (commonly called 'tags').  It is available under the GNU 
General Public Licence (GPL).  Please send me any comments or bugs you 
find.

  Tag Tool can be used to edit tags one by one, but the most useful 
features are the ability to easily tag or rename hundreds of files at 
once, in any desired format.

  The interface is arranged into two sections, with the list of available 
files on the left and a set of tabs on the right. Each tab corresponds to 
one of the main operations Audio Tag Tool can do:

  - Tag Editor
    Lets you edit the tags individually. 
  - Tag Multiple Files
    Here you can set the tags of multiple files at once. The tag fields can be set 
    to a fixed value, filled in automatically from the file's name, or left alone.
  - Clear Tags
    Allows you to remove the tags from multiple files at once. For MP3 files it 
    lets you choose to remove only ID3v1 or ID3v2 tags.
  - Move/Rename Multiple Files
    Here you can rename multiple files at once and/or organize them into directories. 
    File names can be based on the contents of the tag. 
  - Create Playlists
    Generates playlists. Playlists can be sorted by file name or by any tag field.

  The mass tag and mass rename features can handle filenames in any 
format thanks to an easily configurable format template. 


### RELEASE NOTES

  Read the file NEWS for information about the current release.


### LIMITATIONS

  For MP3 files:

  - Images and other non-text fields in ID3v2 tags cannot be edited.

  For Ogg Vorbis files:

  - Multiple logical streams are tolerated, but only the tags of the 
    first stream can be edited.  This is not likely to change.
  - Multiple comments with the same name are concatenated with a comma 
    as separator and cannot be edited (or saved back) separately.
    This is not likely to change either, unless someone can suggest a 
    simple and sane user interface for it.

  See also the BUGS file for a list of currently know problems.


### FILESYSTEM ENCODINGS

  The filesystem encoding is assumed to be UTF-8.  As with other Gtk2 
apps, if your filesystem is not in UTF-8 you will need to set the 
G_FILENAME_ENCODING environment variable.  From the Gtk documentation:

  "G_FILENAME_ENCODING may be set to a comma-separated list of 
   character set names. The special token "@locale" is taken to 
   mean the character set for the current locale. The first 
   character set from the list is taken as the filename encoding."


### INSTALLATION

  At the console type

    ./configure
    make
    make install

  For more information refer to the file INSTALL.

  Audio Tag Tool is tested on Linux, and is reported to run without 
trouble on NetBSD and OpenBSD.  If you succeed in compiling on other 
platforms please let me know.  If you don't succeed let me know too, 
and I'll try to fix it...


### LICENSE

  This program is free software; you can redistribute it and/or 
modify it under the terms of the GNU General Public License, 
version 2, as published by the Free Software Foundation.

  This program is distributed in the hope that it will be useful, 
but WITHOUT ANY WARRANTY; without even the implied warranty of 
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
General Public License for more details (it should be included 
in this package in the file COPYING.)


### CONTACTS

* Author:   Pedro �vila Lopes (paol1976<#>yahoo.com)
* Homepage: http://pwp.netcabo.pt/paol/tagtool/

