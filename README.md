# Provision a local Vagrant VM with Ansible

A recent version of Vagrant and Ansible is required to complete this project.
We'll be reviewing your work using Vagrant 2.2+ and Ansible 2.9+, and we'll be
using the VirtualBox Vagrant provider with VirtualBox version 6.1+.

Using a copy of this repository as a starting point, update `playbook.yml` and 
other files as needed to complete the following tasks on the Vagrant VM.  You are 
encouraged to make use of files, templates, handlers, and other Ansible features.

In the COMMENTS.md file provided, please add any notes on running your
solution, ambiguities that you found, assumptions that you made, or any other 
comments that you feel are relevant. 

Additionally, please provide inline comments in `playbook.yml`, and other
files as appropriate.

We expect it should take 1-2 hours to complete this exercise. When completed, 
please send us a tar file of the final state of the repo. Please do include your 
`.git` directory so we can see your commits, but DO NOT include the `.vagrant` 
directory, or the virtual machine.   


Notes: 

* It is *not* neccessary for you playbook to complete the exercise in order to submit, 
but please do note any unmet requirements in your COMMENTS.md file, and discuss what you 
might do next in order to meet them. 

* To shorten your development time, you may want to run `vagrant rsync` and 
`vagrant provision` to update and test new versions of your playbook, rather 
than rebuiling the VM completely. 

## Configure a Static Site 

Your playbook should do the following. 

* Install Nginx, start it up, and configure it to start on system boot. 
* Configure Nginx to accept https requests on port 443 using a self-signed ssl
  certificate. 
* Configure Nginx to redirect all http requests to their https equivalent. 
* Create `/srv/my-site/htdocs` and copy `files/index.html` there. Make this
  top level index page for visitors to the default site of the web server.   
* Make sure SELinux is active and enforcing. 

## Bonus Task: Install PHP 7

* Install PHP 7.x. Document why you chose the PHP that you did in COMMENTS.md 
* Copy `files/phpinfo.php` and configure Nginx so that the script runs and
  displays its output whenever anyone visits the location `/phpinfo.php`.    


## Credits

This exercise was based on Ad Hoc's [Provision](https://homework.adhoc.team/provision/) exercise. 
