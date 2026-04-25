New-Super-Virtual-Chest
由CEBCTADET开发的用于Minecraft Java Edition的Mod,支持Farbic1.21.10-1.21.11  Quilt1.21.10-1.21.11

此Mod所有者，开发者为CEBCTADET，我仅是帮他将此Mod上传至GitHub

此Mod也在Modrinth上（正在审核中）

📦 特色

🗃️ 虚拟宝箱——创建不绑定任何物理方块的宝箱。

🌍 公开与私人——创建一个任何人都可以打开的公开宝箱。使用玩家名创建一个只有该玩家（和管理员）能访问的私人宝箱。

⏳ 延迟公开删除——当非管理员删除公开宝箱时，该宝箱会进入3个游戏日的等待期，之后才会被永久移除。在此期间任何人都可以取消删除。

✅ 即时管理员操作——拥有标签（或控制台/命令块）的玩家可以创建、打开并瞬间删除任何宝箱。

💾 持久存储——所有宝箱内容都会保存到世界文件夹内的磁盘中，并且能在服务器重启时保存。

🌐 多语言支持——包括英语和简体中文。（显示哪种语言由您的客户端语言决定。）

🖥️ 纯服务器端——无需客户端模组！玩家连接原版客户端，仍能看到正常的宝箱界面。

⌨️ 指挥
所有命令都使用前缀:/NSvc

📝 创建宝箱
/NSvc <target> create <name> [small|large]    <target>—— 对公开宝箱来说，或者作为在线玩家对私人宝箱的玩家名。   <name>– 箱子的唯一名称（例如，）:community_farm        [size]–（27个槽位）或（54个槽位）默认为 :small large large
      示例： /NSvc allplayer create PublicStorage large /NSvc Steve create StevePrivate small

📂 打开一个箱子
/NSvc <target> open <name> 打开虚拟宝箱GUI

非管理员玩家只能打开公共宝箱或自己的私人宝箱。

示例： /NSvc allplayer open PublicStorage

🗑️ 删除宝箱
/NSvc <target> delete <name> [close]

无——开始删除（公共宝箱需等待3天;私人宝箱需确认）   close
与 – 取消待删除   close
示例： /NSvc allplayer delete PublicStorage    /NSvc allplayer delete PublicStorage close

📋 列表宝箱
/NSvc <target> list

显示目标所有宝箱（公开宝箱，私人宝箱需玩家姓名）。
管理员能看到所有私人宝箱;普通玩家只看到自己的宝箱。allplayer

🛡️ 管理员权限
该模组不使用单独的权限文件。
管理员通过nsvc_admin标签标识。

🏷️ 资助管理
在服务器控制台或现有管理员中执行以下命令：/tag <player> add nsvc_admin

❌ 移除管理员
/tag <player> remove nsvc_admin

👀 检查玩家标签
/tag <player> list

💡 提示：控制台和命令方块始终拥有完整的管理员权限，不需要标签。

📁 数据存储
虚拟宝箱数据保存在世界文件夹中。
该文件自动创建，兼容世界备份。   nsvc_virtualchests.dat

🌍 语言支持
模组会自动使用你的Minecraft客户端语言。
目前支持的语言：

英文 （en_us)
简体中文（zh_cn)
