# Assetto Corsa Linux Setup
A shell script based on [this](https://steamcommunity.com/sharedfiles/filedetails/?id=2828364666) guide. Works on most modern systems.

## What it does
- Installs [Proton-GE](https://github.com/GloriousEggroll/proton-ge-custom)
- Installs [Content Manager](https://assettocorsa.club/content-manager.html) and everything else required for it to work
- Adds Content Manager to mimeapps.list (allows opening `acmanager://` race invite links)
- Installs [Custom Shaders Patch (CSP) preview](https://acstuff.club/patch/), [PURE weather mod](https://www.patreon.com/peterboese), and SKY pp filter from zip files in `Downloads`
- Installs [DXVK](https://github.com/doitsujin/dxvk)

After running the script you should be able to launch Assetto Corsa from Steam with no issues (it will launch Content Manager). The original launcher is preserved as `AssettoCorsa_original.exe`.

## Instructions
1. Download Assetto Corsa on Steam.
2. Put `CSP*.zip`, `PURE*.zip`, and `SKY*.zip` in your `Downloads` directory.
3. Inside the terminal, run
  ```
  curl -Os https://raw.githubusercontent.com/cast-racing/assettocorsa-linux-setup/main/assettocorsa-linux-setup.sh && bash assettocorsa-linux-setup.sh
  ```
> **Warning**: Always be careful when running scripts from the internet.
4. Follow every step in the console (y - stands for yes, n - stands for no).
5. Launch Assetto Corsa from Steam (it might take a while on the first run, be patient).
6. In Content Manager set the Assetto Corsa root folder to `Z:\path\to\Steam\steamapps\common\assettocorsa`.
7. In Content Manager, go to `Settings -> Content Manager -> Appearace` and check "Disable windows transparency" (fixes the full-black tooltips, pop-ups and dialogues).
8. Enjoy!