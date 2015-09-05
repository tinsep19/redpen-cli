PKGBUILD for [redpen](http://redpen.cc).

# Usage

You can make redpen package on arch linux.

```
$ mkdir -p $HOME/abs
$ cd $HOME/abs
$ git clone https://github.com/tinsep19/redpen-cli.git
$ cd redpen-cli
$ makepkg
$ sudo pacman -U redpen-1.3-0-any.pkg.tar.xz
```

## Use redpen
You MUST set JAVA_HOME.

```
$ export JAVA_HOME=/usr/lib/jvm/java-8-openjdk
$ redpen -v
```
