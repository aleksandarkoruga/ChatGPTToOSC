# ChatGPTToOSC
 OSC Relay from ChatGPT @waylaidwanderer/node-chatgpt-api
  - This relay was created for the purpose of bringing ChatGPT into the SuperCollider environment to test live coding possibilities, architectural feedback, system design etc.
  - It is heavily based on @waylaidwanderer/node-chatgpt-api test code and minimal osc.js implementation.
  
# Usage 

 - `git clone https://www.github.com/aleksandarkoruga/ChatGPTToOSC`
 - `cd ChatGPTToOSC`
 - rename `settings.example.js` to `settings.js`
 - edit `settings.js` and provide an API key under `openaiApiKey` (insert it between the last ''). you can find your API key following the instructions on  https://platform.openai.com/account/api-keys 
   for further details about the other options refer to the original API https://github.com/waylaidwanderer/node-chatgpt-api
   edit `localPort`, `remotePort` and `remoteAddress` under `oscOptions`  
 
 - from the `ChatGPTToOSC` root folder run `npm install` and `node .` to run the relay.
 - run `chatgpt-test.scd` from `ChatGPTToOSC/SuperCollider`
