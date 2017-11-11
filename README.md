# projectile-ghcid

Use [ghcid](https://github.com/ndmitchell/ghcid) within your [projectile](http://projectile.readthedocs.io/en/latest/) projects.

## Installation

To install projectile-ghcid manually, place projectile-ghcid.el in a directory of your choice, add it to your load path and require 'projectile-ghcid:

```
(add-to-list 'load-path "/path/to/projectile-ghcid/")
(require 'projectile-ghcid)
```

## Requirements

* `ghcid` v0.6.8 or greader somewhere on your path
* `projectile` installed in your Emacs
* a `.ghcid` file in the root of your project

## Usage

projectile-ghcid exposes a few interactive commands.

### `projectile-ghcid`

Spawn a new ghcid terminal inside your projectile root. This will
automatically pick up the configuration from the `.ghcid` file and run
the command there.

### `projectile-ghcid-switch-to-buffer`

Focus the running ghcid buffer for this project.

### `projectile-ghcid-stop`

Kill the running ghcid process for this project and close the buffer.