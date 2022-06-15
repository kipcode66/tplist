# tplist
Make an .lst file from the game's map.

## How to use
First, you need to extract the `.map` files from the game. This can easily be done through the Dolphin Emulator.

1. Make sure your dumped game is detected by Dolphin and appears in your game list.
2. Right click on the game and select `Properties` in the context menu.
3. Go to the tab `Filesystem`
4. Under `Disc`, right click on `map` and select `Extract Files...`, then choose where to save the extracted files.

Then you can run the `tplist.py` script to extract the symbols from the `.map` files like this:

```shell
python3 ./tplist.py ./assets/us.txt <path_to_your_map>/map/Final/Release output.lst
```

(Of course, replace `<path_to_your_map>` with the path to where you saved the extracted files.)

The provided `assets/xx.lst` files are example of a list of modules to extract. You can provide your own file which contains a list of the modules you want to extract the symbols from. (The provided lists will extract all symbols from every modules)

You can run `python3 ./tplist.py --help` for further help with the vailable options.