# vod-source

* 提供一些搜集于互联网的 VOD 资源站 / A list of VOD sources collected from internet

## JSON 格式 / JSON Format

* VOD 资源站 JSON 格式为一个字典的数组 / The VOD source JSON requires an array of dictionaries
* 每个字典**只能**包含下表所列的三个键 / The dictionary should contain **only** following three keys

键 / Key|必需性 / Requirement|备注 / Note
:-:|:-:|:-:
`name`|必需 / Required|
`api`|必需 / Required|格式为 / Format is `https://example.com/api.php/provide/vod/`
`note`|可选 / Optional|

## 在本仓库中加入你自己的 JSON / Put your own JSON in this repo

* 你可以创建自己的 VOD JSON 列表并放在这个仓库的 `public/` 文件夹下，以 `name.json` 命名。
* You can create your JSON file of vod source list, with file name `name.json`, under `public/` folder.
* **【仍在开发】** 在 CMSPlayer 中，当从 JSON 添加资源站时，可以输入自己创建的 VOD JSON 文件名称（`name`）来获取 JSON 文件，而不用完整复制整个 URL。
* **[TBD]** In CMSPlayer, you can simply type the name of the file (`name`) to fetch this JSON, instead of copying the whole URL into the app.

## 例子 / Example

```
[
    {
        "name": "海外看",
        "api": "https://haiwaikan.com/api.php/provide/vod/",
        "note": "需要代理"
    },
    ...
]
```
