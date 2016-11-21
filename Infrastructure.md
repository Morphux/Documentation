Morphux Server Infrastructure
=============================

# Overview

```
┌──────────────────────┐
│                      │
│   Packages Website   │
│                      │
└──────────────────────┘
```

Website that list all the packages available on the distribution.
Languages: PHP / HTML / CSS

```
┌──────────────────────┐
│                      │
│     Build system     │
│                      │
└──────────────────────┘
```

System that build new packages / new versions of packages, on multiple
arch through VMs.
Languages: Python ?

```
┌──────────────────────┐
│                      │
│      MPM server      │
│                      │
└──────────────────────┘
```

Server that respond to an user request to install a package.
Languages: C, Go, C++ ?

```
┌──────────────────────┐
│                      │
│   Package Database   │
│                      │
└──────────────────────┘
```

Server that stores informations about packages
Language: SQL


# Life of a package

- Maintainer create a package
- Package is send to the build system
- VMS build the package, check if there's no dependencies problems
- Build system fill out the package automatic information:
	- Size of the installed package
	- Compilation time
	- Files installed by the package
	- Extract the binaries installed by the package
- The build system add the package to the Package database
