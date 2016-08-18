## Installation

The first step to using Rust is to install it. You’ll need an internet
connection to run the commands in this chapter, as we’ll be downloading Rust
from the internet.

We’ll be showing off a number of commands using a terminal, and those lines all
start with `$`. You don't need to type in the `$`s; they are there to indicate
the start of each command. You’ll see many tutorials and examples around the web
that follow this convention: `$` for commands run as a regular user, and `#`
for commands you should be running as an administrator. Lines that don't start
with `$` are typically showing the output of the previous command.

### Installing on Linux or Mac

If you're on Linux or a Mac, all you need to do is open a terminal and type
this:

```bash
$ curl https://sh.rustup.rs -sSf | sh
```

This will download a script and start the installation. You may be prompted for
your password. If it all goes well, you’ll see this appear:

```bash
Rust is installed now. Great!
```

### Installing on Windows

If you're on Windows, please go to [rustup.rs](https://rustup.rs/) and follow
the instructions to download rustup-init.exe. Run that and follow the rest of
the instructions.

The rest of the Windows-specific commands in the book will assume that you are
using `cmd` as your shell. If you use a different shell, you may be able to run
the same commands that Linux and Mac users do. If neither work, consult the
documentation for the shell you are using.

### Uninstalling

Uninstalling Rust is as easy as installing it. From your shell, run
the uninstall script:

```bash
$ rustup self uninstall
```

### Troubleshooting

If you've got Rust installed, you can open up a shell, and type this:

```bash
$ rustc --version
```

You should see the version number, commit hash, and commit date in a format
similar to this for the latest stable version at the time you install:

```bash
rustc x.y.z (abcabcabc yyyy-mm-dd)
```

If you see this, Rust has been installed successfully!
Congrats!

If you don't and you're on Windows, check that Rust is in your `%PATH%` system
variable.

If it still isn't working, there are a number of places where you can get help.
The easiest is [the #rust IRC channel on irc.mozilla.org][irc], which you can
access through [Mibbit][mibbit]. Go to that address, and you'll be chatting with
other Rustaceans (a silly nickname we call ourselves) who can help you out.
Other great resources include [the user’s forum][users] and [Stack
Overflow][stackoverflow].

[irc]: irc://irc.mozilla.org/#rust
[mibbit]: http://chat.mibbit.com/?server=irc.mozilla.org&channel=%23rust
[users]: https://users.rust-lang.org/
[stackoverflow]: http://stackoverflow.com/questions/tagged/rust

### Local documentation

The installer also includes a copy of the documentation locally, so you can
read it offline. Run `rustup doc` to open the local documentation in your
browser.
