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
