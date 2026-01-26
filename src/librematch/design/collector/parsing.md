# Parsing

The parsing stages does the decoding/decompression, normalization and prioritization.

- decoding/decompression\
  Some data, especially in 'slotinfo', is base64 encoded and further compressed with zlib.

- normalization\
  The data format is 'json-like', but only contains arrays. Probably for bandwidth reasons.\
  We need to transfer the data in our own schema.

- prioritization\
  Some data is the foundation for real-time information that we deliver to users of our API (state changes of lobbies, e.g. ongoing matches, and leaderboard rankings).\
  This data should fill 'sorted sets' or the Pub/Sub-Message bus from Redis.

- conversion\
  For the localization data, we need to query data from the Relic Link API and convert it to the FTL (Fluent Translation) file format.
