# ML.Net Sentiment Analysis Demo

This is a simple ML.Net demo showing how you can use ML.Net to train a model, save the model to a file, and then load that file in a different program.  

This repository has two projects in a single solution:
1. **Demo.SentimentAnalysis.Part1 (F#)** - Loads the training data, trains the model, runs some tests, saves the model to a file
2. **Demo.SentimentAnalysis.Part2 (C#)** - Loads the model created in the other project and throws whatever input you provide at the model.

## Part 1 Output
```
Testing trained model

### Train
Accuracy          : 0.8771
F1                : 0.8842
Positive Precision: 0.8550
Positive Recall   : 0.9155
Negative Precision: 0.9040
Negative Recall   : 0.8367

SentimentText: A very, very, very slow-moving, aimless movie about a distressed, drifting young man.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.595641375f
Features: Sparse vector of size 7907, 84 explicit values
PredictedLabel: false
Score: -19.7281933f

SentimentText: Not sure who was more lost - the flat characters or the audience, nearly half of whom walked out.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.58837676f
Features: Sparse vector of size 7907, 110 explicit values
PredictedLabel: false
Score: -45.7980728f

SentimentText: Attempting artiness with black & white and clever camera angles, the movie disappointed - became even more ridiculous - as the acting was poor and the plot and lines almost non-existent.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.753678203f
Features: Sparse vector of size 7907, 188 explicit values
PredictedLabel: false
Score: -16.5628166f

SentimentText: Very little music or anything to speak of.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.967485666f
Features: Sparse vector of size 7907, 52 explicit values
PredictedLabel: true
Score: 0.64545542f

SentimentText: The best scene in the movie was when Gerardo is trying to find a song that keeps running through his head.
Label: true
Probability: 0.0f
IdPreservationColumn: 0.929597497f
Features: Sparse vector of size 7907, 118 explicit values
PredictedLabel: true
Score: 41.2434196f



### Test
Accuracy          : 0.6761
F1                : 0.6806
Positive Precision: 0.6323
Positive Recall   : 0.7368
Negative Precision: 0.7287
Negative Recall   : 0.6225

SentimentText: The rest of the movie lacks art, charm, meaning... If it's about emptiness, it works I guess because it's empty.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.171681881f
Features: Sparse vector of size 7907, 113 explicit values
PredictedLabel: true
Score: 2.48205495f

SentimentText: Wasted two hours.
Label: false
Probability: 0.0f
IdPreservationColumn: 0.185497403f
Features: Sparse vector of size 7907, 20 explicit values
PredictedLabel: true
Score: 0.573475182f

SentimentText: And those baby owls were adorable.
Label: true
Probability: 0.0f
IdPreservationColumn: 0.250951052f
Features: Sparse vector of size 7907, 37 explicit values
PredictedLabel: false
Score: -32.9482346f

SentimentText: It's practically perfect in all of them ? a true masterpiece in a sea of faux "masterpieces.
Label: true
Probability: 0.0f
IdPreservationColumn: 0.128096819f
Features: Sparse vector of size 7907, 80 explicit values
PredictedLabel: true
Score: 50.0117111f

SentimentText: I can think of no other film where something vitally important occurs every other minute.
Label: true
Probability: 0.0f
IdPreservationColumn: 0.229808331f
Features: Sparse vector of size 7907, 93 explicit values
PredictedLabel: true
Score: 8.48926353f



Text       : It was cool, cute, and funny.
Prediction : true
Score      : 33.9868

Text       : It was very bad.
Prediction : false
Score      : -71.4956

Text       : It was the greatest thing I've seen.
Prediction : true
Score      : 36.9727

Testing loaded model

Text       : It was cool, cute, and funny.
Prediction : true
Score      : 33.9868

Text       : It was very bad.
Prediction : false
Score      : -71.4956

Text       : It was the greatest thing I've seen.
Prediction : true
Score      : 36.9727

```
