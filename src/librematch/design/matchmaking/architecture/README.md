# Architecture

- Client-Server (non-monolithic/microservices)(?)

#### Frontend

- Basically: Frontend <---> REST-API (CRUD) <---> Matchmaking Library

#### Backend

##### Registration with aoe2-Profile-ID

- e.g. `!register <aoe2 profile id>` – register the given account with the discord name
- then you are asked by Direct Message to create a lobby with special randomly generated settings
- the created lobby and the options are then checked by the bot and the mapping to the account is done internally
- good thing is that the register endpoint can theoretically be queried from the outside with all kinds of stuff (should be platform-agnostic, whether it's from openage or from voobly, from a discord bot, a web-app or anything else)

#### Persistence

- basic PG stuff I guess for the user information
- maybe a fast in-memory database for anything temporary that is only needed during the actual matchmaking process

#### UX

- if it is less likely that you will find a match in the next 2-3 minutes, it will recommend you better settings to find a faster match
- people should see how many players queue in the different settings
- they should be free to queue at a setting they chose to find a match

1. they should be able to play what they want
1. if there are no players in that settings, we give feedback and recommend them settings how they would find a faster match
1. like having dynamically pop up an Arabia 1v1 queue because there are like 25 people queuing right now
   1. could click on it and jump into the queue
   1. if there is another queue for Socotra, and you have Socotra in your settings as a “beloved map”,
      - and there are 7 people in it, you could feel free to pull that into your personal queue as well and check if one or both queues gives you a game and so on

#### Recorded games upload and analysation

- could even reward special plays analysed from the recorded game

1. we might want to reimplement/contribute to a recorded game parser in Rust ( https://github.com/SiegeEngineers/genie-rs/tree/default/crates/genie-rec )

- could get the recorded games from official API
