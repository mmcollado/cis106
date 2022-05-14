---

Name: Marcelo Collado
Semester: Spring 22

---

* date
* uname
* du
* free
* echo
* apt
* pwd
* cd
* ls
* tree
* man
* mkdir
* touch
* rm
* cp
mv
stat
Wildcards (*,?,[])
Brace expansion
cat
head
tail
cut
tr
paste
wc
grep
output redirection
Saving the output of a command
vim or nano (basic stuff: open a file, close a file, edit a file)
tar
gz, bzip2, or xz
chmod


# Command name
```date```
## Description
 Display  date  and  time  in  the given FORMAT.  With -s, or with [MMD‐
       Dhhmm[[CC]YY][.ss]], set the date and time.

## Syntax
`date OPTION + FORMAT`
## Example
* Description of example:
  * `date --date='TZ="America/Los_Angeles" 09:00 next Fri`
* Description of example:
  * `TZ='America/Los_Angeles' date`
* Description of example:
  * `date --date='@2147483647'`

# Command name
```uname```
## Description
  Print certain system information.  With no OPTION, same as -s.
## Syntax
`uname [OPTION]...`
## Example
* Description of example:
  * `uname -a`
* Description of example:
  * `uname -r`
* Description of example:
  * `uname -m`

# Command name
```du```
## Description
* Summarize  device  usage  of the set of FILEs, recursively for directo‐
       ries.

## Syntax
`du [OPTION]... [FILE]...`
## Example
* Description of example:
  * `du -h /home/cis106/Downloads`
* Description of example:
  * `du -a -h /home/cis106/Downloads`
* Description of example:
  * `du -c -h /home/cis106/Downloads`


# Command name
```free```
## Description
* free  displays the total amount of free and used physical and swap mem‐
       ory in the system, as well as the buffers and caches used by  the  ker‐
       nel.  The  information  is  gathered by parsing /proc/meminfo. The dis‐
       played columns

## Syntax
`free [options]`
## Example
* Description of example:
  * `free -h`
* Description of example:
  * `free -b`
* Description of example:
  * `free --mega`

# Command name
```echo```
## Description
*  display a line of text


## Syntax
`echo [SHORT-OPTION]... [STRING]...`
## Example
* Description of example:
  * `echo -e 'Hello, GPU! \c This is PNAP!'`
* Description of example:
  * `echo -e 'Hello, \tGPU!'`
* Description of example:
  * `echo -e 'Hello, \vGPU, \vthis \vis \vPNAP!'`

# Command name
```apt```
## Description
* apt is a command-line utility for installing, updating, removing, and otherwise managing deb packages on Ubuntu, Debian, and related Linux distributions. It combines the most frequently used commands from the apt-get and apt-cache tools with different default values of some options.


## Syntax
`apt [-h] [-o=config_string] [-c=config_file] [-t=target_release]
    [-a=architecture] {list | search | show | update |
    install pkg [{=pkg_version_number | /target_release}]... |
    remove pkg... | upgrade | full-upgrade | edit-sources | 
    {-v | --version} | {-h | --help}}`
## Example
* Description of example:
  * `sudo apt full-upgrade`
* Description of example:
  * `apt list --upgradable`
* Description of example:
  * `sudo apt install nginx`


# Command name
```pwd```
## Description
* Print the full filename of the current working directory.


## Syntax
` pwd [OPTION]...`
## Example
* Description of example:
  * `pwd -P`
* Description of example:
  * `pwd -L`
* Description of example:
  * `pwd`

# Command name
```cd```
## Description
* change the working directory

## Syntax
` cd [-L|-P] [directory]`
## Example
* Description of example:
  * `cd ..`
* Description of example:
  * `cd /Downloads`
* Description of example:
  * `cd /Downloads/cis106`

# Command name
```ls```
## Description
* list directory contents

## Syntax
`ls [OPTION]... [FILE]...`
## Example
* Description of example:
  * `ls -l`
* Description of example:
  * `ls -ah /repollo`
* Description of example:
  * `ls -F /Documents`


# Command name
```tree```
## Description
* list contents of directories in a tree-like format.

## Syntax
` tree  [-acdfghilnpqrstuvxACDFJQNSUX]  [-L level [-R]] [-H baseHREF] [-T
       title]  [-o  filename]  [-P   pattern]   [-I   pattern]   [--gitignore]
       [--matchdirs]   [--metafirst]  [--ignore-case]  [--nolinks]  [--inodes]
       [--device] [--sort[=]name] [--dirsfirst] [--filesfirst] [--filelimit #]
       [--si]  [--du]  [--prune]  [--timefmt[=]format]  [--fromfile]  [--info]
       [--noreport] [--version] [--help] [--] [directory ...]`
## Example
* Description of example:
  * `tree -df`
* Description of example:
  * `tree -f -L 2`
* Description of example:
  * ` tree -f -P cata*`


# Command name
```man```
## Description
*  man  is  the system's manual pager.  Each page argument given to man is
       normally the name of a program, utility or function.  The  manual  page
       associated with each of these arguments is then found and displayed.  A
       section, if provided, will direct man to look only in that  section  of
       the  manual.   The  default action is to search in all of the available
       sections following a pre-defined order (see DEFAULTS), and to show only
       the first page found, even if page exists in several sections.

## Syntax
`man [OPTION]... [COMMAND NAME]...`
## Example
* Description of example:
  * `man printf`
* Description of example:
  * `man -f ls`
* Description of example:
  * `man -k cd`


# Command name
```mkdir```
## Description
*  make directories

## Syntax
`mkdir [OPTION]... DIRECTORY...`
## Example
* Description of example:
  * `mkdir Linux`
* Description of example:
  * `mkdir {test1,test2,test3}`
* Description of example:
  * `mkdir -P {one,two,three}/deva{andalai,maniu,manuki}`


# Command name
```touch```
## Description
*  The touch command is a standard program for Unix/Linux operating systems, that is used to create, change and modify timestamps of a file. Before heading up for touch command examples, please check out the following options.
## Syntax
`touch <options> <file or directory name>`
## Example
* Description of example:
  * `touch bismuto1 bismuto2 bismuto3`
* Description of example:
  * `touch -m bismuto3`
* Description of example:
  * `touch -c bismuto4`

# Command name
```rm```
## Description
*  rm command is used to remove objects such as files, directories, symbolic links and so on from the file system like UNIX.
## Syntax
`rm [OPTION]... [FILE]...`
## Example
* Description of example:
  * `rm -i d.txt`
* Description of example:
  * `rm -f e.txt`
* Description of example:
  * ` rm -r *`


# Command name
```cp```
## Description
*  Copy SOURCE to destination, or multiple SOURCE(s) to DIRECTORY.

## Syntax
` cp [OPTION]... SOURCE... DIRECTORY`
## Example
* Description of example:
  * `cp -i a.txt b.txt`
* Description of example:
  * `cp -b alimony.txt juvenile.txt`
* Description of example:
  * `cp -f repulsion.txt lamusa.txt`


# Command name
```mv```
## Description
*  Copy SOURCE to destination, or multiple SOURCE(s) to DIRECTORY.

## Syntax
` `
## Example
* Description of example:
  * `cp -i a.txt b.txt`
* Description of example:
  * `cp -b alimony.txt juvenile.txt`
* Description of example:
  * `cp -f repulsion.txt lamusa.txt`



