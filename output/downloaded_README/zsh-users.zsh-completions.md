zsh-completions ![GitHub release](https://img.shields.io/github/release/zsh-users/zsh-completions.svg) ![GitHub contributors](https://img.shields.io/github/contributors/zsh-users/zsh-completions.svg) [![IRC](https://img.shields.io/badge/IRC-%23zsh--completions-yellow.svg)](irc://irc.freenode.net/#zsh-completions) [![Gitter](https://badges.gitter.im/zsh-users/zsh-completions.svg)](https://gitter.im/zsh-users/zsh-completions?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
=============

**Additional completion definitions for [Zsh](http://www.zsh.org).**

*This projects aims at gathering/developing new completion scripts that are not available in Zsh yet. The scripts may be contributed to the Zsh project when stable enough.*


## Status

See [issues](https://github.com/zsh-users/zsh-completions/issues) for details on each completion definition.


## Usage

### Using packages

| System  | Package |
| ------------- | ------------- |
| Debian / Ubuntu | [zsh-completions OBS repository](https://software.opensuse.org/download.html?project=shells%3Azsh-users%3Azsh-completions&package=zsh-completions) |
| Fedora / CentOS / RHEL / Scientific Linux | [zsh-completions OBS repository](https://software.opensuse.org/download.html?project=shells%3Azsh-users%3Azsh-completions&package=zsh-completions) |
| OpenSUSE / SLE | [zsh-completions OBS repository](https://software.opensuse.org/download.html?project=shells%3Azsh-users%3Azsh-completions&package=zsh-completions) |
| Arch Linux | [zsh-completions](https://www.archlinux.org/packages/zsh-completions), [zsh-completions-git](https://aur.archlinux.org/packages/zsh-completions-git) |
| Gentoo | [app-shells/zsh-completions](http://packages.gentoo.org/package/app-shells/zsh-completions)  |
| NixOS | [zsh-completions](https://github.com/NixOS/nixpkgs/blob/master/pkgs/shells/zsh-completions/default.nix) |
| Void Linux | [zsh-completions](https://github.com/voidlinux/void-packages/tree/master/srcpkgs/zsh-completions) |
| Mac OS | [homebrew](https://github.com/Homebrew/homebrew-core/blob/master/Formula/zsh-completions.rb), [MacPorts](https://github.com/macports/macports-ports/blob/master/sysutils/zsh-completions/Portfile)  |

### Using zsh frameworks

#### [antigen](https://github.com/zsh-users/antigen)

Add `antigen bundle zsh-users/zsh-completions` to your `~/.zshrc`.

#### [oh-my-zsh](http://github.com/robbyrussell/oh-my-zsh)

* Clone the repository inside your oh-my-zsh repo:

        git clone https://github.com/zsh-users/zsh-completions ~/.oh-my-zsh/custom/plugins/zsh-completions

* Enable it in your `.zshrc` by adding it to your plugin list and reloading the completion:

        plugins=(… zsh-completions)
        autoload -U compinit && compinit

### Manual installation

* Clone the repository:

        git clone git://github.com/zsh-users/zsh-completions.git

* Include the directory in your `$fpath`, for example by adding in `~/.zshrc`:

        fpath=(path/to/zsh-completions/src $fpath)

* You may have to force rebuild `zcompdump`:

        rm -f ~/.zcompdump; compinit

### Contributing

Contributions are welcome, just make sure you follow the guidelines:

 * Completions are not accepted when already available in zsh.
 * Completions are not accepted when already available in their original project.
 * Please do not just copy/paste someone else completion, ask before.
 * Completions only partially implemented are not accepted.
 * Please add a header containing authors, status and origin of the script and license header if you do not wish to use the Zsh license (example [here](src/_ack)).
 * Please try to follow [Zsh completion style guide](https://github.com/zsh-users/zsh/blob/master/Etc/completion-style-guide).
 * Please send one separate pull request per file.
 * Send a pull request or ask for committer access.


## License
Completions use the Zsh license, unless explicitely mentionned in the file header.
See [LICENSE](https://github.com/zsh-users/zsh-completions/blob/master/LICENSE) for more information.
