recollections
=============

Base repo to manage development of all the recollections things.

* Vagrant
* Puppet
* App

## Bootstrap

`rake`

You should not need to make any commits to this super-repo after init.
This is just to make things clean.

## Usage
* Puppet Modules for Guest Machines should be placed in the `recollections/puppet/modules` directory. 
*Node management is handled in `recollections/puppet/manifests/site.pp`
