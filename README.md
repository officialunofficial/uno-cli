# Uno CLI

Release downloads for the Uno command-line client. Source development lives in a separate internal repository.

## Install

On macOS with Apple silicon:

```sh
brew install --cask officialunofficial/tap/uno
```

On macOS or Linux:

```sh
curl -fsSL https://github.com/officialunofficial/uno-cli/releases/download/uno-cli-latest/install.sh | sh
```

The installer checks the archive against the release's `SHA256SUMS` file. Add `$HOME/.uno/bin` to your `PATH`.

```sh
uno --version
uno doctor
uno --help
```

macOS releases include a Developer ID signed and notarized passkey helper. Linux supports guest Kit commands. Account login requires macOS. Linux builds use glibc and are tested on Ubuntu 22.04 and Debian 12.

## Update

Curl installations support `uno update` and `uno update --rollback`.
For Homebrew installations, run `brew upgrade --cask uno`.
Set `UNO_NO_AUTO_UPDATE=1` to disable automatic updates on curl installations.

The `uno-cli-latest` release contains a moving `LATEST` pointer and the installer.
Download each platform archive from its versioned release.

Learn about Uno at [uno.fun](https://uno.fun).
