##  Chuck Norris Joke Skill

Install `chuck-norris-api` module

```sh
npm install --save chuck-norris-api
```

Define skill

```javascript
const cnApi = require('chuck-norris-api');
const kJokeSkill = new Skill('my_knock_knock_joke_skill', 'knock_joke', function (context, request, response) {
    return response.send(new SingleLineMessage(knockKnockJokes()));
});
```
