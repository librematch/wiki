# Roadmap

1. PoC Script
   1. play a bit around with it how to get data from different endpoints
   1. adopt it to any changes on the API and the different endpoints
   1. create test script out of it that tests the availability of different endpoints, which parameters are optional and saves the responses together with the requests for easier OpenAPI file generation
   1. analyse the responses and map them to fields and document it
1. Data collection & Database
   1. based on our findings from the PoC Script we can start thinking about database layout and implement a tool for data collection
   1. we should divide our effort into a smaller working group that starts with thinking about a possible architecture
   1. i think it makes sense to automate as much as possible, e.g. logging the endpoints/requests the games use together with the responses, automatically create an openapi file from it, generate a client from it for the data collector and pull in this generated client as a library for the data collector itself, so it's easier to update
   1. sufficient error handling will be pretty important here as the API is relatively instable and as you might see from the initial response, it's basically one huge JSON array with only the values, sometimes completely empty arrays at positions, the order of these things might also changes by chance without any warning
1. Backend
   1. in parallel we can draft a possible backend solution
   1. for most information a basic REST-API will be sufficient, but for other things Pub/Sub and Websockets will be nice (e.g. subscribing to the matches of a player and get updates in real-time)
   1. also it would be nice to have a login endpoint for e.g. tournament organizers, so they can hide the results of matches of certain relic-link ids for a limited amount of time to avoid spoilers
1. Frontend(s)
   1. imho frontends should be not part of the work of this group
   1. frontends can be implemented by anyone that likes to use our backend
   1. we can ask someone or maybe we know already some people that can create nice ones and cooperate with these people closely
   1. like this we divide our effort and fix on the purpose of having a stable API for the community while other people are able to concentrate on their frontend efforts
