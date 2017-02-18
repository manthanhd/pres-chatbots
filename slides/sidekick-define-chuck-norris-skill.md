##  Chuck Norris Joke Skill

Install `chuck-norris-api` module

```sh
npm install --save chuck-norris-api
```

Define skill

```javascript
const cnApi = require('chuck-norris-api');
const cJokeSkill = new Skill(
  'my_chuck_norris_joke_skill',
  'chuck_norris_joke',
  function(context, request, response) {
    return cnApi.getRandom(
      {exclude: ['explicit']}
    ).then(function(data) {
        return response.send(new SingleLineMessage(data.value.joke));
    });
});
```
