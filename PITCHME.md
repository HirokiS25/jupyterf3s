# ゼロから始めるJupyter Notebook

---

## 自己紹介

名前：坂本弘樹

所属：理学研究科素粒子論研究室(D3)


---


## 目次

* Jupyterについて
* python入門
* Jupyterでノートを取る


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

## Jupyter is 何？

**Python**をブラウザ上でインタラクティブに動かすためのWebアプリ


Jupyter labを起動するには

+ Windowsの人 @fa[right-arrow] すべてのプログラム @fa[right-arrow] anaconda3 @fa[right-arrow] プロンプトを実行
+ Macの人 @fa[right-arrow] ターミナル

を立ち上げたら`jupyter lab`と入力して実行してください．


Jupyterをインストール出来てない人はオンラインで使える
google colabolatoryを試してみましょう(要googleアカウント)

---

## Python

@ul
+ 最近人気のプログラミング言語
+ オープンソース
+ 習得が容易
+ 書きやすい
+ 汎用性が高い
+ 高収入(?) [Ref.](https://jp.stanby.com/media/programming_ranking2017/)
+ ライブラリが豊富
@ulend

---

## どんなことが出来るのか

@ul
* Web開発
* AI
* 機械学習
* データ解析
* 数値計算
* 記号計算
* データの可視化
* など

google, youtube, dropbox, instagramなどはPythonで作られている
@ulend

---

## ライブラリの紹介(一部)

* `numpy`: 数値計算を高速に行うことが出来るライブラリ
* `scipy`: 科学計算に必要な特殊なモジュールを提供するライブラリ
* `sympy`: 記号計算用ライブラリ
* `pandas`: データ解析をするためのライブラリ

ほかにも

- `Django, flask`: Web開発のためのフレームワーク
- `TensorFlow, scikit-learn, Kelas`: 機械学習，深層学習，AI

などライブラリを使うことによって，様々なアプリケーションを作れる！

Note:

例えば，

@snap[text-06 span-100]
Q. $a x^2 + b x + c = 0$の解を求めよ. 
A. $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

のようなことが出来る．

参考：[2015年センター試験数学IAを全てプログラム(Python)で解く](https://qiita.com/akai_banana/items/b328fe0116d248127a36)
@snapend


---

## Jupyterの使い方の例

Jupyterの特徴： 

* セルごとにPythonのコードが実行でき，その結果をノートブック上に保存できる．
* Markdownを使って見出しや表などが簡単に表示できる

@snap[fragment]
**Pythonを書いて得られたデータやグラフを，ノートのようにまとめることができる**
@snapend

---

![gamen](https://user-images.githubusercontent.com/32427720/65029837-64fbbb00-d979-11e9-8e63-1f28001c4dd4.gif)

---

## python入門

---

![jy_window_new](https://user-images.githubusercontent.com/32427720/66415236-1b613600-ea36-11e9-9dab-6f4faebb2cf1.png)


---


## jupyterを使ってノートを取ろう


+ Markdownを使ったメモ書き
+ sympyによる数式処理
+ numpyによる数値計算
+ グラフの可視化

などを駆使して，ノートを取ると便利です．

---

## Markdown

軽量なマークアップ言語(htmlの簡単varsion)


1. `Esc + m`またはタブの下にあるプルダウンメニューからMarkdownを選ぶ
2. Markdownセルをクリック
3. 文章を書く
4. `shift+Enter`でレンダリングする


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

```md
ニュートンの運動方程式は
$$
F = ma
$$
である．ここで$F$は力，$m$は質量，$a$は加速度を表す．
```

---

ニュートンの運動方程式は
$$
F = ma
$$
である．ここで$F$は力，$m$は質量，$a$は加速度を表す．


---

### 数式について


Jupyterでは数式の記述にMathJaxというライブラリを使っています．MathJaxは$\LaTeX$の文法に準拠しているので，$\LaTeX$を知らない人は

https://home.hiroshima-u.ac.jp/~d172596/markdown.html

に簡単な文法の説明がありますので，参考にしてください

