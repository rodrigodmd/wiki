# Nvm



# [Install Mac](http://dev.topheman.com/install-nvm-with-homebrew-to-use-multiple-versions-of-node-and-iojs-easily/)

Install nvm with [Homebrew](../Mac/Homebrew.md):

    brew update
    brew install nvm
# Install linux

TBD


# Useful commands

If you want to see what versions are installed:

    nvm ls

If you want to see what versions are available to install:

    nvm ls-remote

Install a new node version:

    nvm install <version>

Use specific version 

    nvm use <version>

To set a default Node version to be used in any new shell, use the alias 'default':

    nvm alias default <version>