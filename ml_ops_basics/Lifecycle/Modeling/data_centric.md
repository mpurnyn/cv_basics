### Data Centric 

- focus on getting high-quality data to train on.
- ex. Holding the neural network architecture fixed, work to improve the data to do well on the problem.

### Data Augmentation
- adding/creating data to improve your algorithm in areas where it is performing weakly

### how to do it
Example In Audio
- Add the a clean example with a noisy waveform to make a test

**goal**
create examples for parts where the algorithm is weak, but humans do well on
- but tweaking parameters and testing every time can result in a lot of time lost training and not getting a better result
- it is better to use this data for sanity checking.

**checklist**
- is the data realistic
- is the data -> label mapping clear (could a human label it?)
- is the algorithm doing poorly on it?

**data iteration loop**
- add data -> train -> error -> add more data
- usually adding more data (to an unstructured data problem) does not make the algorithm accuracy worse
    - needs to meet these criteria
        - model is large (with low bias)
        - mapping is clear (humans could identify it)

### Adding features
- adding features to the data to improve results
- ex. adding characteristics to a user of an recomendation algorithm may make the recomendation better.