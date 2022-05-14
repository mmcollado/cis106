---

Name: Marcelo Collado
Semester: Spring 22

---

date
uname
du
free
echo
apt
pwd
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