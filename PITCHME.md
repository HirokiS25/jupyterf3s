# ゼロから始めるJupyter Notebook


- 2019年度F3S
- 10月9日
- 広島大学理学研究科
- 坂本弘樹

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
- 機械学習，深層学習，AI(TensorFlow, scikit-learn)

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

## 実際にやってみよう

---

@snap[north-west]
## Jupyter lab

+ Windowsの人 → すべてのプログラム -> anaconda3 -> プロンプトを実行
+ Macの人 → ターミナル
@snapend

@snap[west]
```sh
jupyter lab
```
@snapend

---

![画面の説明](url)

---

@snap[north-west span-100]
## Markdown
@snapend

軽量なマークアップ言語(簡単html)


@css[box](
1. `Esc + m`またはタブの下にあるプルダウンメニューからMarkdownを選ぶ
2. Markdownセルをクリック
3. 文章を書く
4. `shift+Enter`でレンダリングする
)


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


