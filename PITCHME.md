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

![jy_window_new](https://user-images.githubusercontent.com/32427720/66415236-1b613600-ea36-11e9-9dab-6f4faebb2cf1.png)

---

## python入門

---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### Hello, World

pythonでは`var = 12`のようにして変数を与えます．

* 数値(int, float, complex)
* 配列(list, tuple, dict)
* 文字列(str)

クォーテーションかダブルクォーテーションで囲まれた部分が文字列となります．

Hello, Worldを出力してみましょう．

---

```python
char = 'Hello, World'
print(char)
# Hello, World
```


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### 四則演算

数値型の変数に対して四則演算`+, -, *, /`が定義されています．

```python
a = 3
b = 5
a + b
# 8
```

他にも
* 切り捨て除算 `//`
* 余り `%`
* 累乗 `**`
が使えます．


---?color=linear-gradient(to top, #6dd5ed, #2193b0)

### 配列

複数のデータをカンマで区切ってひとまとめにしたものを配列といいます．

* `list`: [a, b, c]
* `tuple`: (a, b, c)
* `dict`: {"key1": value1, "key2": value2}

---?color=linear-gradient(to top, #6dd5ed, #2193b0)

```py
a = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"]
a  # ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday']
```

リストやタプルの要素を取り出すには
```py
b = (1, 10, 100, 1000, 10000)
b[3]  # 1000
```

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
