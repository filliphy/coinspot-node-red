# coinspot-node-red
Various Flows for Coinspot API interaction via node-red

I have seen lots of repos that have various code on interacting with the coinspot API, however I wasn't (not being a coder) able to easily figure out how to change it easily into a node-red HTTP request.

I kept getting an error return as - *invalid/missing nonce* despite having what I thought was the correct setup, however the correct payload for the API was to have the nonce as a JSON string (rather than a Javascript Object from node-red).


The API documentation is at: https://www.coinspot.com.au/api

**My Balances.json**
- https://www.coinspot.com.au/api#romybalances 	
- you need to replace the API Key in the inject node, and the secret (from the coinspot API page when you created it) into the HMAC
 - the first API request setup
 - could probably be optimised (please re-upload or let me know if you can).
