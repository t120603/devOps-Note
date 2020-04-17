# Install for macOS

## Homebrew
- [official Website](https://brew.sh/)

### Install Homebrew
- This command copy from official website

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

### CLI Usage Sample

```
brew info azure-cli
brew update
brew install azure-cli
```


[Philip feedback]
I ran into following error message when execute "brew install azure-cli"

Updating Homebrew...
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig
/usr/local/share/man/man5
/usr/local/share/man/man7

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig /usr/local/share/man/man5 /usr/local/share/man/man7

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig /usr/local/share/man/man5 /usr/local/share/man/man7

Not sure what I done, finally, the installation was completed.
