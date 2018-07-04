# TIMERS
This is a sample implementation of "[Community Preserving Network Embedding](http://cuip.thumedialab.com/papers/NE-Community.pdf)"(AAAI 2017).

### Requirements
```
MATLAB 
```

### Usage
run `MNMF.m` with matlab
```
function [U, M, H, C, L] = MNMF(S, M, U, H, C, B1, B2, alpha, beta, lambda)
% The demo is written by Xiao Wang (wangxiao007@mail.tsinghua.edu.cn), and the details of the algorithm can be
% found in "Community Preserving Network Embedding" (AAAI 2017).
%%--------------input-----------------
% S: S1+5*S2, the first- and second-order proximities (n-by-n);
% M: the initialized basis matrix (n-by-m);
% U: the initialized representations of nodes (n-by-m);
% H: the initialized community indicator matrix (n-by-k);
% C: the initialized representations of communities (k-by-m);
% B1: the adjacency matrix B1(i,i)=0 (n-by-n);
% B2: (k_i*k_j)/2e (n-by-n);
% alpha, beta, lambda: the values of parameters, usually alpha and beta need to be tuned and we can set lambada = 1e9;
%%-------------output------------------
% U: the optimal representations of nodes;
% M: the optimal basis matrix;
% H: the optimal community indicator matrix;
% C: the optimal representations of communities;
% L: the final values of objective function.
%%-------------------------------------
```

### Cite
If you find this code useful, please cite our paper:
```
@inproceedings{wang2017community,
  title={Community Preserving Network Embedding},
  author={Wang, Xiao and Cui, Peng and Wang, Jing and Pei, Jian and Zhu, Wenwu and Yang, Shiqiang},
  booktitle={Proceedings of the 31st AAAI Conference on Artificial Intelligence},
  year={2017}
}
```