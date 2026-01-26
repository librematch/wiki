# [GET] /community/clan/getClanInfoFull

[Example request](https://aoe-api.worldsedgelink.com/community/clan/getClanInfoFull?title=age2&name=gli)

## Request

| parameter | type     | value                  | comments |
| --------- | -------- | ---------------------- | -------- |
| title     | str/enum | age1, age2, age3, age4 |          |
| name      | str      | gli                    |          |

## Response

### AoE2:DE

```
{
  "result": {
    "code": 0,
    "message": "SUCCESS"
  },
  "clan": {
    "id": 52618,
    "name": "gli",
    "fullname": "TheClick",
    "description": "",
    "tags": "",
    "icon": "CR-001",
    "membercount": 4,
    "joinpolicy": 0,
    "metadata": "",
    "messageoftheday": "",
    "statgroup_id": 2254028,
    "permissions": [
      {
        "rank": 1,
        "chat": 1,
        "promote": 1,
        "demote": 1,
        "invite": 1,
        "remove": 1,
        "disband": 1,
        "editinfo": 1,
        "editpermission": 1,
        "name": "Leader",
        "locstringid": -1
      },
      {
        "rank": 2,
        "chat": 1,
        "promote": 1,
        "demote": 1,
        "invite": 1,
        "remove": 1,
        "disband": 0,
        "editinfo": 0,
        "editpermission": 0,
        "name": "Officer",
        "locstringid": -1
      },
      {
        "rank": 3,
        "chat": 1,
        "promote": 0,
        "demote": 0,
        "invite": 0,
        "remove": 0,
        "disband": 0,
        "editinfo": 0,
        "editpermission": 0,
        "name": "Member",
        "locstringid": -1
      }
    ],
    "members": [
      {
        "avatar": {
          "entityversion": 15609,
          "profile_id": 238631,
          "name": "/steam/76561198114433482",
          "metadata": "{\"icon\":\"PR7-019\"}",
          "alias": "Timinator",
          "clanlist_name": "gli",
          "personal_statgroup_id": 38975,
          "xp": 622,
          "level": 1,
          "leaderboardregion_id": 3,
          "presence_id": 0,
          "presenceproperty": []
        },
        "membershipstatus": 1,
        "playerlistpermission_rank": 3
      },
      {
        "avatar": {
          "entityversion": 5612,
          "profile_id": 2107872,
          "name": "/steam/76561198125039468",
          "metadata": "{\"icon\":\"PR4-010\"}",
          "alias": "Matt Bootsma",
          "clanlist_name": "gli",
          "personal_statgroup_id": 1872571,
          "xp": 195,
          "level": 1,
          "leaderboardregion_id": 3,
          "presence_id": 0,
          "presenceproperty": []
        },
        "membershipstatus": 1,
        "playerlistpermission_rank": 3
      },
      {
        "avatar": {
          "entityversion": 7676,
          "profile_id": 2327018,
          "name": "/steam/76561198300477799",
          "metadata": "{\"icon\":\"PR7-031\"}",
          "alias": "Atashwong",
          "clanlist_name": "gli",
          "personal_statgroup_id": 2072253,
          "xp": 276,
          "level": 1,
          "leaderboardregion_id": 3,
          "presence_id": 0,
          "presenceproperty": []
        },
        "membershipstatus": 1,
        "playerlistpermission_rank": 1
      },
      {
        "avatar": {
          "entityversion": 3579,
          "profile_id": 2407155,
          "name": "/steam/76561198449514731",
          "metadata": "{\"icon\":\"PR7-033\"}",
          "alias": "ekorvee",
          "clanlist_name": "gli",
          "personal_statgroup_id": 2149677,
          "xp": 136,
          "level": 1,
          "leaderboardregion_id": 3,
          "presence_id": 0,
          "presenceproperty": []
        },
        "membershipstatus": 1,
        "playerlistpermission_rank": 3
      }
    ]
  }
}
```

```
{
    "$schema": "http://json-schema.org/schema#",
    "type": "object",
    "properties": {
        "result": {
            "type": "object",
            "properties": {
                "code": {
                    "type": "integer"
                },
                "message": {
                    "type": "string"
                }
            },
            "required": [
                "code",
                "message"
            ]
        },
        "clan": {
            "type": "object",
            "properties": {
                "id": {
                    "type": "integer"
                },
                "name": {
                    "type": "string"
                },
                "fullname": {
                    "type": "string"
                },
                "description": {
                    "type": "string"
                },
                "tags": {
                    "type": "string"
                },
                "icon": {
                    "type": "string"
                },
                "membercount": {
                    "type": "integer"
                },
                "joinpolicy": {
                    "type": "integer"
                },
                "metadata": {
                    "type": "string"
                },
                "messageoftheday": {
                    "type": "string"
                },
                "statgroup_id": {
                    "type": "integer"
                },
                "permissions": {
                    "type": "array",
                    "items": {
                        "type": "object",
                        "properties": {
                            "rank": {
                                "type": "integer"
                            },
                            "chat": {
                                "type": "integer"
                            },
                            "promote": {
                                "type": "integer"
                            },
                            "demote": {
                                "type": "integer"
                            },
                            "invite": {
                                "type": "integer"
                            },
                            "remove": {
                                "type": "integer"
                            },
                            "disband": {
                                "type": "integer"
                            },
                            "editinfo": {
                                "type": "integer"
                            },
                            "editpermission": {
                                "type": "integer"
                            },
                            "name": {
                                "type": "string"
                            },
                            "locstringid": {
                                "type": "integer"
                            }
                        },
                        "required": [
                            "chat",
                            "demote",
                            "disband",
                            "editinfo",
                            "editpermission",
                            "invite",
                            "locstringid",
                            "name",
                            "promote",
                            "rank",
                            "remove"
                        ]
                    }
                },
                "members": {
                    "type": "array",
                    "items": {
                        "type": "object",
                        "properties": {
                            "avatar": {
                                "type": "object",
                                "properties": {
                                    "entityversion": {
                                        "type": "integer"
                                    },
                                    "profile_id": {
                                        "type": "integer"
                                    },
                                    "name": {
                                        "type": "string"
                                    },
                                    "metadata": {
                                        "type": "string"
                                    },
                                    "alias": {
                                        "type": "string"
                                    },
                                    "clanlist_name": {
                                        "type": "string"
                                    },
                                    "personal_statgroup_id": {
                                        "type": "integer"
                                    },
                                    "xp": {
                                        "type": "integer"
                                    },
                                    "level": {
                                        "type": "integer"
                                    },
                                    "leaderboardregion_id": {
                                        "type": "integer"
                                    },
                                    "presence_id": {
                                        "type": "integer"
                                    },
                                    "presenceproperty": {
                                        "type": "array"
                                    }
                                },
                                "required": [
                                    "alias",
                                    "clanlist_name",
                                    "entityversion",
                                    "leaderboardregion_id",
                                    "level",
                                    "metadata",
                                    "name",
                                    "personal_statgroup_id",
                                    "presence_id",
                                    "presenceproperty",
                                    "profile_id",
                                    "xp"
                                ]
                            },
                            "membershipstatus": {
                                "type": "integer"
                            },
                            "playerlistpermission_rank": {
                                "type": "integer"
                            }
                        },
                        "required": [
                            "avatar",
                            "membershipstatus",
                            "playerlistpermission_rank"
                        ]
                    }
                }
            },
            "required": [
                "description",
                "fullname",
                "icon",
                "id",
                "joinpolicy",
                "membercount",
                "members",
                "messageoftheday",
                "metadata",
                "name",
                "permissions",
                "statgroup_id",
                "tags"
            ]
        }
    },
    "required": [
        "clan",
        "result"
    ]
}
```
