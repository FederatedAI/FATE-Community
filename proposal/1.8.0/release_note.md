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
* Model migration optimization to reduce user operation steps
* Added version compatibility check in Component Center to support multiple parties using different versions
* Added batch disable table interface; table clean can be performed according to filter fields
> FATE-Board
* xxxx
