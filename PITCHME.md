# ゼロから始めるJupyter Notebook

---

## 自己紹介

名前：坂本弘樹
所属：理学研究科素粒子論研究室(D3)


---


## 目次

* jupyterについて
* 

---

## Jupyter is 何？

**Python**をブラウザ上でインタラクティブに動かすためのWebアプリ

---

## Python

+ 最近人気のプログラミング言語
+ 習得が容易
+ 高収入？ [Ref.](https://jp.stanby.com/media/programming_ranking2017/)
+ **ライブラリが豊富**

---

### numpy, scipy

数値計算を高速に行うことが出来るライブラリ(numpy)と科学計算に必要な特殊なモジュールを提供するライブラリ(scipy)



---

### sympy

記号計算用ライブラリ

例えば，

Q. $a x^2 + b x + c = 0$の解を求めよ.
A. $$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

のようなことが出来る．

[2015年センター試験数学IAを全てプログラム(Python)で解く](https://qiita.com/akai_banana/items/b328fe0116d248127a36)

---

### pandas

データ解析に向いたライブラリ

`DataFrame`というオブジェクトを使って
様々なデータ処理を容易に行うことができる

---

ほかにも

- Webアプリ(Django, flask)
- 機械学習，深層学習，AI(TensorFlow, scikit-learn, Kelas)

なんかも出来たりします．

---

@snap[north span-100]
## Jupyterでできること
@snapend

@snap[fragment left]
ex.) 

1. 計算結果をグラフにプロットしてその結果をメモする

2. 大量のデータの中から必要なところだけ抜き出してその特徴量の可視化を行う
@snapend

---
![example](url)

---

## python入門

---

@snap[north-west]
## Jupyter lab

+ Windowsの人 → すべてのプログラム -> anaconda3 -> プロンプトを実行
+ Macの人 → ターミナル
@snapend

@snap[west span-100]
```sh
jupyter lab
```
@snapend

---

![画面の説明](url)

---

### Hello, world

pythonではクォーテーションかダブルクォーテーションで囲まれた部分が文字列となります．
Hello, worldを出力してみましょう．

```python
print('Hello, world')
```

---

### 四則演算

`+, -, *, /`

```python
a = 3
b = 5
a + b
```

---

### 関数の定義


```python
def add(x, y):
	return x + y
```

---

@snap[north-west span-100]
## Markdown
@snapend

軽量なマークアップ言語(簡単html)


<div class=box>
1. `Esc + m`またはタブの下にあるプルダウンメニューからMarkdownを選ぶ
2. Markdownセルをクリック
3. 文章を書く
4. `shift+Enter`でレンダリングする
</div>


---?color=linear-gradient(to left, #56ccf2, #2f80ed)

@snap[west span-40]
コード
```md
ニュートンの運動方程式は
$$
F = ma
$$
である．ここで$F$は力，$m$は質量，$a$は加速度を表す．
```
@snapend

@snap[midpoint span-10]
@fa[code-branch black]
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
