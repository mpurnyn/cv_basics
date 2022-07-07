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