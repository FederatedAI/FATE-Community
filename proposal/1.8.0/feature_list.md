## Feature 1.8.0
> HightLight
* Add non-coordinated-version Hetero Linear Regression
* Add SecureBoost-MO algorithm to speed up multi-class classification

> FederatedML 
* Add SecureBoost-MO algorithm to speed up multi-class classification of Hetero & Homo SecureBoost
* Merge Hetero FastSecureBoost into Hetero SecureBoost as a boosting strategy option
* Add non-coordinated-version Hetero Linear Regression, based on integrated Hetero GLM framework, with mixed protocol of HE and SPDZ
* Support weighted training in non-coordinated Hetero Logistic Regression & Linear Regression
* Homo LR support one-vs-rest
* Speed up DH Intersection implementation, 30%+ faster
* Optimized Quantile Binning gk-summary structure & split point query

> FATE-ARCH
* Adjustable task_cores for standalone FATE

> FATE-Test
* Optimized testsuite printout table colorization
* Optimized testsuite printout summary status
* Include Paillier encryption performance evaluation
* Include examples data upload and mnist download
* Provide pipeline to dsl convert tools.

> FATE-Flow
* Optimize the model migration function to reduce user operation steps
* Add version compatibility check in component center to support multiple parties to use different versions
* Add batch disable table interface, and clean up tables based on filter fields

> FATE-Board
* Supports GBDTMO mode in SBT.
* Add SSHE linr component.
* Add Writer component.
