##  Quorums

*When a single classifier isn't enough.*

Note:
Single classifier can only go so far. For complex parsing, you'll need more than one.
In quorums, one classifier classifies one or two things.
Helps keep classifiers focused and light weight.
Allows you to use domain specific classifiers. Classification for location based questions will benefit from a different algorithm to that classifying general knowledge questions.

---

```javascript
const bot = new Bot({
  classifiers: [
    paymentQuestionsClassifier,
    appTroubleshootingClassifier
  ]
});
```

Note:
Identify domains that could benefit from identical classification algorithms.
Try to keep one classifier to one or two topic ratio. This will help you train it with a lot of training data.

---

### Pros

Better, more accurate classification on a range of topics.
Easy out of the box analytics.

---

### Cons

Could get costly when using it with external services like IBM Watson.

---

## Classification Graphs

---

*When having multiple serial classifiers isn't enough*

<img src="/pres-chatbots/resources/classification-graph.png" style="background: none; border: none; box-shadow: none;"/>

Note:
Scalability is always a problem in tech. Not many disciplines have this issue.
Imagine a bot that can answer all problems of the world. Surely you wouldn't want a million classifiers.
Maybe that'd work but it'd take a crazy amount of time. You could parallelize it but it still wouldn't be very accurate.
Helps get to a solution quicker using context driven strength based classification resolution.
DFS (quicker, potentially less accurate) vs BFS (slower, potentially more accurate) algorithms to evaluate graphs.

---

## Selective vs Additive skill resolution strategy

---

*Topic focused vs description focused*

<img src="/pres-chatbots/resources/additive-classification.png" style="background: none; border: none; box-shadow: none;"/>

Note:
Selective: 'Best match'
Additive: 'feature resolution'
