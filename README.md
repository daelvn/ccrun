# ccrun

**WARNING: This project has been replaced by [ccrunx](//github.com/daelvn/ccrunx). This project is deprecated.**

`ccrun` is a wrapper for [CCEmuX](https://github.com/CCEmuX/CCEmuX), a ComputerCraft Emulator. This shell script lets you pass a directory and execute the whole project in a ComputerCraft environment, without having to configure CCEmuX or copy the files manually.
## Installing
This should be as easy as cloning this repo (`git clone https://github.com/daelvn/ccrun.git`), making the script an executable if it isn't already (`chmod +x ./ccrun`) and running it. It's recommendable that you put this script in your path.
If you need to install CCEmuX, you can easily download it from the AUR as `ccemux-git` (Arch).
## Usage
For the first time, `ccrun` needs to create CCEmuX's data directory. For that, you can run `ccrun -i` or `ccrun --install`. CCEmuX will start automatically but you can close it as soon as it's open. Then, your preferred editor (or one specified with the `-e/--editor` flag) will open the configuration file for you to tweak whatever is necessary. You can uninstall `ccrun` at any moment with `ccrun -u` or `ccrun --uninstall`.
### First-run
The basic syntax for `ccrun` is `ccrun <folder>`, but if you are running `ccrun` just after using the install flag, you should use `-a` (Asks you to create folders that don't exist) so that you can create the data directory for the computer ID automatically. If you don't want to do it even for the first time, you can just create it manually. After doing this once it's not necessary anymore.
### Specifying another configuration
You can specify another configuration folder with the `-c` or `--config` flag, as well as another computer ID with `-d` or `--id`. The full list of possibilities is listed with `--help`.
## Credits
Thanks to all the collaborators at [CCEmuX](https://github.com/CCEmuX) for the amazing emulator.
## License
This project is released to the public domain.
