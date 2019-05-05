Freedomotic Open IoT Framework
=================================
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/48aa004c305547b7bda625f78a8363c0)](https://www.codacy.com/app/mcicolella/freedomotic?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=freedomotic/freedomotic&amp;utm_campaign=Badge_Grade)
[![Code Triagers Badge](https://www.codetriage.com/freedomotic/freedomotic/badges/users.svg)](https://www.codetriage.com/freedomotic/freedomotic)
[![](https://dockerbuildbadges.quelltext.eu/status.svg?organization=freedomotic&repository=freedomotic)](https://hub.docker.com/r/freedomotic/freedomotic/builds/) 

Official website is https://www.freedomotic-iot.com

Freedomotic is an open source, flexible, secure Internet of Things (IoT) application framework, useful to build and manage modern smart spaces. It is targeted to private individuals (home automation) as well as business users (smart retail environments, ambient aware marketing, monitoring and analytics, ...)

Freedomotic can run also on **Raspberry Pi** and can easily interact with DIY **Arduino** projects.

Starting from 2 Feb 2014, this is the Freedomotic mainstream repository. Previous repository was hosted on googlecode http://code.google.com/p/freedomotic

Requirements: 
- **Java Open JDK** version 8 or Oracle jdk _(to install Un ubuntu: sudo apt-get install openjdk-8-jdk)_
- **Maven** version 2 or 3 _(to install on Ubuntu: sudo apt-get install maven)_
- **Any OS** with java support _(Linux, Windows, Mac, Solaris ...)_

Development status:
- **Current released version**: 5.6.0 'Commander RC4' (released on 16 Aug 2017)
- **Version in development (HEAD of this repository)**: 5.6.0 'Commander'


Quick Start
======================

Follow these instructions if you want to compile Freedomotic from source (eg: to develop your own plugins). If you just want to try it, just download the precompiled binaries you can find at the official download page https://sourceforge.net/projects/freedomotic/

**1) Fork Freedomotic on GitHub**

* Create an account on https://github.com if you don't have one.
* **Fork Freedomotic** [_(What does it mean?)_](https://help.github.com/articles/fork-a-repo) following this link: <https://github.com/freedomotic/freedomotic/fork>. 
* Create the local clone of your online fork with this command:

```
git clone https://github.com/YOUR-GITHUB-USERNAME/freedomotic.git
```

Now the repository is ready to work with.

**2) Enter the new local folder**

    cd freedomotic
    
**3) Compile Freedomotic with maven**

    mvn clean install
    
**4) IMPORTANT!!!! THIS IS REQUIRED: Copy the example-data folder into freedomotic-core/data.** If you miss this step Freedomotic won't start

    cp -r data-example/ framework/freedomotic-core/data
    
**5) Run Freedomotic**

    java -jar framework/freedomotic-core/target/freedomotic-core/freedomotic.jar

As an alternative you can start **freedomotic-core** project from your favourite IDE.
    

Demo
====

An online demo is kindly hosted for free by our tech partner [Appcademy - Florence](https://appcademy.tech/).

Go to
- [API demo](http://51.77.212.115:9111/)
- [Vue Web client - under development](http://fd-vue-webapp.herokuapp.com/) | [GitHub repository](https://github.com/freedomotic/fd-vue-webapp)


Getting help
============

Having trouble with Freedomotic? We’d like to help!

- Check out the [user manual](http://freedomotic-user-manual.readthedocs.io) for reference documentation. 
- Write on the [mailing list](https://groups.google.com/forum/#!forum/freedom-domotics)
- Send an email to info@freedomotic-iot.com
- Open an issue on https://github.com/freedomotic/freedomotic/issues

Contributing
============

Want to help us? It's very simple and funny. [Here](https://github.com/freedomotic/freedomotic/blob/master/CONTRIBUTING.md) how to do.

License
=============

Freedomotic is an Open Source software released under the [GNU GPLv2](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) license.
