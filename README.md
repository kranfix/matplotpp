MATPLOT++ (MATLAB-like plotting tool in C++)
--------------------------------------------

# What is this?

This is a fork from https://code.google.com/p/matplotpp/ and 


# Required library

We need to install freeglut

Ubuntu:

```
$ sudo apt-get install freeglut3-dev
```

Fedora:
```
$ sudo yum install freeglut-devel
```

# Compile MATPLOT++ library

Clone the repositoy:

```
git clone git@github.com:kranfix/matplotpp.git
```

Place into the project:

```
cd matplotpp
```

And excetute the Makefile:
```
make
```

# Compile the examples

Only type the following:

```
$ cd matplotpp
$ make build
```
