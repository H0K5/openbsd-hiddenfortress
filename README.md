openbsd-hiddenfortress
====================

Setup a minimal [OpenBSD](http://openbsd.org/) virtual machine with [Tor](https://www.torproject.org/) + [polipo](http://www.pps.univ-paris-diderot.fr/~jch/software/polipo/) + a few web browsers.
Intended as a quick way to provision a secure Tor environment for improved privacy and security.

Prerequisites
-------------
- Working [Vagrant](http://www.vagrantup.com/) install
- [VirtualBox](https://www.virtualbox.org/)
- Ssh client
- X11 Install _(Graphical browsers coming soon!)_

Instructions
------------
- `vagrant up`
- *ignore warnings about missing interface*
- `vagrant provision`
- `vagrant ssh`
- `lynx -dump -nolist http://check.torproject.org/`

        Congratulations. Your browser is configured to use Tor.
        Please refer to the Tor website for further information about using Tor
        safely. You are now free to browse the Internet anonymously.

Todo
----
- [ ] X11 installation
  - [ ] Chromium
  - [ ] Firefox
- [ ] En3crypt root file system with session key?
- [ ] Build VM using [Packer](http://packer.io/)
<pre>
                                     /)
                                    //
                  __*_             //
               /-(____)           //
              ////- -|\          //
           ,____o% -,_          //
          /  \\   |||  ;       //
         /____\....::./\      //
        _/__/#\_ _,,_/--\    //     THIS IS A SAMURAI
        /___/######## \/""-(\</
       _/__/ '#######  ""^(/</    NOT A NINJA
     __/ /   ,)))=:=(,    //.
    |,--\   /Q...... /.  (/     SO YOU FUCKING IDIOT BACON ZOMBIE
    /       .Q....../..\         NERDS DON'T EVEN GET STARTED
           /.Q ..../...\
          /......./.....\
          /...../  \.....\
          /_.._./   \..._\
           (` )      (` )
           | /        \ |
           '(          )'
          /+|          |+\
          |,/          \,/  b'ger
</pre>

