# pwnagotchi-plugins

For custom plugins to work, you have to add the path to your folder in the `config.toml`.

```toml
main.custom_plugin_repos = [
  "https://github.com/evilsocket/pwnagotchi-plugins-contrib/archive/master.zip",
  "https://github.com/dotzero/pwnagotchi-plugins/archive/master.zip",
]
```

Then run this command: `sudo pwnagotchi plugins update`

## Plugins

### age.py

```toml
main.plugins.age.enabled = true
main.plugins.age.age_x_coord = 0
main.plugins.age.age_y_coord = 32
main.plugins.age.str_x_coord = 67
main.plugins.age.str_y_coord = 32
```

### exp.py

```toml
main.plugins.exp.enabled = true
main.plugins.exp.lvl_x_coord = 0
main.plugins.exp.lvl_y_coord = 81
main.plugins.exp.exp_x_coord = 38
main.plugins.exp.exp_y_coord = 81
main.plugins.exp.bar_symbols_count = 12
```

### wavesharebattery.py

```bash
sudo apt-get install python-smbus
sudo raspi-config nonint do_i2c 0
```

```toml
main.plugins.wavesharebattery.enabled = true
```
