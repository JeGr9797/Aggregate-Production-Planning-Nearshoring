# Aggregate-Production-Planning-Nearshoring
The code where the Aggregate Production Planning problem can be solved under uncertainty from the research article ""Multiproduct, multiperiod aggregate production planning subject to maximum inventory area and service level with demand uncertainty: A nearshoring context in Mexican companies" is posted in this repository.

The model is the following: 

$min\sum_{s\in S}{p^s\sum_{k\in K}{W_k^sc_{W\left(k\right)}\left|T\right|}}\ \ +\sum_{s\in S}{p^s\sum_{t\in T}\sum_{k\in K}\left(U_{\left(t\right)k}^sc_{U\left(k\right)}+B_{\left(t\right)k}^sc_{B\left(k\right)}+I_{\left(t\right)k}^sc_{I\left(k\right)}\right)}+A_{req}^sc_{A_{req}}\ 
(11)$
$U_{\left(t\right)k}^s+I_{\left(0\right)k}=d_{\left(t\right)k}^s+I_{\left(t\right)k}^s-B_{\left(t\right)k}^s\ \forall t=1,k\in K,s\in S\  (12)$
$U_{\left(t\right)k}^s+I_{\left(t-1\right)k}^s=d_{\left(t\right)k}^s+I_{\left(t\right)k}^s-B_{\left(t\right)k}^s+B_{\left(t-1\right)k}^s\ \forall t=2,\ldots,T,k\in K,s\in S\  (13)$
$U_{\left(t\right)k}^s\le W_k^s{cp}_k\ \forall t\in T,k\in K,s\in S\  (14)$
$\sum_{k\in K}{a_k\left(I_{\left(0\right)k}+U_{\left(t\right)k}^s\right)}\le a_{max}+A_{req}^s\ \forall t=1,\ s\in S\ (15)$
$\sum_{k\in K}{a_k\left(I_{\left(t-1\right)k}^s+U_{\left(t\right)k}^s\right)}\le a_{max}+A_{req}^s\ \forall t=2,\ldots,T,\ s\in S\ (16)$
$\sfrac{\sum_{t\in T}{(d_{\left(t\right)k}^s-B_{\left(t\right)k}^s)}}{\sum_{t\in T} d_{\left(t\right)k}^s}\geq{sl}_k\ \forall\ k\in K,s\in S\ (17)$
$A_{req}^s=\sum_{s\in N_{s\left(t\right)}}{p^sA_{req}^s/p\left(n_{s\left(t\right)}\right)\ }\forall\ s\in S\ (18)$
$W_k^s=\sum_{s\in N_{s\left(t\right)}}{p^sW_k^s/p\left(n_{s\left(t\right)}\right)\ }\forall\ k\in K,s\in S\  (19)$
$U_{\left(t\right)k}^s=\sum_{s\in N_{s\left(t\right)}}{p^sU_{\left(t\right)k}^s/p\left(n_{s\left(t\right)}\right)\ }\forall t\in T,k\in K,s\in S\ (20)$
$I_{\left(t\right)k}^s=\sum_{s\in N_{s\left(t\right)}}{p^sI_{\left(t\right)k}^s/p\left(n_{s\left(t\right)}\right)\ }\forall t\in T,k\in K,s\in S\ (21)$
$S_{\left(t\right)k}^s=\sum_{s\in N_{s\left(t\right)}}{p^sS_{\left(t\right)k}^s/p\left(n_{s\left(t\right)}\right)\ }\forall t\in T,k\in K,s\in S\ (22)$
$B_{\left(t\right)k}^s=\sum_{s\in N_{s\left(t\right)}}{p^sB_{\left(t\right)k}^s/p\left(n_{s\left(t\right)}\right)\ }\forall t\in T,k\in K,s\in S\  (23)$
$A_{req}^s\geq0\ \forall\ s\in S\ (24)$
$U_{\left(t\right)k}^s\geq0\ \forall t\in T,k\in K,s\in S\  (25)$
$W_k^s,B_{\left(t\right)k}^s,I_{\left(t\right)k}^s\in\mathbb{Z}_+\ \forall t\in T,k\in K,s\in S\ (26)$

