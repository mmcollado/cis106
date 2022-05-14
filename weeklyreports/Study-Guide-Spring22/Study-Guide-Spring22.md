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

cd
ls
tree
man
mkdir
touch
rm
cp
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