![logo][]

`oh-my-zsh` is an open source, community-driven framework for managing
your [Zsh][] configuration.

It comes bundled with a ton of helpful functions, helpers, plugins,
themes, and a few things that make you shout…

> “OH MY ZSHELL!”

Setup
-----

`oh-my-zsh` should work with any recent release of [Zsh][]. The minimum
recommended version is **4.3.9**.

If not already installed, you can install [Zsh][] using the
command-line.

### The automatic installer… do you trust me?

You can install this via the command-line with either `curl` or `wget`.

#### via `curl`:

`curl -L http://git.io/LdtZ_g | sh`

#### via `wget`:

`wget --no-check-certificate http://git.io/LdtZ_g -O - | sh`

#### **Optionally**, change the install directory:

The default location is `~/.oh-my-zsh` (hidden in your home directory).

You can change the install directory with the `ZSH` environment
variable, either by running `export ZSH=/your/path` before installing,
or by setting it before the end of the install pipeline like this:

`curl -L http://git.io/LdtZ_g | ZSH=~/.dotfiles/zsh sh`

### The manual way

1\. Clone the repository:

`git clone git://github.com/ysmood/oh-my-zsh.git ~/.oh-my-zsh`

2\. **Optionally**, backup your existing `~/.zshrc` file:

`cp ~/.zshrc ~/.zshrc.orig`

3\. Create a new [Zsh][] config file by copying the [Zsh][] template
we’ve provided:

`cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc`

4\. Set [Zsh][] as your default shell:

`chsh -s /bin/zsh`

5\. Start or restart [Zsh][] by opening a new command-line window.

### Problems?

You *might* need to modify your `PATH` in `~/.zshrc` if you’re not able
to find some commands after switching to `oh-my-zsh`.

If you installed manually or changed the install location, check the
`ZSH` environment variable in `~/.zshrc`.

Usage
-----

-   enable the plugins you want in your `~/.zshrc` (take a look at the
    `plugins/` directory and the [wiki][] to see what’s available)
    -   example: `plugins=(git osx ruby)`
-   theme support: change the `ZSH_THEME` environment variable in
    `~/.zshrc`
    -   take a look at the `themes/` directory and the [wiki][1] to see
        what comes bundled with `oh-my-zsh`
-   & much, much more… take a look at the `lib/` directory to see what
    `oh-my-zsh` has to offer…

Useful
------

The [refcard][] is pretty useful for tips.

### Customization

If you want to override any of the default behaviors, just add a new
file (ending in `.zsh`) in the `custom/` directory.

If you have many functions that go well together, you can put them as a
`*.plugin.zsh` file in the `custom/plugins/` directory and then enable
this plugin (see ’[Usage][]

  [logo]: https://s3.amazonaws.com/ohmyzsh/oh-my-zsh-logo.png
  [Zsh]: http://www.zsh.org/
  [wiki]: https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins
  [1]: https://wiki.github.com/robbyrussell/oh-my-zsh/themes
  [refcard]: http://www.bash2zsh.com/zsh_refcard/refcard.pdf
  [Usage]: https://g
