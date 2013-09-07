GitHub Pages Jekyll Environment for Vagrant
====================

Simple Vagrant file to build a GitHub Pages-compatible Jekyll environment. Uses the "official" github-pages gem. Use this environment to build and test your GitHub Pages-based jekyll sites without polluting your host box.

How to use
--------------------

First, make sure you've installed [Vagrant](http://docs.vagrantup.com/v2/getting-started/index.html) and [VirtualBox](https://www.virtualbox.org/).

Next, clone this repo.

```
git clone git@github.com:rjsilk/vagrant-github-pages.git
```

Now, `cd` into that directory and start up the Vagrant VM. 

```
cd vagrant-github-pages
vagrant up
```

Finally, you can ssh into the vm and do all your Jekyll-related work in there.

```
vagrant ssh
```

Note on SSH-forwarding
---------------------
The Vagrantfile enables ssh-forwarding so that you can use your host ssh keys to authenticate with github. Make sure to add you keys to the agent with ```ssh-add``` before running ```vagrant ssh``` if your keys aren't automatically added to the agent.
