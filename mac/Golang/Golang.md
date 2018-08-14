# Golang

Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.

More info: https://golang.org/
# [Install Go Mac](http://sourabhbajaj.com/mac-setup/Go/README.html)

Install Golang with [Homebrew](../Homebrew.md):
    
    brew install golang

Go has a different approach of managing code, you'll need to create a single Workspace for all your Go projects. For more information consult [How to write Go Code](https://golang.org/doc/code.html#Workspaces).

Open your bash_profile to configure the environment variables:
    
    vi $HOME/.bash_profile

Then add those lines to export the required variables:

    export GOPATH=$HOME/Documents/go-workspace # don't forget to change your path correctly!
    export PATH=$PATH:$GOPATH/bin

Create the workspace directories tree:

    mkdir -p $GOPATH $GOPATH/src $GOPATH/pkg $GOPATH/bin


# Install Go Linux

    Not Docuemented Yet