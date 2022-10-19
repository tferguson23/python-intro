# Running List of Reference Material

Below is a running list of tools and reference material associated with those tools. Resist the [Toolbox Fallacy](https://www.process.st/toolbox-fallacy/#:~:text=The%20toolbox%20fallacy%20is%20self,start%20a%20project%20without%20them.). These are merely tools. You'll get a feel for when you need them and when you don't. Remember, sometimes, it is the archer and not the arrow.

### Markdown basics
[Markdown](https://www.markdownguide.org/basic-syntax/) is a powerful markup (hence the name) language. I find it to be very expressive, and most code documentation you see will be written in Markdown. There are ways to augment it and make it _extremely_ powerful, but we only need the basics right now.

### ssh tutorial
[This](https://www.digitalocean.com/community/tutorials/ssh-essentials-working-with-ssh-servers-clients-and-keys) is a big article, but you don't need to get too far into the weeds with it. The first few sections should more than cover what we did. DigitalOcean is a web _platform_ that you can host things on. We'll likely use them when we deploy something later.


### git basics
[This](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/) should be everything you need to know for now. Git is a deep well. It is extremely powerful; however, you won't need these advanced techniques outside or large scale engineering projects. 

### vim
`vim` is an insanely powerful editor built into your command line. Everything you do in vscode can be done in vim. Using vim as your primary code editor is for god-tier developers or Wizards. Few things are as inspiring as seeing someone who knows how to use vim use vim. They code so fast, and they _live_ in that flow state I was describing. This is a [super fun browser game](https://vim-adventures.com/) designed to help you learn it. 

You will only need a couple things from vim. Not because you'll be using it to _code_ but because sometimes `git` will launch vim automatically. For now, there are only two things to be aware of:
1. Command mode. This is the default mode. Activate this mode by pressing escape.
2. Insert mode. Activate this mode by pressing `i`. Go back to command mode by pressing escape again.

When in command mode, _anything you type will be interpreted as a command_. This is likely _not_ what you want. But, the way to _quit_ vim is a command. So, for now, when you get into vim (you'll know because your terminal will look very different and your curson will be positioned at the top instead of the bottom) just try to quit out of is as soon as you can. This early on you probably opened vim by accident anyway. 

To quit:
1. activate command mode by pressing escape
2. `:q` quit - this will fail if you have made changes
3. `:q!` force quit - should discard your changes
4. `:wq` write quit - use when you want to save what you did then quit (you need this for git sometimes but not yet)
5. If all else fails, close your terminal window entirely and open a new one.