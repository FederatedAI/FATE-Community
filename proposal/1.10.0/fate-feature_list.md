## Feature 1.10.0
> FederatedML 
* Add semi-supervised Learning algorithm
* Add intel paillier cryptosystem library as an optional paillier scheme
* A more general way to support torch backend development in HomoNN
* Support multi-host intersection base on ECDH\DH psi protocol
* Optimize predicting process of Hetero SecureBoost
* Support using manually built model to transform data in HeteroFeatureBinning
* Support up sample with weight column in Sample Component

> FATE-Flow
* Support kerberos authentication on spark
* Support importing user created model and using in later job with ModelLoader
* Add two-way connectivity detection api
* Support submitting job by cluster mode on spark

> FATE-Board
* Display training sample quantity at leaf node in SecureBoost
* Optimization and arrangement of style library
* throttle data stream according to status of job，for reducing server concurrency and log volume

> Fate-Client
* Integrate min-test task into flow client
* Optimize fate client and pipeline initialization
* Support resetting role and model_id\version in pipeline

# R&D Plan
* Dev Time: 2022/09/01 - 2022/11/15
* Test Time: 2022/11/16 - 2022/12/15
* Release Time: 2022/12/16 - 2022/12/20



