# Installing Ruby on WSL2

## Install Ruby Environment Manager (RVM) on Ubuntu

Ruby Environment Manager (RVM) is a tool that will allow you to download and
install multiple versions of Ruby, one of the programming languages that we
teach at Flatiron School. Installing RVM is the first step in installing Ruby on
your Ubuntu operating system.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. Type `sudo apt-get install software-properties-common` and press `<Enter>`
3. You may be asked to enter your Ubuntu terminal password
4. Type `sudo -E apt-add-repository -y ppa:rael-gc/rvm` and press `<Enter>`
5. Type `sudo apt-get update` and press `<Enter>`
6. Type `sudo apt-get install rvm` and press `<Enter>` _(Note: if you are asked
   "Do you want to continue [Y/n]", type "Y" and press `<Enter>`)_
7. Type `source /etc/profile.d/rvm.sh` and press `<Enter>`
8. Type `echo ‘export PATH=$PATH:$HOME/.rvm/bin’ >> ~/.bashrc` and press `<Enter>`
9. Close the "Ubuntu" application
10. Open the "Ubuntu" application using the "Start" menu
11. Type `rvm` and press `<Enter>`

### Check Your Work

If you see a long message ending in "For additional documentation, please visit
https://rvm.io", continue below.

## Install Ruby Version 2.6.1 on Ubuntu

For our Ruby labs and lessons, we expect that students use Ruby version 2.6.1 on
Ubuntu. If Ruby Environment Manager (RVM) has been successfully installed, you
can quickly install Ruby with a couple of commands.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. If the "Ubuntu" application is still open from the last step, close and
   re-open to prevent errors with running the next command.
3. Type `rvm install 2.6.1` and press `<Enter>`
4. Type `rvm list` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/GErkBvGIGu0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see a message starting with "=\* ruby-2.6.1", continue below. 

> **Note:** If you see that Ruby 2.6.1 is installed, but does not display
> `=*` before it, close and reopen the "Ubuntu" application, then run
> `rvm use 2.6.1 --default`.

## Install Ruby Gems on Ubuntu

Ruby Gems are small programs written in Ruby that help you to code more easily
in Ruby. The gems you will install today include: Bundler, which allows you to
keep track of which gems your projects need to work; Pry, which allows you to
pause your code when it runs and inspect it; Nokogiri, which allows you to read
and pick apart HTML pages; and Ruby on Rails, which allows you to easily create
a web application with Ruby.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. Type `gem update --system` and press `<Enter>`
3. Type `gem install bundler` and press `<Enter>`
4. Type `gem install pry` and press `<Enter>`
5. Type `gem install nokogiri` and press `<Enter>` (Note: this gem typically
   takes longer than the others to install)
6. Type `gem install rails` and press `<Enter>`
7. Type `gem install learn-co` and press `<Enter>`
8. Type `gem list | wc -l` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/RVwo7RPviNI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you are able to complete each step without any issues and you see an output
of a number around or above 100 from the last command, continue to the next lesson,
**Installing Node.js on WSL2**.
