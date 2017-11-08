# git-upstream

Type `git upstream` to automatically assign your git upstream url.

## Usage

```sh
git upstream
```

## Installation

### Basic install

The preferred way of installation is to simply add the `git-upstream` script
somewhere into your path (e.g. add the directory to your `PATH` environment or
copy `git-upstream` into an existing included path like `/usr/local/bin`).

### Install via NPM:

```sh
npm install --global jonathantneal/git-upstream
```

### Windows Powershell

Save git-upstream anywhere, say as ~/Documents/Scripts/git-upstream.sh and
define a function in your Powershell profile
(see ~/Documents/WindowsPowerShell/profile.ps1) like this:

```sh
function git-upstream { cmd /c "C:\Program Files\Git\usr\bin\bash.exe" "~/Documents/Scripts/git-upstream.sh" }
Set-Alias -Name gop -Value git-upstream
```

### Windows with `cmd` terminal

Save the `git-upstream` script in any place accessible via your `%PATH%`
environment var.

### ZSH

#### [Antigen](https://github.com/zsh-users/antigen)

Add `antigen bundle jonathantneal/git-upstream` to your `.zshrc` with your
other bundle commands.

Antigen will handle cloning the plugin for you automatically the next time you
start zsh, and periodically checking for updates to the git repository. You can
also add the plugin to a running zsh with
`antigen bundle jonathantneal/git-upstream` for testing before adding it to
your `.zshrc`.

#### [Oh-My-Zsh](http://ohmyz.sh/)

1. `cd ~/.oh-my-zsh/custom/plugins`
1. `git clone https://github.com/jonathantneal/git-upstream.git`
1. Add `git-upstream` to your plugin list - edit `~/.zshrc` and change
   `plugins=(...)` to `plugins=(... git-upstream)`

#### [Zgen](https://github.com/tarjoilija/zgen)

Add `zgen load jonathantneal/git-upstream` to your .zshrc file in the same
function you're doing your other `zgen load` calls in. ZGen will take care of
cloning the repository the next time you run `zgen save`, and will also
periodically check for updates to the git repository.

#### [zplug](https://github.com/zplug/zplug)

`zplug "jonathantneal/git-upstream", as:plugin`


## Related projects

- [`git open`](https://github.com/paulirish/git-open) - Open your repo website
- [`git recent`](https://github.com/paulirish/git-recent) - View your most
  recent git branches
- [`diff-so-fancy`](https://github.com/so-fancy/diff-so-fancy/) - Making the
  output of `git diff` so fancy
