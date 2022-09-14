# ![logo](https://camo.githubusercontent.com/5bd79abbaf37dc6a3e74de00f39490e70476bdb09e67e60f65b8063c08b9eaee/68747470733a2f2f636f6d6d756e6974792e7472696e697479636f72652e6f72672f7075626c69632f7374796c655f696d616765732f315f7472696e697479636f72652e706e67) TrinityCore
## ARAC - All Races All Class

**基于 TrinityCore 魔兽世界 WotLK 3.3.5 全种族全职业补丁**



测试效果可进我的[公益服](https://wow.oolong.live/)

# ![ARAC icon](https://github.com/ZhxChen/mod-arac/blob/master/icons.png?raw=true)
## Description

    Download from release https://github.com/ZhxChen/mod-arac/releases/
    License: AGPL

## Screenshot

![All Races All Classes](https://github.com/ZhxChen/mod-arac/blob/master/images/screen01.jpg?raw=true)

![All Races All Classes](https://github.com/ZhxChen/mod-arac/blob/master/images/screen02.jpg?raw=true)


# Usage

- 在打PATCH之前备份好你的数据库，关闭auth和server服务。

- 下载PATCH包 [release](https://github.com/ZhxChen/mod-arac/releases)。

- 在world数据库下应用/PATCH/SERVER/SQL_DATA下的8个数据库补丁。

  ```mysql
  #进入数据库
  mysql -u 用户名 -p
  输入密码
  #进入world数据库
  use world;
  #执行补丁
  source /home/zhxchen/PATCH/SERVER/SQL_DATA/1 - player_classlevelstats.sql
  后续还有7个
  ```

- 将`/PATCH/SERVER/DBC_DATA`下的两个DBC文件覆盖至TrinityCore服务端`server/data/dbc/`目录下。

- 将`/PATCH/CLIENT`下的`Patch-A.MPQ`文件覆盖至  魔兽客户端根目录`Wow/Data/`  目录下（WOW为客户端根目录）。

- 重启auth和server服务。

  
