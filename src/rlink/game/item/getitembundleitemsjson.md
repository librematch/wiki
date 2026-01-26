# [GET] /game/item/getItemBundleItemsJson

**AUTHENTICATION**

## AoE2:DE

### Request

```
GET /game/item/getItemBundleItemsJson?callNum=123&connect_id=ccc&lastCallTime=111&sessionID=zzz&signature=sss HTTP/1.1
Cookie: ApplicationGatewayAffinity=0;ApplicationGatewayAffinityCORS=1;worldsedgelink=2;
Host: aoe-api.worldsedgelink.com
Accept-Encoding: identity
Accept: */*
Pragma: no-cache
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cache-Control: no-store
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |
| signature    | str       |       |          |

### Response

```
{
    "result": 0,
    "dataSignature": "Q8jVpeRaWqNAyXwg7I/+4elO6TtyZGGRFkgOzBdiuh+h3CTgIHvCODfZZ95GFMSSpkBOwAgW/rx0EOiPXLn1BKyQW1qjmLIJFkCAfy06JoxPGpRXoo6WxRyLhe3xg6YrIm4AVa2sxeAkA9mNfFfFr+feiSNZ/6HBp621flD+f2Y+zHPd3ClPcQGiEvQXy6CCzsfqifr15+zTXZKsrrCmKgnrWQpefBxcaQipsZy063tHmH1DVbq05nC+iiecZJjhe70Pn+hzTBli6AOhAvFjrU7/95JFyWuHsfHu9GjWWAz5XNppOaPs5qChhm4bqr/4hd6pmnD9h4htIDDctdiAJw=="
}
```

## AoE4

### Request

```
GET /game/item/getItemBundleItemsJson?callNum=223&connect_id=bgoo2n1murnn43kzdnnfc9fhp2no19&lastCallTime=2937108&sessionID=bgoo2n1murnn43kzdnnfc9fhp2no19&signature=fQDmHzAkaNfK40Ajoc1HDWJ6Fh4o43%2FmKKwoTOOtnWnoyKS7GiG07DGlO30sW5RpXAAcWbhOdpz27%2BGS7vI947VQv6I6onHGc6OkmlF3GUKeZnmYLZcm%2BZURtdWpo6%2BBX%2F6RY%2FFPgnYomeCcDtMbmSMYM5KkWy09j3jOotN%2FIHCQD0rPZAkFdUV8nMeSTDAh1WcM%2BS6eWROjfy9yuZ76x2ZrNDNamFS9noHP%2Bi3ViCtQjdmwy9Q%2BVWKKzdmoAIM8tri3YEZMPJH%2FVMJyRENE7J4VMGGL6lzAkNmjIm%2BT66w%2B7XIRiC3aWo5DY8RdsvuIDpExG3AyQXr%2FL2dGT87POg%3D%3D HTTP/1.1
Host: aoe-api.worldsedgelink.com
Accept: */*
Accept-Encoding: identity
Cookie: ApplicationGatewayAffinity=a2bd9c803374aa3cdd1337b02986746f;ApplicationGatewayAffinityCORS=a2bd9c803374aa3cdd1337b02986746f;worldsedgelink=-1321719400;
Cache-Control: no-store
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Pragma: no-cache
```

| parameter    | type      | value | comments |
| ------------ | --------- | ----- | -------- |
| callNum      | int       | 123   |          |
| connect_id   |           |       |          |
| lastCallTime | timestamp |       |          |
| sessionID    | str       |       |          |
| signature    | str       |       |          |

### Response

```
{
    "result": 0,
    "dataSignature": "fQDmHzAkaNfK40Ajoc1HDWJ6Fh4o43/mKKwoTOOtnWnoyKS7GiG07DGlO30sW5RpXAAcWbhOdpz27+GS7vI947VQv6I6onHGc6OkmlF3GUKeZnmYLZcm+ZURtdWpo6+BX/6RY/FPgnYomeCcDtMbmSMYM5KkWy09j3jOotN/IHCQD0rPZAkFdUV8nMeSTDAh1WcM+S6eWROjfy9yuZ76x2ZrNDNamFS9noHP+i3ViCtQjdmwy9Q+VWKKzdmoAIM8tri3YEZMPJH/VMJyRENE7J4VMGGL6lzAkNmjIm+T66w+7XIRiC3aWo5DY8RdsvuIDpExG3AyQXr/L2dGT87POg=="
}
```
