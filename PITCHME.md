### Apache Spark Machine Learning Blueprint

Chapter.5 Risk Scoring on Spark

chie hayashida

---

### Agenda

* Introduction
* Spark for risk scoring
* The use case
* Apache Spark notebooks
* Methods of risk scoring
	* Logistic regression
	* Random forest and decision trees
	* Data and feature preparation
	* OpenRefine
* Model estimation
* Model evaluation
	* Confusion matrix
	* ROC
	* Kolmogorov-Smirnov
	* Results explanation
	* Big influencers and their impacts
* Deployment
	* Scoring
* Summary

@title[Agenda]
---
### Spark for risk scoring

---
### Use Case
```
XST Corpはビジネス継続や個人的な緊急の事情のために現金を必要とする
数百万の個人へローンやその他の財政的支援を提供している。
この会社は、オンライン申し込みを受け付け、申し込みに対して
一時的な決断をする。
このために、彼らはオンライン申し込みの内容、DWHに収集済みの
過去のデータ、サードパーティから提供されるデータを利用する。

オンライン申し込みは個人を特定するデータと申込者の財政状況に関する
データを含む。
収集済みのデータは、地理、財政、その他に関連する情報を含む。
サードパーティによるデータは、過去のクレジット、現在の雇用状況等の
情報を含む。

この会社は競合会社が多く、変化が多い。
そこで、彼らは常に競合に負けないよりよいリスクスコアリングモデルを
探している。
特に競合より精度良く予測し、かつたくさんの申込者に対して少ないリスクで
受け入れたい。
```
---
### Use Case(続き)

```

```
---

### math test

$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$

$$\hat{r}_{ij} = {p_{i}}^{T}q_{j} = \sum_{k=1}^{k}p_{ik}q_{kj}$$

@title[math example]
---
### fin3

@title[custome label]

