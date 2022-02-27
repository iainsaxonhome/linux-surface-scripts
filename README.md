# linux-surface-scripts
Collection of scripts for Surface for Lubuntu

These packages were installed however some may not be needed for the final product:
```
sudo apt install onscreen
sudo apt install onboard
sudo apt install xrandr
sudo apt install florence
sudo apt install touchegg
sudo apt install touchegg-gui
sudo apt install touche
sudo apt install xinput
sudo apt install ionotify-tools
sudo apt install sensorfw
```

The scripts under`/opt/scripts` need to be owned by root, given execute permissions and then symlinked into the user's binary directory:
```
sudo chmod u+x /opt/scripts/autorotate
sudo chmod u+x /opt/scripts/rotatescreen

ln -s /opt/scripts/autorotate /usr/local/bin/autorotate
ln -s /opt/scripts/rotatescreen /usr/local/bin/rotatescreen
```

## Onboard settings

### General

(Activate all options)

### Window

#### Transparency

* Transparency
  * Window: 10
  * Background: 10 ([x] No Background)
* When Inactive
  * [x] set transparency to [50] after [1.0] seconds

### Layout

* Core layouts: Compact

### Theme

* High Contrast, Inverse

### Keyboard

#### Advanced

* Input Options
  * Touch input: single-touch
  * Input event source: XInput
* Key-stroke Generation
  * Delay between keystrokes in milliseconds: 1
  * Key-stroke generator: Auto

**Note**

Remember to install `menulibre` package to easily edit the menu.
