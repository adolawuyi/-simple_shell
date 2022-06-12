stat (__xstat) (man 2 stat)

lstat (lxstat) (man 2 lstat)

fstat (fxstat) (man 2 fstat)

strtok (man 3 strtok)

wait (man 2 wait)


waitpid (man 2 waitpid)

wait3 (man 2 wait3)

wait4 (man 2 wait4)

write (man 2 write)


### Testing

Your shell should work like this in interactive mode:

$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
But also in non-interactive mode:

$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$

### Checks

The Checker will be released at the end of the project (1-2 days before the deadline). We strongly encourage the entire class to work together to create a suite of checks covering both regulartests and edge cases for each task. See task 8. Test suite.

