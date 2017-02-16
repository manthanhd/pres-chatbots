##  Knock Knock Joke Skill

Install `knock-knock-jokes` module

```sh
npm install --save knock-knock-jokes
```

Define skill

```javascript
const knockKnockJokes = require('knock-knock-jokes');
const kJokeSkill = new Skill(
  'my_knock_knock_joke_skill',
  'knock_joke',
  function (context, request, response) {
    return response.send(new SingleLineMessage(knockKnockJokes()));
});
```
