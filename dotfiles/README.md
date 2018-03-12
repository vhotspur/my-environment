# My dot files settings

`$MY_PATH` refers to root of this repository.


## `bashrc-use` (`~/.bashrc`, `~/.use.rc`)

* quick change of alternative for one console
* following configuration (`~/.use.rc`) is for two JDKs on Arch Linux
    *  `use java 8` switches to JDK8
    *  `use java 9` switches to JDK9

```text
java 8 path /usr/lib/jvm/java-8-jdk/bin/
java 8 env JAVA_HOME=/usr/lib/jvm/java-8-jdk/
java 9 path /usr/lib/jvm/java-9-openjdk/bin/
java 9 env JAVA_HOME=/usr/lib/jvm/java-9-openjdk/
```


## `bashrc-*` (`~/.bashrc`)

```shell
. $MY_PATH/dotfiles/bashrc-*
```


## `gitconfig` (`~/.gitconfig`)

```text
[include]
	path = $MY_PATH/dotfiles/gitconfig
```

## `Rprofile` (`~/.Rprofile`)

Just a symlink.

