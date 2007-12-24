# War and Peace

An RTS made in GameMaker. Villager, swordsman, spearman and cavalry units plus hall and barracks buildings are split across two factions, and it comes with a map editor.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="420" alt="Title screen">
  <img src="docs/screenshots/screenshot-2.png" width="420" alt="Map editor">
</p>


## How to play

Download from Releases and run it.

On the title screen, Start asks for a saved `.mak` map file and starts the game on it, and Editor goes into the map editor.

In the editor, the buttons along the top pick units and buildings to place on screen, and the starting funds can be adjusted. A map is saved in two forms, one for editing and one for playing, and reopened with Load. The left and right arrow keys scroll the view.


## How it works

Map saving uses GameMaker's `game_save` as is. Rather than designing a file format for the coordinates and types of placed units, the whole game state is written out as a snapshot. The file dialog attaches a `.mak` extension so it looks like a map file. The map editor ran without a save format ever being designed.

Scrolling is a small dummy object moved with the left and right keys, with the view set to follow it.


## Files

| Path | Contents |
|---|---|
| `source/war-and-peace.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
