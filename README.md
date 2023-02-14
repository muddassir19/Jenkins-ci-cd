# Jenkins-ci-cd
Using Mutiple Agent we can run Multiple Agent for differnet Stages in the Declarative pipeline.
We also use Stash and Unstash in the pipeline.  Example: there are two agents, Agent1 and Agent2.
In Agent1 clone the repo and in Agent2 we need to build maven war file .So for this we need to copy the ,
Clone repo from Agent1 to Agent2 for Maven build purpose. So we use stash and unstash.

Mutiple Agent in single jenkins pipeline and Using stash we can pick files from one Agent and using unstash we can copy to different agent.
To use Mutile Agent pipeline we need configure Master Slave Configuration.
