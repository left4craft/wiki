# Old worlds

So you can continue to enjoy your builds long after we update and reset, we make previous worlds available to download for as long as possible.


## Downloads

| World                                  | Seed                   | Spawn location    | Compressed size | Links                                                                                                                  |
| -------------------------------------- | ---------------------- | ----------------- | --------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Survival 1.13 - 1.15 (`world`)         | `-3417273309160634301` | `-1215, 149, 609` | 21.2 GB         | [Compressed](https://l4c.link/13-15-survival-zip), [Uncompressed](https://l4c.link/13-15-survival-files)               |
| Creative *long ago* - 1.15             | --                     | --                | --              | `/warp oldcreative`                                                                                                    |
| Survival 1.16 - 1.17 (`world`)         | `911358417907257`      | `777, 96, -334`   | 28.8 GB         | [Compressed](https://l4c.link/16-17-survival-zip), [Uncompressed](https://l4c.link/16-17-survival-files)               |
| Survival 1.16 - 1.17 (`world_nether`)  | --                     | --                | 3.9 GB          | [Compressed](https://l4c.link/16-17-survival-nether-zip), [Uncompressed](https://l4c.link/16-17-survival-nether-files) |
| Survival 1.16 - 1.17 (`world_the_end`) | --                     | --                | 3.4 GB          | [Compressed](https://l4c.link/16-17-survival-end-zip), [Uncompressed](https://l4c.link/16-17-survival-end-files)       |
| Survival 1.18 (`world`)                | `-796373454075539119`  | `1087, 93, -509`  | 17.5 GB         | [Compressed](https://l4c.link/18-survival-zip), [Uncompressed](https://l4c.link/18-survival-files)                     |
| Survival 1.18 (`world_nether`)         | --                     | --                | 2.2 GB          | [Compressed](https://l4c.link/18-survival-nether-zip), [Uncompressed](https://l4c.link/18-survival-nether-files)       |
| Survival 1.18 (`world_the_end`)        | --                     | --                | 1.0 GB          | [Compressed](https://l4c.link/18-survival-end-zip), [Uncompressed](https://l4c.link/18-survival-end-files)             |

Other downloads are available at [left4craft.download](https://left4craft.download/).

The "Compressed" links are ZIP files containing the entire world, whilst "Uncompressed" links go to a page where you can [download specific files](#how-to-download-specific-chunks). 

## How to download specific chunks

The worlds can be over 20GB in size which may be too large for some players to be able to download or save. This guide explains how to download your own builds without everyone else's.


1. Use [this tool](https://web.archive.org/web/20221129042222/https://dinnerbone.com/minecraft/tools/coordinates/) to find the region names
2. Click on the "Uncompressed" link for the world
3. Select and download all of the MCA region files you need from `region/` and `entities/`
4. Optionally, download the `advancements/`, `playerdata/`, and `stats/` files with your UUID in the file name
5. Launch Minecraft (with the version that the world was originally made for) and create a new world using the seed from the table above
6. Move the previously downloaded files into your new local world [save folder](https://www.howtogeek.com/207484/how-to-find-your-minecraft-saved-games-folder/)

## Merging The Nether and The End

If The Nether and The End are also available, you can merge them into the main save folder.

Either:

- Download and decompress the entire world (called `world_nether` or `world_the_end`) using the "Compressed" link
- Use the "Uncompressed" link, navigate to `DIM-1/` for The Nether or `DIM1/` for The End, and download specific files from `region/` and `entities/` as described above 

Then, move the downloaded files into the `DIM-1/` (The Nether) and `DIM1/` (The End) folders inside the main save folder

You should now have a directory tree that looks like this:

```
world
|- advancements
|- data
|- datapacks
|- DIM1
|  |- data
|  |- entities
|  |- poi
|  |- region
|- DIM-1
|  |- data
|  |- entities
|  |- poi
|  |- region
|- entities
|- playerdata
|- poi
|- region
|- stats
```
