---
title: "LogicCalculator"
date: 2020-12-30
draft: false
tag: ["Simulator","Parser","Elm"]
---

# SATソルバの実装
[ここから飛べます](https://iorin-elmo.github.io/elm-LogicCalculator/).  
構文解析のライブラリを作ったので使いたいと思い，高機能の計算機を作るのに挫折したので一旦ちょっと簡単なSATソルバを書いてみました．  
再帰下降構文解析が関数型言語とかなり相性がいいことがわかってよかったです．  
<!--more-->

## 使い方
ボタンがあると思うので，それ使って論理式を立てることができます．  
あとは命題変数を設定することができて，任意のアルファベット1文字で命題変数を定義できます．  
例えば`A⋏B`という風に入力すると`And A B`という風に解釈されます．  
ここまでは構文解析です．  
文字列が解析されると，命題変数が含まれる式についてはチェックボックスが出現します．  
チェックボックスがTrue/Falseの二値に対応していて，式の評価を変更できます．  
また，Solveをすることができ，  
充足可能性問題（SAT）を解くことができます．  
