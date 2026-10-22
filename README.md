# NekoBox DDNet 地图库

NekoBox 双模式服（Gores + DDRace）使用的 DDNet 地图文件。

## 内容

| 项 | 数量 |
|---|---|
| `.map` 地图文件 | 3785 |
| `license.txt` | 地图作者署名与许可 |
| `nekobox-maps.tsv` | 地图元信息（名称 / 模式 / 星级 / 分数 / 作者 / 发布日期） |

## 用法

游戏服把本仓库的 `.map` 文件放进 `data/maps/` 即可：

```bash
git clone --depth 1 https://github.com/cookieidea/ddnet-maps.git
cp ddnet-maps/*.map /path/to/server/data/maps/
```

或直接作为子目录挂载 / 软链。

## 地图元信息

`nekobox-maps.tsv` 是制表符分隔，字段顺序：

```
名称	模式	星级	分数	作者	发布日期
```

- 模式：`0` = Gores，`1` = DDRace
- 星级：`0`–`5`
- 分数：完成该图获得的积分
- 作者 / 发布日期可能为空

权威数据在服务器数据库的 `record_maps` 表，本文件是导出快照。

## 许可

各张地图的版权与许可归原作者所有，具体见 `license.txt`。
本仓库仅为分发与备份用途。

## 地图来源

收集自 DDNet 社区、KoG (King of Gores)、Axiom、0XF、EGO (Eternal Gores) 等公开地图库。
