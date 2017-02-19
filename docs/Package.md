# Morphux Package Manager

## What is a Package Manager
A package manager keeps track of what software is installed on your computer,
and allows you to easily install new software, upgrade software to newer
versions, or remove software that you previously installed. As the name
suggests, package managers deal with packages: collections of files that are
bundled together and can be installed and removed as a group.

## MPM
Mpm is the morphux package manager. If you're familiar with other package
managers like apt, pkg, etc. it's about the same.

## Install a Package
Open a terminal, and type:
```
sudo mpm install pkg/name
```
Let's deconstruct this command:

- ```sudo```: Give the root power to this command (Required for installing a
program)
- ```mpm```: Mpm binary
- ```install```: Install command
- ```pkg/```: Category of the package
- ```name```: Name of the package

## Categories
As you can read above, mpm works with package categories. Here's all the
supported categories:

- ```pkg/```: Basic linux packages
- ```lib/```: Developer libraries, with headers
- ```kernel/```: Kernel sources and tools
- ```virt/```: Virtualization tools
- ```graphic/```: Graphic utilities
- ```fonts/```: Fonts
- ```sys/```: System utilities
- ```programming/```: Programming utilities
- ```net/```: Networking utilities
- ```servers/```: Servers
- ```python/```: Python packages, provided by pip
- ```X/```: X utilities
- ```wayland/```: Wayland utilities
- ```kde/```: Kde packages
- ```gnome/```: Gnome packages
- ```xfce/```: Xfce packages
- ```lxde/```: Lxde packages
- ```lxqt```: Lxqt packages
- ```multimedia/```: Multimedia packages
- ```node/```: NodeJS packages, provided by npm
- ```vim/```: Vim plugins, provided by Vim-Awesome
- ```irssi/```: Irssi scripts / themes, provided by Irssi
- ```go/```: Go packages, provided by Glide
- ```php/```: PHP Packages, provided by Composer
- ```latex/```: Latex packages, provided by CTAN
- ```java/```: Java packages, provided by Gradle
- ```lua/```: Lua Packages, provided by LuaRocks
- ```lisp/```: Lisp packages, provided by Quicklisp
- ```ruby/```: Ruby packages, provided by RubyGems
- ```scala/```: Scala packages, provided by sbt
- ```rust/```: Rust packages, provided by cargo
- ```perl/```: Perl modules, provided by cpan
