# vod-source

A collection of VOD sources.

## JSON Format

* The VOD source JSON requires an array of dictionaries.
* The dictionary should contain **only** following three keys.

Key|Requirement|Note
:-:|:-:|:-:
`name`|Required|
`api`|Required|Format is `https://example.com/api.php/provide/vod/`
`note`|Optional|

## Put your own JSON in this repo

* You can create your JSON file of vod source list, with file name `name.json`, under `public/` folder.
* **TBD** In CMSPlayer, you can simply type the name of the file (`name`) to fetch this JSON, instead of copying the whole URL into the app.

## Example

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
