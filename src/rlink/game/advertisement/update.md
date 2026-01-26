# [POST] /game/advertisement/update

**AUTHENTICATION**

## AoE2:DE

### Request

```
POST /game/advertisement/update HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Content-Length: 1660
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
Expect: 100-continue

advertisementid=1&appbinarychecksum=4141&automatchPoll_id=-1&callNum=123&connect_id=ccc&datachecksum=-777&description=SESSION_MATCH_KEY&hostid=1&isObservable=1&lastCallTime=111&mapname=no_map&matchtype=19&maxplayers=8&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&observerDelay=180&observerPassword=&options=opts&password=&passworded=0&sessionID=zzz&slotinfo=slot&state=-1&versionFlags=0&visible=0
```

| parameter         | type      | value             | comments |
| ----------------- | --------- | ----------------- | -------- |
| advertisementid   | int       | -1                |          |
| appBinaryChecksum | int       | 4141              |          |
| automatchPoll_id  | int       | -1                |          |
| callNum           | int       | 123               |          |
| connect_id        |           |                   |          |
| dataChecksum      | int       | -777              |          |
| description       | str       | SESSION_MATCH_KEY |          |
| hostid            | int       | 1                 |          |
| isObservable      | int       | 1                 |          |
| lastCallTime      | timestamp | 111               |          |
| mapname           | str       | no_map            |          |
| matchtype         | int       | 19                |          |
| maxplayers        | int       | 8                 |          |
| moddllchecksum    | str       | 0                 |          |
| moddllfile        |           |                   | INVALID  |
| modname           |           |                   | INVALID  |
| modversion        |           |                   | INVALID  |
| observerDelay     | int       | 180               |          |
| observerPassword  | ?         | None              |          |
| options           | ?         | opts              |          |
| password          | ?         | None              |          |
| passworded        | int/bool  | 0                 |          |
| sessionID         | str       |                   |          |
| slotinfo          | ?         | slot              |          |
| state             | int       | -1                |          |
| versionFlags      | int       | 0                 |          |
| visible           | int       | 0                 |          |

### Response

```
[
    0,
    [
        186430525,
        109775243524512500,
        "0",
        233334,
        0,
        "TEST",
        "TEST",
        0,
        "my map",
        "eNpFUs2OgyAQfpc+gVQl6aEHGmxDUiC2mK17rGncxW7tZaPy9Dsw4HqaOPP9zDdsLn3N4NtKOzo2QcUZlSz+c+/fgy/54LSVE/YrekdMofm7xH+CyjpizDgdfMXbSVtW+VIbBhjpSwL/7r5QRtLrUD6vp51oPoi73J7kvOxeHfmqH7fj7dNlO+RuqZqagAWPuYx+lQFvQaffalsdUaelZ1OhJu/oAz3l2nYEufq0G1Fu9bnVryFglPWY4LNM3qXxeQT9GXab5RTwpeKAD9n0RH9nc6yzUCNvAb4i70BV9CL5SLDfzcm3cpCfYUfUk1SZpF1DrqitDOzOWqwt+LBNnOlS9rPmY4HcFfivBHJLzz1JHjntet/F74O+xaJtG/MQcGuBXmxNlWUn5AEvRpA4D3cUaX7NX0J+yoqoA1ljVjl4Lw59mC09Luq7/xt06w20Eel9Oc3Xfq5/CswSbhzxGbyHBfvDvPZdn/C5Nu8S+02xvkXu32IX3i/sX0IuUaNf/mdkujkBjue93+83f9Wl8QA=",
        0,
        8,
        "eNrVkVtPgzAYhv0tvQZDAWdC4g2MKkYWQShuxosKJes4BlBHFv+7K2ZTMhNDlsxw9R3b783zQll42oCyKmKWUiuPi3MWAU1W1ImiCqBuSMOK3JoCDQqgoSTjqSSAmIS7wbaqSEj3aZ7c0Tea7iubNOHSa8tuQ+TfsIze0wpVJKP2Q7fHapeSqO2u8JuvddfOaEOmpCFAA1Zyq7s+0h0fqU4Q8Wh6HtL9rufqTtLNZtSEPBoYJS3O8SIwy/f5ChkhTOcv1+sVkdcwSKJgZiJ3u6e7JkQ8Onhxg7Ml833M3+u2YV2BD+EQjQh7WMQfXGCPC5/swHzlR5GRvsnAHpmhKuUTqZT/9M9/LA/8I4P9S3/3jw33TzkRGeko/9RRqLwYhcrJKFRe/pPK57NPLoDn9g==",
        0,
        [
            [
                186430525,
                233334,
                -1,
                33833,
                -1,
                -1,
                "/10.0.11.21"
            ]
        ],
        0,
        512,
        0,
        0,
        1,
        0,
        null,
        "westeurope",
        null
    ]
]
```

