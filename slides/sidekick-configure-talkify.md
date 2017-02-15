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
