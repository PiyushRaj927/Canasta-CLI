# Canasta-CLI-Go
The Canasta command line interface, written in Go

# Installation
Make sure you have the `go` compiler installed (at least 1.18) and set your `$GOPATH`

Clone the repo

`git clone git@github.com:CanastaWiki/Canasta-CLI-Go.git`

Checkout into the `dev` branch

`git checkout dev`

Install Canasta.go

`go install canasta.go`

Now you should be able to access the `canasta` cli from any directories

# Documentation

``` A CLI tool to create, import, start, stop and backup multiple Canasta installations

Usage:
  canasta [command]

Available Commands:

  completion  Generate the autocompletion script for the specified shell

  create      Create a Canasta Installation
  
  delete      delete a  Canasta installation
  
  help        Help about any command
  
  import      Create a Canasta Installation
  
  list        list all  Canasta installations
  
  start       Start the Canasta installation
  
  stop        Stop the Canasta installation

Flags:
  -h, --help   help for canasta

Use "canasta [command] --help" for more information about a command.
```

# Example

create

` sudo canasta create -w "My Wiki" -n wiki.my.com -i mywiki -a admin -o docker-compose `

This command will create a canasta installation with a Wiki named ` My Wiki `, hosted at domain ` wiki.my.com `, admin name as ` admin `, using the orchestrator ` docker-compose `. This also sets a unique ID `mywiki` to the Installation. Which can be used to start, stop, delete instances without moving into the installation folder.