## AoE4

### Request

```
POST /game/advertisement/update HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Length: 1668
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
Expect: 100-continue

advertisementid=50865084&appbinarychecksum=24916&automatchPoll_id=-1&callNum=274&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&datachecksum=-638535971&description=SESSION_MATCH_KEY&hostid=233334&isObservable=1&lastCallTime=3026321&mapname=no_map&matchtype=19&maxplayers=8&moddllchecksum=0&moddllfile=INVALID&modname=INVALID&modversion=INVALID&observerDelay=180&observerPassword=&options=eNp1jtEKgjAUhnuWXS9wkpZeVhRRQqB0ExJDD7Vym7hZiPjubSuoi7o85/++/5we8RNtteRUF5eE1gfQEhSKjzk2iYIKCs2kQHFvRgdlXQ2rip4N5FnmwcRCipJZzImD3V4lE1AmVkhBKZNtligeE/x9L9W00Rnj8K5qqLhBSe7EfVHuaCdbvZ+vt9DZZhL50SzCxJ9OIg/7XhiQMMg/YgaUq9+qo1rx4v4gw+gJPtNd0w==&password=&passworded=0&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&slotinfo=eNrtU02PmzAQ7W/hnFR8LOl6pT0sWZmAErIhfFc92IYIgyEoEBJS9b/XkDS7TbXqqZdqTx7PG888v5mR5NHX70K1224oS4xys/1MY+FBVu4myt1IqBvU0G1pPAsP0khoElT0pjgSNoj8Avhth0jSm7KoAEWWekeZz5M2YRe4zBeoIanTVUPcuE9Gi+Ql2cEdKpLFeoijtZ2guBvsvvK+HswiadAzapDwICSd2QQy29sybKK1MVlMDxR7oMJlxHBpt6Rk68iHefKKHbAO1Sgwb/1d6Ks5liUn1mEXQ60lMhORD/ZGtj3Op7yOYolhYHKfWro6OKHArrB8R5dUPOOy1EZQS0O5eSGzHlNPRlZ9MYqrv7/jIBBr7ttgH+SuDjMkRnXoxxzbHm7ynFzFTuOZd363HnimyNMYKa0WF7DmHFT+jhr0grnHNvTtNg5WdJmtuqWzUq2M8NMdaoYyOGHf43+wbjluiA65brYTyinjMaY9NSYXfXNeQ1xkubh0QoWf0lkPWyW6y+to4HzXUq6N6M7MCvuw67U16H077+7b+CSCC8dD6LN9DC3Guewj/W9xdod8kWtsDPhcIeBlbdRv+LrR0JN381CuRxl5Gs8jpaTMb3KZF+42C31Jw/qx4nOQ9bNk5J4TilBbOddcKSkkdeXz/+n9bPzelx7zAq0kBcyjYEGXrInP/YQdDpiHCyaSzpj40rn/kQ6WWLHXl7mrkqLX8mnAUGBxv8XcAnKNQINnzIn8Iws5z2h6ndltGFhTrIMMyV7uufHzdYYUrQ4DxkjO50QHEqHGZO6Y4Onp8VH4MfpzwfsNfLPc43e3eyy9rvf4H272B8sPlh8s/3eW3z79BF44tSI=&state=0&versionFlags=0&visible=0
```

