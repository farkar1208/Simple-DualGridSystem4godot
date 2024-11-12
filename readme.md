# 打倒双网格系统！OVERTHROW Dual-Grid Sysdem!

为了替代费时费力的47瓦片集和需要大量代码且代码量随地形种类的增加指数上涨的双网格系统，靴靴（我）提出了用godot的地形集（匹配角）简便地实现只需16瓦片且每格地类型归属明确的方案，并将用到的脚本上传于此。
In order to replace the time-consuming and labor-intensive 47 tile set and the dual grid system that requires a large amount of code and the code volume increases exponentially with the increase of terrain types, XueXue (me) proposes a simple solution using Godot's terrain set (matching corners) that only requires 16 tiles and clearly defines the type of terrain in each grid, and uploads the scripts used here. 
## 原理schematic：
我们发现，godot的自动瓦片（地形）匹配不是依据周围九宫格的地形确定采用的瓦片，而是根据周围八格地形接壤部分的类型和自身类型决定。
因此我们可以采用匹配角的地形集，将四角的地形设置为对应地形，将中间地形设置为与左上角相同（你也可以设置成其它角，但这个项目中统一采用设置为左上角的方案）
这样，当你更改一格的地形时，向左上偏移半个瓦片的方块将改变为对应的地形。也就是说，每格方块的类型由向右下偏移半个瓦片的瓦片地形类型决定。
鄙人英文和中文都不好，翻译是机翻，见谅。
We discovered that Godot's automatic tile (terrain) matching does not determine the tiles to be used based on the terrain of the surrounding nine-grid, but rather on the type of terrain bordering the surrounding eight-grid and its own type. 
Therefore, we can adopt the terrain set that matches the corners, set the terrain of the four corners to the corresponding terrain, and set the terrain in the middle to be the same as the upper left corner (you can also set it to other corners, but in this project, we uniformly adopt the scheme of setting it to the upper left corner) 
In this way, when you change the terrain of a square, the block shifted half a tile to the upper left will change to the corresponding terrain. That is to say, the type of each square is determined by the terrain type of the tile shifted half a tile to the lower right. 
Both my English and Chinese are not very good, and the translation is done by machine translation, please forgive me. 
