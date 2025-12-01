From this directory, run the following commands.

## Disable the mouse in neovim and use relative line numbers

`cp ./.config/nvim/lua/config/options.lua ~/.config/nvim/lua/config/options.lua`

## Setup kanata

```
sudo yay -S kanata
sudo mkdir -p /etc/kanata; sudo cp ./etc/kanata/kanata.kbd /etc/kanata/kanata.kbd
sudo install -m 644 ./lib/systemd/system/kanata.service /lib/systemd/system/kanata.service
# sudo systemctl daemon-reload # maybe this will be required when changing the service file
sudo systemctl start kanata
sudo systemctl enable kanata
```

## Customize hyprland

`cp ./.config/hypr/bindings.conf ~/.config/hypr/bindings.conf`
`cp ./.config/hypr/looknfeel.conf ~/.config/hypr/looknfeel.conf`

## Bash

`cat ./.bashrc >> ~/.bashrc; source ~/.bashrc`

# TODO

- Setup a repeat key
- Customize symbol layer
