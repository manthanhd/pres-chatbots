##  Load Talkify

index.js

```javascript
  const talkify = require('talkify');

  const Bot = talkify.Bot;

  const BotTypes = talkify.BotTypes;

  const SingleLineMessage = BotTypes.SingleLineMessage;

  const TrainingDocument = BotTypes.TrainingDocument;
  const Skill = BotTypes.Skill;

  const bot = new Bot();
```

Note:
Not much is happening here. We're basically loading up the initial set of type definitions that we'll need later on.
The last line is actually creating a bot instance. Here, in the `new Bot()` section, optionally pass in a set of options that'll help us tweak some of the things in the bot. For now, lets leave everything to its default.
