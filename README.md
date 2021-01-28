# Provision a local Vagrant VM with Ansible

A recent version of Vagrant and Ansible is required to complete this project.
We'll be reviewing your work using Vagrant 2.2+ and Ansible 2.9+, and we'll be
using the VirtualBox Vagrant provider with VirtualBox version 6.1+.

Using the provided files as a starting point, write a playbook that completes
the following tasks on the vagrant VM.  These tasks can be completed in any
order, and you are encouraged to make use of files, templates, handlers, and
other Ansible features as needed. 

In the COMMENTS.md file provided, please add any notes on running your
solution, ambiguities that you found, assumptions that you made, or any other 
comments that you feel are relevant. 

Additionally, please provide inline comments in your new playbook, and other
files as appropriate.

Note: It is *not* neccessary for you playbook to complete all of the following
tasks in order to submit, but please do note any unmet requirements in your
COMMENTS.md file, and discuss what you might do next in order to meet them. 

## Part 1 - Static Site 

To complete Part 1, your playbook should do the following. 

* Install Nginx, start it up, and configure it to start on system boot. 
* Configure Nginx to accept https requests on port 443 using a self-signed ssl
  certificate. 
* Configure Nginx to redirect all http requests to their https equivalent. 
* Create `/srv/my-site/htdocs` and copy `files/index.html` there. Make this
  top level index page for visitors to the default site.   
* Make sure SELinux is active and enforcing. 

## Part 2 - 

* Install PHP 7.x 
* Copy `files/phpinfo.php` and configure Nginx so that the script runs and
  displays its output whenever anyone visits the location `/phpinfo.php`.    

## Credits

This exercise was based on Ad Hoc's [Provision](https://homework.adhoc.team/provision/) exercise. 
