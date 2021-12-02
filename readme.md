Recursively embedded atom neural network 
=================================================
**1. Introduction:**
___________________________
Recursive Embedded Atomic Neural Network (REANN) is a physically-inspired neural network framework, in which the orbital coefficients in the original EANN are transmitted iteratively and are considered to depend on the local environment. REANN can formulate a complete description of atomic structure without explicitly calculating high-order correlations, and effectively incorporate non-local effects, validated by numerical results in a various system. This repo preserves the nn potential of this numerical result in this work (Reference 3) with the form of serializable models. The full package has been released at <REANN>(from https://github.com/zhangylch/REANN).

**2. Employ the model**
___________________________________________________
In this repo, a series of serializable models were generated using TorchScript embedded in PyTorch. Pytorch (or libtorch in c++ production) is required to employ these models. The "test.py" is a script to display how to inference with this serializable model generated by EANN.

**3. Requirements:**
___________________________________
* PyTorch 1.8.1
* opt_einsum 3.2.0

**References:**
1. The original EANN model: Yaolong Zhang, Ce Hu and Bin Jiang *J. Phys. Chem. Lett.* 10, 4962-4967 (2019).
2. The EANN model for dipole/transition dipole/polarizability: Yaolong Zhang  Sheng Ye, Jinxiao Zhang, Jun Jiang and Bin Jiang *J. Phys. Chem. B*  124, 7284–7290 (2020).
3. The REANN model: Yaolong Zhang, Junfan xia and Bin Jiang *Phys. Rev. Lett.* 127, 156002 (2021).
