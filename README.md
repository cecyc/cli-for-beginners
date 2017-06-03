## Command Line for Beginners and Nondevelopers

[Click here for slides](https://cecyc.github.io/cli-for-beginners/)

### Notes

There are a lot of misconceptions of what the command line can do, especially when it comes to things like hacking.
  
But the portrayal in the media makes it seem like you have to be a wiz to work it, it makes it look inaccessible.
 
The command line was the biggest barrier to entry for me when I started coding. I thought I would never be able to do it and I avoided it as much as I could, often using GUIs to do the job for me, and this can be a huge blocker if you want to be a programmer. 
 
This talk is meant for 2 groups:
 
* New developers / learning to code (or maybe you’re thinking about it): hopefully this will help get you started or feel more confident
* Non-programmers: Product Manager, Marketing, Designer, Copywriter and you want to understand the command line better, maybe even use it in your day to day
 
Anyone can benefit from command line knowledge!
 
### Bit of history: What is Unix?
 
The title of this talk is “Unix command line” — why?
 
![It's a Unix system](https://raw.githubusercontent.com/cecyc/cli-for-beginners/master/images/unix.gif)
 
Unix is
 
* An operating system 
* Type of filesystem
* Set of philosophies
 
Mac OS is the largest OS using Unix as a “base”.
 
There are other “Unix-like” systems, such as Linux.
 
If I just said “Command Line”, I could be referring to the PC Command Line or Command Prompt, but the Windows Command Prompt is very different.
 
So when I say “Unix” command line, I am really referring to
 
* Unix system like Mac OS
* Unix-like system like Linux
 
### Terminal, command line, shell, what's the difference?

**Terminal:** An application that runs a shell

**Shell:** The program / interface that runs our commands
 
There are a lot of shell variants!
 
* Shell (sh) by Steve Bourne in 1977
* C shell (csh) designed to read more like the C programming language, released in 1978
* Korn shell (ksh) by David Korn, based on sh source code and incorporates features of csh, released 1983
* Bash, improvement on original Shell, released in 1989. Stands for Bourne-Again Shell, as it is an improvement on the original shell created by Steve Bourne.
 
All of these are still around!
 
Check it out:
 
`cat /etc/shells`
 
Will print out a list of shells in your system.
 
You can choose to use whichever one you want.
 
**The most common shell is Bash (1989).**
 
When you open up your terminal in Mac OS, you are opening a Terminal that’s running bash.
 
On Windows, this is different. Windows uses the Command Prompt and MS-DOS. These commands are different than bash and I won’t be covering those.
 
But — you can now get [bash on Windows](https://www.windowscentral.com/how-install-bash-shell-command-line-windows-10)! 
 
**Why bash? (opinion)**
 
* bash is more standard (can run commands on a Mac, Linux machine, and Windows if it has bash installed)
* If you ever need to run commands on a remote server somewhere, it is likely to be a Linux server, which means you would need to run bash commands (so running commands on a remote server can be the same commands as on your local machine)
 
### The basics
 
`$` is the prompt
 
When you see a `$` that means this is a command you are supposed to run on the command line, you don’t need to copy the `$`.
 
bash is (typically) case sensitive
 
#### Basic commands
 
* pwd 
* ls
* ls -a 
* mkdir 
* touch 

#### Other cool commands

* cal
* date
* ctrl + z
* fg / bg
* ctrl + c
* top
* kill 
 
Cool! Those are some practical things we can do. Let’s level up.
 
### Homebrew
 
Homebrew is a program that helps you install things, like languages and applications. It manages dependencies in some cases and also takes care of downloading updates.
 
If you’re a developer, you will likely use Homebrew a lot for installing languages, etc.
 
If you’re not a developer, you can use Homebrew to easily install applications using “cask”
 
`brew cask install google-chrome`
 
[Search applications available here](https://caskroom.github.io/search).
 
Using Homebrew, we can easily create a script that installs all the software we need in a new computer.
 
`new_computer.sh`
 
``` 
#install homebrew
 
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
 
#install apps
 
brew cask install google-chrome
 
brew cask install spotify
 
brew cask install evernote
 
brew cask install slack
```
 
### zsh and Oh My Zsh!
 
Remember when we talked about all the different shells?
 
zsh or z shell is a popular alternative to bash
 
Why?
 
* Autocompletion 
* Spelling correction
* Not case sensitive
* Themeable
 
[Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh): framework for zsh
 
* Lots of themes!
* Lots of plugins!
 
### fish and Oh My Fish
 
[fish](https://fishshell.com/) is another alternative to bash.
 
Stands for Friendly Interactive Shell
 
Newer (released 2005)
 
Syntax is a somewhat different than bash (I don’t find it too different)
 
* Autocompletion
* Suggestions
* Syntax highlighting
 
[Oh My Fish](https://github.com/oh-my-fish/oh-my-fish): Similar to Oh My Zsh
 
* Easily install themes and plugins
