---
Name: Marcelo Collado 
class: cis106
semester: spring 2022
---

# week5 report 

#        A table of the commands in the Homework5 including what the command does and some examples

|Command |	Definition |uses| Examples|
|--------|-----------|---------|------------|
|mkdir |is a command that makes directories |make directories |mkdir -p directory/path/newdir  ``` mkdir -p home/cis106/beans```|
|touch| A FILE argument that does not exist is created empty, unless -c  or  -h is supplied.|change file timestamps| touch file1 file2 file3 |
|rm| rm is a command-line utility for removing files and directories|remove files or directories | rm -i d.txt  ```rm -i howards.txt```|
|rmdir|Remove the DIRECTORies, if they are empty.|remove empty directories | rmdir [-p] [-v –verbose [–ignore-fail-on-non-empty] ``` rmdir -p home/island ```||
|mv|  Rename SOURCE to DEST, or move SOURCEs to DIRECTORY.| move (rename) files| mv [options] source dest ```mv -f ~/home/games ~home/games/steam/destiny2```||
|cp| Copy SOURCE to DEST, or multiple SOURCEs to DIRECTORY. |copy files and directories| cp [OPTION] Source Destination ```cp a.txt b.txt new```||
|ln| In  the  1st form, create a link to TARGET with the name LINK_NAME.  In the 2nd form, create a link to TARGET in the current directory.  In the 3rd  and  4th  forms, create links to each TARGET in DIRECTORY.  Create hard links by default, symbolic links  with  --symbolic.   By  default, each  destination  (name  of  new link) should not already exist.  When creating hard links, each TARGET must exist.  Symbolic links  can  hold arbitrary  text;  if  later resolved, a relative link is interpreted in relation to its parent directory.|make links between files| ln [OPTION]... TARGET ```ln file1.txt file2.txt```||
|man| man  is  the system's manual pager.  Each page argument given to man is normally the name of a program, utility or function.  The  manual  page associated with each of these arguments is then found and displayed.  A section, if provided, will direct man to look only in that  section  of the  manual.The default action is to search in all of the available sections following a pre-defined order (see DEFAULTS), and to show only the first page found, even if page exists in several sections.| an interface to the system reference manuals| man [man options] [[section] page ...] ```man -a intro``` ||
##
###
>>>
