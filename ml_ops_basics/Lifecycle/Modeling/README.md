# The Modeling Step in the ML Lifecycle
During the Modeling step is when you
- select and train a model
- perform error analysis


### Common Key Challenges
- Handeling Skewed datasets
- Model doesnt do well in the real world despite doing well on the Test Data.

### Aproaches to Modeling
- Model-Centric Approach
    - trying to find the best architecture
- Data-Centric Development
    - focus on getting high-quality data to train on.
    - ex. Holding the neural network architecture fixed, work to improve the data to do well on the problem.


### ML is an iterative process cycle
### Step 1. Model + Hyperparameters + Data
**getting started**
to get started on the new problem you can
1. do a quick literature search to find what is possible but dont spend too much time. find something reasonable.
2. find open-source implementations if available
3. find a reasonable algorithm with good data because that can often outperform something cutting edge with lacking or poor data.
4. getting the process and cycle started is more important than delaying until you get something perfect.

**Establish a baseline**
- try to find a baseline for what counts as a "better" system
- what to use for baseline? 
    - human level performance
    - state of the art in open source or literature
    - quick and dirty implementation
    - performance of older systems

**deployment contstraints**
- figuring out cpu/gpu/other constraints of the deployment are early is good, but it is more important to establish a baseline

**Sanity-check**
- try to overfit a small training data set before training a large one
    - make sure that you dont waste time running a broken model on a large data set.

### Step 2. Training

### Step 3. Error Analysis