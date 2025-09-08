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
[main.plugins.age]
enabled = true
age_x_coord = 0
age_y_coord = 32
str_x_coord = 67
str_y_coord = 32
```

### exp.py

```toml
[main.plugins.exp]
enabled = true
lvl_x_coord = 0
lvl_y_coord = 81
exp_x_coord = 38
exp_y_coord = 81
bar_symbols_count = 12
```

### pwnachu-exp.py

```toml
[main.plugins.pwnachu-exp]
enabled = true
lvl_x_coord = 0
lvl_y_coord = 81
exp_x_coord = 32
exp_y_coord = 81
bar_symbols_count = 12

```

### pwnachu-theme.toml

```toml
[main.plugins.pwnachu-theme]
enabled = true
```

### wavesharebattery.py

```bash
sudo apt-get install python-smbus
sudo raspi-config nonint do_i2c 0
```

```toml
[main.plugins.wavesharebattery]
enabled = true
```