| parameter         | type      | value             | comments |
| ----------------- | --------- | ----------------- | -------- |
| advertisementid   | int       | -1                |          |
| appBinaryChecksum | int       | 4141              |          |
| automatchPoll_id  | int       | -1                |          |
| callNum           | int       | 123               |          |
| connect_id        |           |                   |          |
| dataChecksum      | int       | -777              |          |
| description       | str       | SESSION_MATCH_KEY |          |
| hostid            | int       | 1                 |          |
| isObservable      | int       | 1                 |          |
| lastCallTime      | timestamp | 111               |          |
| mapname           | str       | no_map            |          |
| matchtype         | int       | 19                |          |
| maxplayers        | int       | 8                 |          |
| moddllchecksum    | str       | 0                 |          |
| moddllfile        |           |                   | INVALID  |
| modname           |           |                   | INVALID  |
| modversion        |           |                   | INVALID  |
| observerDelay     | int       | 180               |          |
| observerPassword  | str       |                   |          |
| options           | str       | opts              |          |
| password          | str       |                   |          |
| passworded        | int/bool  | 0                 |          |
| sessionID         | str       |                   |          |
| slotinfo          | ?         | slot              |          |
| state             | int       | 0                 |          |
| versionFlags      | int       | 0                 |          |
| visible           | int       | 0                 |          |

### Response

```
[
    0,
    [
        50865084,
        109775243868575631,
        "0",
        233334,
        0,
        "SESSION_MATCH_KEY",
        "SESSION_MATCH_KEY",
        0,
        "no_map",
        "eNp1jtEKgjAUhnuWXS9wkpZeVhRRQqB0ExJDD7Vym7hZiPjubSuoi7o85/++/5we8RNtteRUF5eE1gfQEhSKjzk2iYIKCs2kQHFvRgdlXQ2rip4N5FnmwcRCipJZzImD3V4lE1AmVkhBKZNtligeE/x9L9W00Rnj8K5qqLhBSe7EfVHuaCdbvZ+vt9DZZhL50SzCxJ9OIg/7XhiQMMg/YgaUq9+qo1rx4v4gw+gJPtNd0w==",
        0,
        8,
        "eNrtU02PmzAQ7W/hnFR8LOl6pT0sWZmAErIhfFc92IYIgyEoEBJS9b/XkDS7TbXqqZdqTx7PG888v5mR5NHX70K1224oS4xys/1MY+FBVu4myt1IqBvU0G1pPAsP0khoElT0pjgSNoj8Avhth0jSm7KoAEWWekeZz5M2YRe4zBeoIanTVUPcuE9Gi+Ql2cEdKpLFeoijtZ2guBvsvvK+HswiadAzapDwICSd2QQy29sybKK1MVlMDxR7oMJlxHBpt6Rk68iHefKKHbAO1Sgwb/1d6Ks5liUn1mEXQ60lMhORD/ZGtj3Op7yOYolhYHKfWro6OKHArrB8R5dUPOOy1EZQS0O5eSGzHlNPRlZ9MYqrv7/jIBBr7ttgH+SuDjMkRnXoxxzbHm7ynFzFTuOZd363HnimyNMYKa0WF7DmHFT+jhr0grnHNvTtNg5WdJmtuqWzUq2M8NMdaoYyOGHf43+wbjluiA65brYTyinjMaY9NSYXfXNeQ1xkubh0QoWf0lkPWyW6y+to4HzXUq6N6M7MCvuw67U16H077+7b+CSCC8dD6LN9DC3Guewj/W9xdod8kWtsDPhcIeBlbdRv+LrR0JN381CuRxl5Gs8jpaTMb3KZF+42C31Jw/qx4nOQ9bNk5J4TilBbOddcKSkkdeXz/+n9bPzelx7zAq0kBcyjYEGXrInP/YQdDpiHCyaSzpj40rn/kQ6WWLHXl7mrkqLX8mnAUGBxv8XcAnKNQINnzIn8Iws5z2h6ndltGFhTrIMMyV7uufHzdYYUrQ4DxkjO50QHEqHGZO6Y4Onp8VH4MfpzwfsNfLPc43e3eyy9rvf4H272B8sPlh8s/3eW3z79BF44tSI=",
        19,
        [
            [
                50865084,
                233334,
                -1,
                4275156,
                2039321,
                0,
                "/10.0.11.6"
            ]
        ],
        0,
        512,
        1,
        180,
        0,
        0,
        null,
        "ukwest",
        "UK"
    ]
]
```
