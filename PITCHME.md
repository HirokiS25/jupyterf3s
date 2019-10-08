# ゼロから始めるJupyter Notebook

---

## 自己紹介

名前：坂本弘樹

所属：理学研究科素粒子論研究室(D3)


---


## 目次

* jupyterについて
* 


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

## Jupyter is 何？

**Python**をブラウザ上でインタラクティブに動かすためのWebアプリ


#### Jupyter labの起動

+ Windowsの人 → すべてのプログラム -> anaconda3 -> プロンプトを実行
+ Macの人 → ターミナル

```sh
jupyter lab
```

---

## Python

+ 最近人気のプログラミング言語
+ 習得が容易
+ 高収入？ [Ref.](https://jp.stanby.com/media/programming_ranking2017/)
+ **ライブラリが豊富**

---

### numpy, scipy

@fa[hand-point-right text-white]
`numpy`: 数値計算を高速に行うことが出来るライブラリ

@fa[hand-point-right text-white]
`scipy`: 科学計算に必要な特殊なモジュールを提供するライブラリ

```sh
import numpy as np
import scipy as sp


def f(x):
    return 4 / (1 + x ** 2)


sp.integrate.quad(f, 0, 1)
```

---

### sympy

@fa[hand-point-right text-white]
記号計算用ライブラリ

例えば，

@snap[text-06 span-100]
Q. $a x^2 + b x + c = 0$の解を求めよ. 
A. $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

のようなことが出来る．

参考：[2015年センター試験数学IAを全てプログラム(Python)で解く](https://qiita.com/akai_banana/items/b328fe0116d248127a36)
@snapend


---

### pandas

@fa[hand-point-right text-white]
データ解析をするためのライブラリ

`DataFrame`というオブジェクトを使って
様々なデータ処理を容易に行うことができる

---

ほかにも

- `Django, flask`: Webアプリ
- `TensorFlow, scikit-learn, Kelas`: 機械学習，深層学習，AI

などライブラリを使うことによって，様々なアプリケーションを作れる！

google, youtube, instagram

---

## Jupyterでできること

@snap[fragment]
ex.)  
1. 計算結果をグラフにプロットしてその結果をメモする 
2. 大量のデータの中から必要なところだけ抜き出してその特徴量の可視化を行う
@snapend

---
![example](url)

---

## python入門

---

![画面の説明](url)


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### Hello, world

pythonではクォーテーションかダブルクォーテーションで囲まれた部分が文字列となります．
Hello, worldを出力してみましょう．

```python
print('Hello, world')
```


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### 四則演算

数値が定義された変数に`+, -, *, /`を作用させると四則演算が出来ます．

```python
a = 3
b = 5
a + b
```

他にも
* 切り捨て除算`//`
* 余り`%`
* 累乗`**`
が使えます．

---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### 関数の定義

一連の処理をまとめてオリジナルの関数を作ることも出来ます．

```python
def add(x, y):
	return x + y
```

---

## Markdown

軽量なマークアップ言語(簡単html)


@box[](1. `Esc + m`またはタブの下にあるプルダウンメニューからMarkdownを選ぶ
2. Markdownセルをクリック
3. 文章を書く
4. `shift+Enter`でレンダリングする
)


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

@snap[west span-40]

```md
ニュートンの運動方程式は
$$
F = ma
$$
である．ここで$F$は力，$m$は質量，$a$は加速度を表す．
```
@snapend

@snap[midpoint span-10]
@fa[arrow-right text-white]
@snapend

@snap[east span-40]
ニュートンの運動方程式は
\[
F = ma
\]
である．ここで$F$は力，$m$は質量，$a$は加速度を表す．
@snapend


---

### 数式について


Jupyterでは数式の記述にMathJaxというライブラリを使っています．MathJaxは$\LaTeX$の文法に準拠しているので，$\LaTeX$を知らない人は

https://home.hiroshima-u.ac.jp/~d172596/markdown.html

に簡単な文法の説明がありますので，参考にしてください

---


## jupyterを使ってノートを取ろう


+ Markdownを使ったメモ書き
+ sympyによる数式処理
+ numpyによる数値計算
+ グラフの可視化

などを駆使して，ノートを取ると便利です．
