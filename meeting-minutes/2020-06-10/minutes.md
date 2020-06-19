# Meeting minutes of FATE community on 2020/06/10

## Topic
FATE LTS version & China Unionpay joins FATE TSC

## Attendees Present

Toby Chen@WeBank(Tianjian)
Dylan Fan@WeBank(dylan-fan)
Henry Zhang@VMware(hainingzhang)
Sookie Qin@Tencent(sookieqin)
Zotrseeew Ma@WeBank(mgqa34)
Jarvis Zeng@WeBank(zengjice)
Layne Peng@VMware
Clarkieliu@Tencent

## Minutes

### New FATE maintainer
1. Introduced a new friend Yongkai Zhou from China UnionPay and the current progress of China UnionPay and FATE；
2. Implemented the decision of Yongkai Zhou to join FATE TSC;

### FATE version discussion
1. Discussed about the planning of FATE LTS version and determined FATE v1.5 as the beginning of FATE LTS. The maintenance cycle of LTS is planned to last for 2 years.
2. Discussed about the R&D planning of FATE v1.5, mainly includes FAST SBT, FTL reconstruction, FATE-Pipeline, retry scheduling optimization of FATE-Flow, etc.

### FATE-operator
1. FATE-operator, an object submit to KubeFlow project, has been shared by VMware.
2. The community promotion of FATE-operator will be launched later.

### Discussion of FATE roadmap
1. Support for homogeneous online serving: FATE provides model conversion function and supports existing online frameworks such as tf-serving.
2. Support standalone offline prediction in homogeneous scenario
3. Add multiple types of input components such as images and audio data
4. Support for CNN and RNN: Reused existing deep-learning frameworks in homogeneous scenario while lacking requirements in heterogeneous scenario.
5. Support for ARM.



