---
title: "ChaosTheory"
date: 2022-02-22
draft: false
tags: ["chaos-theory","exponential-idle","Elm","math","simulator"]
---

# Chaos Theory の実装
[某放置ゲーム](https://conicgames.github.io/exponentialidle/)
に登場するカオス理論の点の動きがいいなと思って自分で実装しました．  
[こっから飛べます](https://iorin-elmo.github.io/elm-ChaosTheory/)
<!--more-->
## カオス理論とは
なんか初期値がちょっとでも違うと全く別の結果になるみたいなやつです(適当)  
## 実装した内容
今回僕が実装したのはローレンツアトラクタと呼ばれる種類のものです．  
数式とかは各々ググろう  
三次元の行列の回転とかやって計算量がゴリゴリにあるのでスペックの低いデバイスだと死ぬ可能性が高いです  
三次元の行列の積\*2を各点でやってるからまじで重い，あほ  
### 使った言語
Elmだよもちろん，使ってみな，飛ぶぞ