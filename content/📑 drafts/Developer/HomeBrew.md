https://brew.sh/

**The Missing Package Manager for macOS (or Linux)**

# [Command Documentation](https://docs.brew.sh/Manpage)

## SYNOPSIS

`brew` `--version`  
`brew` _`command`_ [`--verbose`|`-v`] [_`options`_] [_`formula`_] …

## DESCRIPTION

Homebrew is the easiest and most flexible way to install the UNIX tools Apple didn’t include with macOS. It can also install software not packaged for your Linux distribution without requiring `sudo`.

## SYNOPSIS

`brew` `--version`  
`brew` _`command`_ [`--verbose`|`-v`] [_`options`_] [_`formula`_] …

## DESCRIPTION

Homebrew is the easiest and most flexible way to install the UNIX tools Apple didn’t include with macOS. It can also install software not packaged for your Linux distribution without requiring `sudo`.

---

## TERMINOLOGY

**formula**

Homebrew package definition that builds from upstream sources

**cask**

Homebrew package definition that installs macOS native applications

**prefix**

path in which Homebrew is installed, e.g. `/opt/homebrew` or `/home/linuxbrew/.linuxbrew`

**keg**

installation destination directory of a given **formula** version, e.g. `/opt/homebrew/Cellar/foo/0.1`

**rack**

directory containing one or more versioned **kegs**, e.g. `/opt/homebrew/Cellar/foo`

**keg-only**

a **formula** is _keg-only_ if it is not symlinked into Homebrew’s prefix

**opt prefix**

a symlink to the active version of a **keg**, e.g. `/opt/homebrew/opt/foo`

**Cellar**

directory containing one or more named **racks**, e.g. `/opt/homebrew/Cellar`

**Caskroom**

directory containing one or more named **casks**, e.g. `/opt/homebrew/Caskroom`

**external command**

`brew` subcommand defined outside of the Homebrew/brew GitHub repository

**tap**

directory (and usually Git repository) of **formulae**, **casks** and/or **external commands**

**bottle**

pre-built **keg** poured into a **rack** of the **Cellar** instead of building from upstream sources


---
## ESSENTIAL COMMANDS

For the full command list, see the [COMMANDS](https://docs.brew.sh/Manpage#commands) section.

With `--verbose` or `--debug`, many commands print extra debugging information. Note that these options should only appear after a command.

Some command behaviour can be customised with environment variables; see the [ENVIRONMENT](https://docs.brew.sh/Manpage#environment) section.

### `install` _`formula`_

Install _`formula`_.

_`formula`_ is usually the name of the formula to install, but it has other syntaxes which are listed in the [SPECIFYING FORMULAE](https://docs.brew.sh/Manpage#specifying-formulae) section.

### `uninstall` _`formula`_

Uninstall _`formula`_.

### `list`

List all installed formulae.

### `search` [_`text`_|`/`_`text`_`/`]

Perform a substring search of cask tokens and formula names for _`text`_. If _`text`_ is flanked by slashes, it is interpreted as a regular expression. The search for _`text`_ is extended online to `homebrew/core` and `homebrew/cask`. If no search term is provided, all locally available formulae are listed.