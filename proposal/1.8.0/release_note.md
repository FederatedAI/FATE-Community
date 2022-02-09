## Release 1.8.0
> FederatedML 
* Add SecureBoost-MO algorithm to speed up multi-class classification of Hetero & Homo SecureBoost
* Model inference protection enhancement for Hetero SecureBoost with FED-EINI algorithm.
* Merge Hetero FastSecureBoost into Hetero SecureBoost as a boosting strategy option
* Speed up DH Intersection implementation, 30%+ faster
* Add two-party-version Hetero Linear Regression, based on integrated Hetero GLM framework, with mixed protocol of HE and SPDZ
* Support weighted training in two-party Hetero Logistic Regression & Linear Regression
* Homo LR support one-vs-rest
* New batch strategy in three-party Hetero LR: support masked batch data and batch shuffle
* Optimized Quantile Binning gk-summary structure & split point query
* Hetero SecureBoost supports split feature importance on host side. 

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
* xxxx

> Bug-Fix
* Fix Data Transform's schema label name setting problem when `with_label` is False