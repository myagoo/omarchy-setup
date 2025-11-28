From this directory, run the following commands.

## Disable the mouse in neovim and use relative line numbers

`cat ./.config/nvim/lua/config/options.lua >> ~/.config/nvim/lua/config/options.lua`

## Setup keyd and home row mods

`sudo yay -S keyd`

`sudo systemctl enable keyd`

`sudo cat ./etc/keyd/default.conf >> /etc/keyd/default.conf`

`sudo systemctl start keyd`

## Setup kanata

```
sudo yay -S kanata
sudo cp -r --parents ./etc/kanata/ /
sudo install -m 644 ./lib/systemd/system/kanata.service /lib/systemd/system/kanata.service
# sudo systemctl daemon-reload # maybe this will be required when changing the service file
sudo systemctl start kanata
sudo systemctl enable kanata
```

## Customize hyprland keybinds

`cat ./.config/hypr/bindings.conf >> ~/.config/hypr/bindings.conf`
