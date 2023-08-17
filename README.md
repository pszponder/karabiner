# Piotr's Karabiner Elements configuration

NOTE: This project has been cloned from @mxstbr's Karabiner Elements configuration

Watch the video from the original repo:

[![YouTube video by Max Stoiber explaining how and why to use this repo](https://img.youtube.com/vi/j4b_uQX3Vu0/0.jpg)](https://www.youtube.com/watch?v=j4b_uQX3Vu0)

## Installation

1. Install & start [Karabiner Elements](https://karabiner-elements.pqrs.org/)
1. Clone this repository
1. Delete the default `~/.config/karabiner` folder
1. Create a symlink with `ln -s ~/github/mxstbr/karabiner ~/.config` (where `~/github/mxstbr/karabiner` is your local path to where you cloned the repository)
1. [Restart karabiner_console_user_server](https://karabiner-elements.pqrs.org/docs/manual/misc/configuration-file-path/) with `` launchctl kickstart -k gui/`id -u`/org.pqrs.karabiner.karabiner_console_user_server ``

## Development

```
# install the dependencies. (one-time only)
pnpm install
```

```
# build the `karabiner.json` from the `rules.ts`.
pnpm build
```

```
# watch the TypeScript files and rebuild whenever they change.
pnpm watch
```
