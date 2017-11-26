# butlerbot-uno

uno plugin for butlerbot


## Install

```sh
yarn add butlerbot-uno
```
Create a file in the plugin dir as follows

```js
import uno from 'butlerbot-uno';
export default uno({
  development: {
    "url": "http://redbrick.dcu.ie/api/committee",
    channels: ['#butlerbot'],
    channelsToExclude: [],
    channelsToJoin: ['#butlerbot'],
    "gameOptions": {
      "turnMinutes": 3,
      "maxIdleTurns": 3,
      "idleRoundTimerDecrement": 60,
      "setTopic": true,
      "topicBase": "|| Dev Bot || Expect spam || Expect breakings"
    },
  },

  production: {
    "url": "http://redbrick.dcu.ie/api/committee",
    channels: ['#butlerbot'],
    channelsToExclude: [],
    channelsToJoin: ['#butlerbot'],
    "gameOptions": {
      "turnMinutes": 3,
      "maxIdleTurns": 3,
      "idleRoundTimerDecrement": 60,
      "setTopic": true,
      "topicBase": "|| Dev Bot || Expect spam || Expect breakings"
    },
  },
});
```
