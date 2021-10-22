# naptime

This is the tiniest possible way I can find to run node / yarn / webpack in a container instead of installing it in my workspace.


## Usage

1. Put the `naptime` script in your path.
1. Run `naptime <command>` to run `<command>` in the naptime container (where node, yarn & webpack are available).

Note that local node modules required by your package.lock are installed to `~/.local/<project>` instead of `./node_modules/` in your working directory. This is more like other tools like pipx that manage those environments for you.
