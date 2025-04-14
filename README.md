SourceMod
=========

基于 https://github.com/alliedmodders/sourcemod/commits/1.12-dev/ `08ad11981225258a14135b9ed8dd8f4eca7957fc`Commits on Mar 24, 2025 版本修改

目前大部分功能都不可用，请重新找sdktool等偏移
如果你打算修复偏移，请记得将[这个位置](https://github.com/RightNowMod/sourcemod-1.12/commit/3902f76c90a677b329ceffbbf4ecf1314052156b#diff-9581e73ae24e6ca5b23f6bc8c051cafb01fa52cdc54aec74a356b9908f45af4cR1164)的return给注释掉。当前源码能正常运行均靠这个return，否则会出现段错误。可能是偏移问题导致所有与实体相关的函数都无法使用

当前版本仅可以使用：
1. css的部分事件，如回合结束等。目前已知游戏开始事件和玩家断开连接事件无法使用
2. 获取server.cfg里的参数值，这里获取的值后面会跟着随机脏数据，暂未修复
3. 获取游戏的一些变量，如地图名称，人数，玩家名称等
4. MySQL功能正常

可以参考[这个脚本](https://github.com/RightNowMod/CS-MOS-overtime-fix/blob/main/CSMOS-overtime-fix.sp)，目前仅用于记录比赛的统计数据，无法修改玩法，丧尸模式什么的无法使用

无法使用的功能：
1. 所有和实体相关的功能，如给予武器，增加子弹，设置玩家各种属性，优化插件，改变游戏模式和玩法等
2. 其它未提及的大部分功能



General
-------
- [SourceMod website](http://www.sourcemod.net): Source Engine scripting and server administration
- [Forum](https://forums.alliedmods.net/forumdisplay.php?f=52): Discussion forum including plugin/extension development
- [General documentation](https://wiki.alliedmods.net/Category:SourceMod_Documentation): Miscellaneous information about SourceMod
- [Stable builds](http://www.sourcemod.net/downloads.php?branch=stable): The latest stable SourceMod releases
- [Dev builds](http://www.sourcemod.net/downloads.php?branch=dev): Builds of recent development versions
 
Development
-----------
- [Issue tracker](https://github.com/alliedmodders/sourcemod/issues): Issues that require back and forth communication
- [Building SourceMod](https://wiki.alliedmods.net/Building_SourceMod): Instructions on how to build SourceMod itself using [AMBuild](https://github.com/alliedmodders/ambuild)
- [SourcePawn scripting](https://wiki.alliedmods.net/Category:SourceMod_Scripting): SourcePawn examples and introduction to the language
- [SourceMod plugin API](https://sm.alliedmods.net/new-api): Online SourceMod plugin API reference generated from the include files
- [SourceMod extension development](https://wiki.alliedmods.net/Category:SourceMod_Development): C++ examples and introduction to various extension interfaces
- [Translation project](https://github.com/orgs/alliedmodders/projects/1): Help [translate SourceMod](https://wiki.alliedmods.net/Translations_(SourceMod_Scripting)) into your language

Contact
-------
- Connect with us on [GameSurge](https://gamesurge.net) IRC in #sourcemod
- Alternatively feel free to join our [Discord](https://discord.gg/HgZctSS) server

License
-------
SourceMod is licensed under the GNU General Public License version 3. Special exceptions are outlined in the LICENSE.txt file inside of the licenses folder.
