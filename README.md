# pmw : Package Manager Wrapper

パッケージ管理ツールのコマンドをラップするスクリプト。


## Intallation

```sh
# Copy 'pmw' file to the directory in PATH
$ cp ./pmw ~/bin/pmw

# Exec 'pmw' command
$ pmw in vim
```


## Available Main Commands

対応しているパッケージ管理ツールは以下のとおり。

- `dnf`
- `yum`
- `apt`
- `apt-get`
- `brew` (Homebrew)
- `pacman`


## Available Sub Commands

以下のサブコマンドが対応している。カッコ内はエイリアス。

- `install` (`i`・`in`)
- `remove` (`r`・`rm`・`un`・`uninstall`)
- `update` (`upd`)
- `upgrade` (`up`・`upg`)
- `search` (`find`)
- `list installed` (`ls installed`・`l`・`ls`・`list-installed`・`ls-installed`)
- `list available` (`ls available`・`L`・`la`・`list-available`・`ls-available`・`list --upgradable`・`ls --upgradable`・`list upgradable`・`ls upgradable`・`list-upgradable`・`ls-upgradable`)
- `info` (`show`)


## Examples

コマンドの実行例と変換後のコマンド。

- In CentOS (`yum` installed)

```sh
$ pmw install vim
# -> yum install vim

$ pmw up vim
# -> yum update vim
```

- In Ubuntu (`apt` installed)

```sh
$ pmw in -y vim
# -> apt install -y vim

$ pmw ls
# -> apt list installed
```

- In MacOS (`brew` installed)

```sh
$ pmw in vim
# -> brew install vim
```

- In Windows Git SDK (`pacman` installed)

```sh
$ pmw in vim
# -> pacman -S vim
```


## Author

[Neo](http://neo.s21.xrea.com/)

- [GitHub - pmw](https://github.com/Neos21/pmw)


## Links

- [Neo's World](http://neo.s21.xrea.com/)
- [Corredor](http://neos21.hatenablog.com/)
- [Murga](http://neos21.hatenablog.jp/)
- [El Mylar](http://neos21.hateblo.jp/)
- [Neo's GitHub Pages](https://neos21.github.io/)
- [GitHub - Neos21](https://github.com/Neos21/)
