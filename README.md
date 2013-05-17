Getting Started with Rake
=========================

A friendly introduction to rake, dependency programming, and being more productive.

The goal of this 'class' is to introduce you step-by-step to rake and how to use it and dependency programming to be more productive, while writing code that is easy to understand and maintain.

Prerequisites
-------------
In order to take advantage of this introduction to rake, you will need to have your environment setup properly. You will need to have a current generation Ruby installed. This means if you are on Mac OS X, you will not be using the default Ruby install.

To help you in managing your Ruby environemnt, we will introduce you to _rbenv_, which will help you to create a sandbox environment in which to work, without polluting your standard environment.

My instructions below assume that you are on Mac OS X. If you are running on Linux or Windows, you will have to adapt them as required.

### brew
As part of this process, you will need to install various packages that will need to be built from source. To ease that process for you, I recommend that you install the Mac OS X package manager, [_HomeBrew_](http://mxcl.github.io/homebrew/).

Installing _HomeBrew_ (or _brew_ as its friends call it) is trivially easy.  Fire up your terminal of choice, paste the line below, and run it.
````
    $ ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
````
The _brew_ script will explain what it does and give you the opportunity to bail out if you so choose.

###### Important Point!
Run this command - and all others I ask you to run - as a local user, not root. Trust me that in the long run it iwll make your life easier. There are places and times to run these commands as root, but this is not one of them.

### rbenv
Now that we have _brew_ installed, it is time to install [_rbenv_](https://github.com/sstephenson/rbenv/), a Ruby environment manager that will allow you to create a 'sandbox' in which to experiment without polluting the rest of your system.

Because we have _brew_ installed, installing _rbenv_ and its associated components as almost as trivally easy as installing _brew_. 

Just open up your terminal - maybe you left it open from installing _brew_ and type:

````
    $ brew update
        - This will bring _brew_ up to date and make sure you have the latest 'formulas' (_brew-speak_ for package          
        definitions) in hand.
        
    $ brew install rbenv
        - Install _rbenv_ for you
        
    $ brew install ruby-build
        - Install the ruby-build tools you will need.
````
Now you need to add a little magic to your .bashrc or .bash_profile, just pop up your favorite editor and add the following `eval "$(rbenv init -)"` at the end of it. Once you have done this, source it, to make sure these changes take effect:
````
    $ source .bashrc
````
Now we need to add a few 'accessories' to rbenv to make it easier to use:
````
    $ brew install rbenv-gem-rehash
    $ brew install rbenv-gemset
    $ brew install rbenv-bundler
````

And then let's get our first Ruby installed:
````
   $ 
    

    
    
    



