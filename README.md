# Chili Piper CLI

`chili-piper-cli` is a command-line client for the [Chili Piper](https://www.chilipiper.com) Edge API.
It offers the same operations as the Chili Piper MCP server.

## Install

macOS (Apple Silicon) and Linux (x86_64), with [Homebrew](https://brew.sh):

```sh
brew install chili-piper/tap/chili-piper-cli
```

Windows (x86_64), with [Scoop](https://scoop.sh):

```powershell
scoop bucket add chili-piper https://github.com/Chili-Piper/homebrew-tap
scoop install chili-piper/chili-piper-cli
```

Or download the binary for your platform from [Releases](https://github.com/Chili-Piper/homebrew-tap/releases).

## Set up

Create an API key in Chili Piper: **Admin Center > API Keys**. Give it only the scopes you need.

```sh
export CHILI_PIPER_API_HOST=https://fire.chilipiper.com/api/fire-edge
export CHILI_PIPER_API_KEY=<your-api-key>
chili-piper-cli health ping
```

You can also pass `--host` and `--token` to each command.
Use `--help` at any level, for example `chili-piper-cli meeting --help`.

## Updates

Each release of the Chili Piper backend publishes a new CLI version here.

```sh
brew upgrade chili-piper-cli    # Homebrew
scoop update chili-piper-cli    # Scoop
```

Check for updates: `chili-piper-cli check-update`

## Terms of use

Use of the CLI is subject to the [Terms of Use](TERMS.md).

## Support

This repository only distributes binaries. The source code is not public.
For help, contact Chili Piper support.
