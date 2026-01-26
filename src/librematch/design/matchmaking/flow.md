# Flow

## Before the game

- Persons can register for the matchmaking, becoming Users of our service
- Users can connect their aoe2-profile with their account
- Users can adjust their personal preferences regarding maps, ladders etc. in the settings.
- Users can queue up for their settings or join a queue they see are the most people in, other recommendations
- Users get informed of their match in their client with a pop-up, switching to the settings of the match
- A Host is being decided randomly of all participating players.
- Else, Users can set their preference in the settings if they like to be hosted more often.
- Hosts create the game lobbies (until, we haven't found a way to automate that)
- Lobby settings get verified as much as possible via aoe2.net matches API endpoint
- Match starts

## After the game

- get basic game information/result from aoe2.net
- download, parse and analyse recorded games
- use results if recs are unavailable

1. results when both players pick no team still show both winning, so recs would be best (aoe2.net)

- create rating change

1. with the recs analysation, we could even calculate a more precise rating change depending on how the game played out
1. like a player that was dead in minute 13 and just stayed in the game until 1h25 because the person had a vill hidden in the corner should probably not get so much rating change as someone that was carrying all the people the whole game (just as an idea)
