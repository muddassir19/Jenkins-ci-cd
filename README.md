# Jenkins-ci-cd
Using Mutiple Agent we can run Multiple Agent for differnet Stages in the Declarative pipeline.
We also use Stash and Unstash in the pipeline.  Example: there are two agents, Agent1 and Agent2.
In Agent1 clone the repo and in Agent2 we need to build maven war file .So for this we need to copy the ,
Clone repo from Agent1 to Agent2 for Maven build purpose. So we use stash and unstash.
