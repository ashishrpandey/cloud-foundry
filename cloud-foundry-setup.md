CF CLI setup on Ubuntu:

    $ wget -q -O - https://packages.cloudfoundry.org/debian/cli.cloudfoundry.org.key | sudo apt-key add -
    $ echo "deb http://packages.cloudfoundry.org/debian stable main" | sudo tee /etc/apt/sources.list.d/cloudfoundry-cli.list
    $ sudo apt-get update
    $ sudo apt-get install cf-cli

CF CLI setup on Centos:
Setup the yum package repository then install the cf CLI 

    $ sudo wget -O /etc/yum.repos.d/cloudfoundry-cli.repo https://packages.cloudfoundry.org/fedora/cloudfoundry-cli.repo
    $ sudo yum install cf-cli
    
Once you have installed the CLI tool, verify that it works, by opening a Terminal and running:
    
     $ cf --version
     
     cf version 6.40.0+07673feb9.2018-10-08
     
References:

Installation:
https://docs.cloudfoundry.org/cf-cli/install-go-cli.htmlhttps://docs.cloudfoundry.org/cf-cli/install-go-cli.html

Command reference:
http://cli.cloudfoundry.org/en-US/cf/
