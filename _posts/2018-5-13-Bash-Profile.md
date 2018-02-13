Some basic stuff that I like to change to terminal so it's easier to work with it

### Find your bash profile!

Usually the bash profile is located under the home directory

```bash
cd ~/
```

List all the files

```bash
ls -la
```
The one named .bash_profile or .profile is the one we are looking for, so let's list a couple of aliases that I like to add:

```bash
alias ll='ls -lGh $@'
alias las='ls -la $@'
alias sshmachine1='ssh YOURUSER@machine1'
alias sshmachine2='ssh machine2'
alias cd..='cd ..'
alias srch='ls -la | grep $@'
```

Most of the alias I use are to make things more easy and fast when using terminal. alias is the way a "new command" can be delcared. In this case these are the new aliases we are creating:

1 "ll" this is ueful when listing all the files in the working directoy
2 "las" I'ts a simple "ls -la" but with less characters
3 "sshmachineX" this is really useful when a lot of SSH connecitons are needed
4 "cd.." Well it's just in case there's a typo!
5 "srch" It's really useful when trying to find files in a directory
