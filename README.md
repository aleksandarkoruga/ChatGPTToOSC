# ChatGPTToOSC
 OSC Relay from ChatGPT @waylaidwanderer/node-chatgpt-api
  - This relay was created for the purpose of bringing ChatGPT into the SuperCollider environment to test live coding possibilities, architectural feedback, system design etc.
  - It is heavily based on @waylaidwanderer/node-chatgpt-api test code and minimal osc.js implementation.
  
# Usage 

 - `git clone https://www.github.com/aleksandarkoruga/ChatGPTToOSC`
 - `cd ChatGPTToOSC`
 - rename `settings.example.js` to `settings.js`
 - Edit `settings.js`: 
   - Provide an API key under `openaiApiKey` (insert it between the last ''). You can find your API key following the instructions on  https://platform.openai.com/account/api-keys 
   - To change the default model, edit/add the `model` entry under `modelOptions`, for further details about the model selection and other options please refer to the original API https://github.com/waylaidwanderer/node-chatgpt-api
   - Edit `localPort`, `remotePort` and `remoteAddress` under `oscOptions`  
 
 - from the `ChatGPTToOSC` root folder run `npm install` 
 - `node .` to run the relay.
 - run `chatgpt-test.scd` from `ChatGPTToOSC/SuperCollider`

# Notes
 The relay transmits the fully assembled response, so based on the query and the selected model it may take more or less time to receive a reply in the OSC client (SuperCollider etc)
