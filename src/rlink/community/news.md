# [GET] /community/news/getNews

[Example request](https://aoe-api.worldsedgelink.com/community/news/getNews?title=age2)

Returns in-game news entries for the specified title. Each news
item includes a headline image text, body content, and metadata
about visibility and expiration.

## Request

| Parameter | Type     | Value                  | Comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |

## Response

### AoE2:DE

The `news` array contains all active news entries. Entries are
returned in descending order by `id`.

```json
{
    "result": {
        "code": 0,
        "message": "SUCCESS"
    },
    "news": [
        {
            "id": 822,
            "hidden": 0,
            "newscategory": "(01/17) 56 en",
            "newstitle_locstringid": -1,
            "newssubtitle_locstringid": -1,
            "newstext_locstringid": -1,
            "newsimage": "Red Bull Wololo: Legacy Tournament October 21 - 30",
            "newsbody": "To battle! Red Bull Wololo is back...",
            "metadata": "NEWS;id=56;lang=en",
            "datevisible": 1666386000,
            "expirytime": 1667196000
        },
        {
            "id": 1,
            "hidden": 0,
            "newscategory": "",
            "newstitle_locstringid": 1,
            "newssubtitle_locstringid": -1,
            "newstext_locstringid": 2,
            "newsimage": "Welcome to Age of Empires II: Definitive Edition!",
            "newsbody": "Welcome to Age of Empires II: Definitive Edition!...",
            "metadata": "LNEWS",
            "datevisible": 1573660800,
            "expirytime": 1763064000
        }
    ]
}
```

| Field                    | Type   | Description                                                                                |
| ------------------------ | ------ | ------------------------------------------------------------------------------------------ |
| id                       | int    | Unique news entry identifier                                                               |
| hidden                   | int    | Whether the entry is hidden (`0` = visible)                                                |
| newscategory             | string | Display ordering hint, e.g. `(01/17) 56 en`                                                |
| newstitle_locstringid    | int    | Localized string ID for the title (`-1` when the raw `newsimage` field is used instead)    |
| newssubtitle_locstringid | int    | Localized string ID for the subtitle (`-1` if unused)                                      |
| newstext_locstringid     | int    | Localized string ID for the body text (`-1` when the raw `newsbody` field is used instead) |
| newsimage                | string | Headline / image caption text                                                              |
| newsbody                 | string | Full news body content                                                                     |
| metadata                 | string | Categorization tag (see note below)                                                        |
| datevisible              | int    | Unix timestamp when the entry becomes visible                                              |
| expirytime               | int    | Unix timestamp when the entry expires                                                      |

> **Note:** News entries are returned in multiple languages.
> The `metadata` field encodes the news ID and language with
> the pattern `NEWS;id=<news_id>;lang=<lang_code>` (e.g.
> `NEWS;id=56;lang=en`). A single piece of news with
> `id=56` can appear as 17 separate entries -- one per
> supported language (`en`, `zh`, `tw`, `fr`, `de`, `hi`,
> `it`, `jp`, `ko`, `ms`, `br`, `ru`, `es`, `mx`, `tr`,
> `vi`, `pl`). Older entries may use a simpler format such
> as `LNEWS` or `LNEWS;PROMOTION=DLC_PORTO;`.
