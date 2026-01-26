# Item Endpoints

Endpoints for managing in-game items, inventory, and the item shop.

> **Authentication:** All endpoints in this section require Steam authentication.

## Endpoints

| Endpoint                                                  | Method | Description                  |
| --------------------------------------------------------- | ------ | ---------------------------- |
| [detachItems](./detachitems.md)                           | POST   | Detach items from loadout    |
| [getInventoryByProfileIDs](./getinventorybyprofileids.md) | GET    | Get inventory for player(s)  |
| [getItemBundleItemsJson](./getitembundleitemsjson.md)     | GET    | Get item bundle contents     |
| [getItemDefinitionsJson](./getitemdefinitionsjson.md)     | GET    | Get all item definitions     |
| [getItemLoadouts](./getitemloadouts.md)                   | GET    | Get player's item loadouts   |
| [getItemPrices](./getitemprices.md)                       | GET    | Get item shop prices         |
| [getLevelRewardsTableJson](./getlevelrewardstablejson.md) | GET    | Get level-up rewards table   |
| [getPersonalizedSaleItems](./getpersonalizedsaleitems.md) | GET    | Get personalized sale offers |
| [getScheduledSaleAndItems](./getscheduledsaleanditems.md) | GET    | Get scheduled sales          |
| [moveCharges](./movecharges.md)                           | POST   | Move item charges            |
| [moveItem](./moveitem.md)                                 | POST   | Move item in inventory       |
| [openItemPack](./openitempack.md)                         | POST   | Open an item pack/lootbox    |
| [signItems](./signitems.md)                               | POST   | Sign items for verification  |
| [updateItemAttributes](./updateitemattributes.md)         | POST   | Update item attributes       |
