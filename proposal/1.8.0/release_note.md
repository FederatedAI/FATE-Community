## Release 1.8.0
> FederatedML 
* Add SecureBoost-MO algorithm to speed up multi-class classification of Hetero & Homo SecureBoost
* Merge Hetero FastSecureBoost into Hetero SecureBoost as a boosting strategy option
* Speed up DH Intersection implementation, 30%+ faster
* Add non-coordinated-version Hetero Linear Regression, based on integrated Hetero GLM framework, with mixed protocol of HE and SPDZ
* Support weighted training in non-coordinated Hetero Logistic Regression & Linear Regression
* Homo LR support one-vs-rest
* Optimized Quantile Binning gk-summary structure & split point query

> FATE-ARCH
* Adjustable task_cores for standalone FATE

> FATE-Test
* Optimized testsuite printout table colorization
* Optimized testsuite printout summary status
* Include paillier encryption performance evaluation
* Include examples data upload and mnist download
* Provide pipeline to dsl convert tools.

> FATE-Client
* xxxx 
> FATE-Flow
* xxxx
> FATE-Board
* Supports GBDTMO mode in SBT.
* Add SSHE linr component.
* Add Writer component.
