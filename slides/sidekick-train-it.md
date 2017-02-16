##  Train it

We'll train our bot to learn two topics.

1. knock_joke
2. chuck_norris_joke

---

```javascript
bot.trainAll([
     new TrainingDocument('knock_joke', 'knock'),
     new TrainingDocument('knock_joke', 'knock knock'),

     new TrainingDocument('chuck_norris_joke', 'chuck norris'),
     new TrainingDocument('chuck_norris_joke', 'chuck'),
     new TrainingDocument('chuck_norris_joke', 'norris'),
     new TrainingDocument('chuck_norris_joke', 'chuck norris joke'),
 ], function () {
     console.log(' BOT> Ready.');
 });
```
