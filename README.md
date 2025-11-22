From this directory, run the following commands.

## Disable the mouse in neovim and use relative line numbers

`cat ./.config/nvim/lua/config/options.lua >> ~/.config/nvim/lua/config/options.lua`

## Setup keyd and home row mods

`sudo pacman -S keyd`

`sudo systemctl enable keyd`

`sudo cat ./etc/keyd/default.conf >> /etc/keyd/default.conf`

`sudo systemctl start keyd`

## Customize hyprland keybinds

`cat ./.config/hypr/bindings.conf >> ~/.config/hypr/bindings.conf`
