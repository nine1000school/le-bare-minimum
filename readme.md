# LE BARE MINIMUM (WIP)

Learn it (scrupulously), use it (with good faith), teach it (and become great).

## Le Linux

If your work OS is Windows, you're doomed.

macOS is kind of okeyish, but still, you will need to start with Linux.

You may ask why? The answer is simple and clear: because linux will be the de-facto kernel (see below for the meaning) of all the machines that will be running your code or that you will manage and monitor.

They say know your enemy, I say know your tools first.

Thus everything below is intended for a Linux user.

## LE MACHINE

### CPU

### RAM

### I/O DEVICES

### BINARY

## LE SYSTEM

### Kernel

### Operating System

### process & scheduler

### systemd

### inetd

### common folders

- /bin
- /boot
- /dev
- /etc
- /home
- /mnt
- /opt
- /sbin
- /tmp
- /usr
- /var

### environment variables

#### `PATH`

## LE COMMAND LINE INTERFACE

### commands & tools

#### `man`

`man` is your CLI "Bible", but not limited to the CLI actually. You can ask it about other things related to your system and such. For instance, try `man signal`.

Sometimes `man` has different entries (called "sections") for the same entry name; there are 9 sections: 1 to 9. Compare `man 1 read` and `man 2 read`.

1. General Commands Manual
2. System Calls Manual
3. Library Functions Manual
4. Kernel Interfaces Manual
5. File Formats Manual
6. Games Manual
7. Miscellaneous Information Manual
8. System Manager's Manual
9. Kernel Developer's Manual

#### `apropos`

Acts like a "search" command for `man` that will use the given keywords as a search term in the manuals' pages.

You can add `-s [SECTION]` to limit the entries to a specific section.

Try `apropos -s 1 ssh` and compare to `apropos -s 3 ssh`

You may need to initialize its database using:

```sh
sudo makewhatis
```

#### `whatis`

Similar to `apropos`, `whatis` will give you a list of pages that are directly related to the given term, with a short explanation.

Try `whatis df` and compare it to `apropos df`.

#### `which`

#### `find`

#### `tree`

#### `tmux`

#### `ag`

#### `lsof`

#### `awk`

#### `sed`

#### `nmap`

#### `cut`

#### `kill`

#### `true` & `false`

#### `ls`

#### `cd`

If you have to go back and forth between two folders or simply return to the previous directory you left:

```sh
cd -
```

### shell scripting

#### `||`

#### `&&`

#### `&`

#### `()`

#### `<`

#### `>` & `>>`

#### `|`

#### `[` aka `test`

#### indirections

- stdin (`0`)
- stdout (`1`)
- stderr (`2`)
