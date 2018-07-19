# PAFAnalysis

PAF a technique that prioritzes automatically-generated test failures based on the likelihood of violating implicit preconditions. 

PAF 

(1) **clusters** generated test failures due to the same cause, 

(2) **partitions** the clusters into two groups, likely fault-revealing and non-fault-revealing, and 

(3) **ranks** the paritioned clusters based on thier likelihood of violating implicit preconditions.


# Experimental Results

This Github provides the experimental data of PAF and the tool to replicate the results. 
The results of each subject contain the following components:

**test-flow-sets**: clusters of tests sharing the same crash origin, crash variable, and crash statement.  

**FR-cluster-OPT**: optimal set of fault revealing clusters that fail due to the same cause. This is used as the ground trugh of RQ1.

**FR-cluster-PAF**: set of fault revealing clusters returned by PAF. This also refers to fault revealing test flow-sets.

**FR-cluster-MSeer, FR-cluster-ReBucket**: clusters returned by existing clustering techniques, MSeer and ReBucket, respectively.

**ranking_PAF**: ranking results of PAF's test-flow-sets.

**ranking_PAF_alltests**: ranking results of PAF's individual tests.

**ranking_others.csv**: ranking results of JCrasher and Daikon's. 
