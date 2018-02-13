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
alias search='ls -la | grep $@'
```

Most of the alias I use are to make things more easy and fast when using terminal
