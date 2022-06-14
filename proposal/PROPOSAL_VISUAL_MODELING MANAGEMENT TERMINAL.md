# Proposal: Visual modeling management side
Author: zhangyifei、liuyuliang

Discussion: FATE/issues/3893

# Abstract #
This proposal describes a visual modeling manager based on Java and React implementation, which enables users to use FATE algorithms for federated modeling by dragging and dropping flow charts. In addition, the project also includes other management functions, such as participant management, data source management, training task management, model management, forecasting, modeling process results viewing, etc
# Background #
Is rich in the FATE of the learning algorithm, can support a variety of federal model training, but for the user's entry is higher, are not so friendly to the user experience, we are always in the process of training to adjust model parameters so that the observation model are the training results meet expectations, with the introduction of the visualized modeling process of drag drag type, Support the independent operation of each algorithm and result confirmation in the process of modeling, and facilitate the management of each participant, clear the use of data samples, to ensure that data samples are not abused, reduce the access threshold of users, and optimize user experience.

# Proposal #
Our proposal is to do this by creating a Portal project, a Web service based on Java and React implementations that helps users to implement federated modeling by dragging and dropping component flow diagrams.
Front-end UI: Package FATE as a visual component to create federated learning flow charts by dragging and dropping.
Back-end: Fate-flow is connected to FATE, and the process of federated learning is completed by running the flow chart created in the front-end UI.

# Non-Goals #
N/A

# Rationale #
N/A

# Compatibility #
N/A

# Implementation #
We will implement the first version of the service, including the front UI and back end, supporting the following:

1. Support participant management, including registration, discovery, signing, etc

2. Support data sample management, including self-owned data samples and data samples of partners

3. Support visual modeling, including algorithm component list, drag canvas, component parameter configuration, etc

4. Support data sample uploading, intersection, standardization, feature screening, vertical logistic regression and other algorithms in FATE.

# Open issues (if applicable) #
N/A