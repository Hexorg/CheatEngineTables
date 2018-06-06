Game Directory Format:
----------------------
To maintain consistency, only the game name is used for naming game directories.
 These are for improving end user ease of use improvements. Spaces are allowed 
since it makes searching for end users easier.

 1. Everything is lower case
 2. Drop [all of the following characters][1]: ```<,>,:,",/,\,|,?,*```
 3. Maintain congruency with the popular game name; meaning if the game uses
    VII instead of 7, then use vii. Use http://howlongtobeat.com as a naming
    guide if you are confused.
 4. If re-releases or newer versions of a game comes out, and it is **not**
    distinguishable from the original, include the year in parenthesis to
    distinguish the game, including the original game release, e.g.:

    ```
    deus ex (1997)
    deus ex (2013)
    ```
5.  If every table the game directory has been processed and verified, add a
    empty file to indicate as such:
    ```
    .verified-YYYY-MM-DD
    ```

Table Naming Format:
--------------------
Tables are named to convey game, game version, table version, attribution, and
platform the cheat table is for. Generally this follows the same naming
convention as [Game Directory Format](#game-directory-format):

> [game](#game)[_game-version](#game-version)[_os-platform](#os-platform)[_os-architecture](#os-architecture)[_graphics-api](#graphics-api)[_drm-platform](#drm-platform)[_table-version](#table-version)[_author](#author).ct
```
deus-ex-1997_1.005_pc_x86_steam_1_biskuts.ct
deus-ex-1997_1.005_pc_x86_steam_2_biskuts.ct
deus-ex-1997_2.03_linux_x86_steam_2_biskuts.ct
deus-ex-1997_2.03_gog_1_frenchfries.ct
```

game:
=====
The name of the game.
1. The game name should be the same as the game directory, but using dashes '-' 
   instead of spaces for table.
2. Parens are dropped: ```(,)```

game-version:
=============
The version of the game this table is for.
1. Drop any shorthand version labeling, e.g.: version, v, etc.
2. Lowercase all letters

os-platform:
============
What OS this table is for.
1. If the game is only on one platform, leave this section out.

    |os-platform|Description                          |
    |-----------|-------------------------------------|
    |win        |Windows                              |
    |osx        |Mac OSX                              |
    |linux      |Linux                                |
    |psx        |Playstation (or playstation emulator)|
    |n64        |Nintendo 64 (or emulator)            |

os-architecture:
================
What architecture this ct is for.
1. If the game is only released in one architecture, leave this section out.
```
x86
x64
arm
```

graphics-api:
=============
The graphics API used for this ct.
1. If the game does not depends on a specific graphics API, leave this section
   out.
2. If directX, use [the version listed on the wiki][8]
3. If only the major version of directX is known, just use that.

```
dx9
...
dx10
dx10.1
...
dx12
opengl
```

drm-platform:
==============
The platform that this specific table is for.
1. If it works on any platform, leave this section out.
2. Use the common name for the DRM platform the game is installed from, search
   before creating a new one. (e.g. A uplay game that is bought on Steam uses 
   Steam DRM, not Uplay's, and should be labeled as ```_steam```)

    |Common Name|Platform                |
    |-----------|------------------------|
    |steam      |[Steam][1]              |
    |gog        |[GOG][2]                |
    |uplay      |[U-play][3]             |
    |origin     |[Origin][4]             |
    |gmg        |[Green Man Gaming][5]   |
    |itch       |[itch.io][6]            |
    |flash      |Shockwave Flash         |
    |browser    |Browser based, non-flash|

table-version:
=============
The version of the table.
1. Drop any shorthand version labeling, e.g.: version, v, etc.
2. Lowercase all letters

author:
=======
The author of the table.
1. Lowercase all letters
2. Links and additional attribution in the README.md for the game.

[1]: https://msdn.microsoft.com/en-us/library/aa365247(VS.85).aspx
[2]: http://www.steampowered.com
[3]: http://www.gog.com
[4]: http://www.uplay.com
[5]: http://www.origin.com
[6]: http://www.greenmangaming.com
[7]: http://www.itch.io
[8]: https://en.wikipedia.org/wiki/DirectX#Release_history
