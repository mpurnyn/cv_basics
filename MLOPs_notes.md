# Machine Learning Operations
set of tools and principles to support progress in ML Project Lifecycle

## ML Project Lifecycle Steps
-iterative process
1. Scoping
    - defining the project. decide key metrics like accuracy, latency, and throughput. estimage resources and time.
2. Data
    - defining data and baseline
    - labeling and organizing data
3. Modeling
    - selecting and training model
    - performing error analysis
4. Deployment
    - deploying in production
    - monitoring and maintaining system
        - checking for data/concept drift
            - drift occurs when the new data collected changes compared to the original data because of a change in the environment 

https://cdck-file-uploads-global.s3.dualstack.us-west-2.amazonaws.com/dlai/original/2X/9/95589262880194306f98de4a9353e16f010afc8d.pdf

## Checklist of questions
1. realtime or batch
2. cloud or edge/browser
3. computer resource limitations
4. latency, throughput (QPS)
5. logging
6. security and privacy

**Canary Development**
- roll out to small fraction of traffic to test initially and monitor system. ramp up gradully from there.

**Blue/Green Deployment**
- have two versions in production old and new and test on both. for easy rollback.

## Degrees of Automation
- Human only
- Human in control with Automation in "Shadow mode".
- Human in the loop
    - AI assistance
    - Partial Automation
- Full Automation

### Key challenges in ML Ops
1. doing well on training set
    - first step to see if a model is good. this needs to be achieved first before going to 2.
    - usually low average error
2. doing well on dev/test set
    - usually the target, but generally not good enough to achieve goals of the project
3. doing well on business metrics or project goals
    - important to stake holders

**low average error isnt good enough**
1. sometimes getting some inputs perfectly is more important than doing well on average
2. unaccptable level of bias for certain slices of data. you need to keep in mind protected classes and treating data "fairly"
3. rare classes / skewed data distribution. you need to account for rare casses and doing poorly on those rare cases even though the average is good would not be a good system.



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

### Step 