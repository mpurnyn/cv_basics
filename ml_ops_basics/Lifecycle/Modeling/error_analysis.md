### Key challenges in ML Ops
1. doing well on training set
    - first step to see if a model is good. this needs to be achieved first before going to 2.
    - usually low average error
2. doing well on dev/test set
    - usually the target, but generally not good enough to achieve goals of the project
    - it does not mean you will do well on rare cases, have low bias, or that the system can be deployed.
3. doing well on business metrics or project goals
    - important to stake holders

**When low average error isn't good enough**
1. sometimes getting some inputs perfectly is more important than doing well on average
2. unaccptable level of bias for certain slices of data. you need to keep in mind protected classes and treating data "fairly"
3. rare classes / skewed data distribution. you need to account for rare casses and doing poorly on those rare cases even though the average is good would not be a good system.

**Skewed Datasets**
- When you labeled data is not evenly split and more examples exist of one category than the others.
- Precision and Recall are good metrics  

**Better metrics than raw accuracy**
Confusion Matrix to evaluate the algorithm - a true/false positive negative matrix
Precision = TP/(TP+FP)
Recall = TP/(TP+FN)
F1 Score (combine precision and recal) = 2/(1/Precision + 1/Recall)

**Performance Auditing**
Auditing framework - a way to check for accuraccy, bias, and other problems before deployment
1. Brainstorm ways the system can do wrong
    - performance on subsets of data (avoid bias)
    - how common are errors (accuracy)
    - performance on rare classes (bias)
2. Establish metrics to access performance
    - based on the brainstorming, choose metrics that help prevent them