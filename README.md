# Kaggle_ChildMindInstitute

## 概要
子どもや青少年の身体活動に基づいて、問題のあるインターネット使用のレベルを予測できますか? このコンテストの目標は、子どもの身体活動とフィットネス データを分析し、問題のあるインターネット使用の早期兆候を特定する予測モデルを開発することです。これらのパターンを特定することで、より健康的なデジタル習慣を促進するための介入を開始できます。

## 評価
- 2重重み付きカッパ係数(k)によって算出
-> モデルの予測が「偶然の一致」よりもどれだけいいかを評価する指標
- 順序データによく利用される
- 目安
  - < 0         ：一致していない
  - 0.00 - 0.20 ：わずかな一致
  - 0.21 - 0.40 ：まずまずの一致
  - 0.41 - 0.60 ：中程度の一致
  - 0.61 - 0.80 ：かなりの一致
  - 0.81 - 1.00 ：ほぼ完全な一致
- 特徴
  - 予測の不均衡に敏感（正解データと分布が近しくなる必要がある）
  - ラベル間の差の大きさに敏感（ラベル1に対して2と間違えるより，5と間違えたほうがスコアが低くなる）

## 戦略
1. データ分析，EDA
   1. EDA.ipynb
