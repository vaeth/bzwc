# bzwc

(C) Martin Väth <martin at mvath.de>
This project is under the BSD license 2.0 (“3-clause BSD license”).
SPDX-License-Identifier: BSD-3-Clause

A POSIX shell wrapper for `wc` supporting compressed files
- `.xz`
- `.lzma`
- `.br`
- `.bz2`
- `.zst`
- `.gz`

All options of `wc` can be used, and as for usual `wc`,
it is possible to pass several files as arguments.

For standard input, the name of the command
- `xzwc`
- `lzwc`
- `brwc`
- `bzwc`
- `zstdwc`
- `zwc

determines which type of compressed data is assumed.

### Requirement

You need `push.sh` from https://github.com/vaeth/push (v2.0 or newer)
in your `$PATH`.

### Installation

For installation, copy the content of `bin/` with executable permission
in your `$PATH`. To obtain support for __zsh completion, you can copy the
content of `zsh/` to a directory of your zsh's `$fpath`.

For Gentoo, there is an ebuild in the mv overlay (available over layman).
