# Gnome custom settings

Just a few scripts to quickly set up GNOME Shell.

# Usage

These are a set of scripts that provide some useful functions to modify some of GNOME Shell (and GNOME Shell extensions)'s settings from the CLI.  They will come in handy if you need to repeatedly change a lot of stuff in fresh installations of GNOME/Ubuntu/debian etc.

It's a two steps process:

- Change the desired settings in the helper scripts.
- Apply the changes with the provided functions.

Optionally, you can clear some settings too if needed.

## Applying the changes

From the `scripts` directory, source the script:

```sh
$ . customise_gnome_shell

```

That won't change anything yet.  It will give you some functions that you can invoke to change settings/keybindings.

Then you can:

### Show the current keybindings:

```sh
$ get_keybindings

```

### Delete all selected keybindings:

I found it useful not to have assigned keys to stuff I do not normally use.  That way I don't get unexpected behaviour when I accidentally hit a key and it turns out it has an action bound to it i.e. launching an app or executing a GNOME Shell/WM command.

```sh
$ delete_keybindings

```

### Set the desired keybindings:

If you have set up the desired keys on the helper scripts (or you're happy with the ones provided).

```sh
$ set_keybindings

```

## WIP

Scripts for extensions (i.e. PaperwM) and other settings are on their way!
