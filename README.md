## Maxwell eqs.

<!--
**hikarukitamura-0/hikarukitamura-0** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<img src="https://latex.codecogs.com/png.latex?\color{red}\nabla\cdot\mathbf{E}=\frac{\rho}{\varepsilon_0}" alt="Maxwell 1" />
<img src="https://latex.codecogs.com/png.latex?\color{red}\nabla\cdot\mathbf{B}=0" alt="Maxwell 2" />
<img src="https://latex.codecogs.com/png.latex?\color{red}\nabla\times\mathbf{E}=-\frac{\partial\mathbf{B}}{\partial%20t}" alt="Maxwell 3" />
<img src="https://latex.codecogs.com/png.latex?\color{red}\nabla\times\mathbf{B}=\mu_0\mathbf{J}+\mu_0\varepsilon_0\frac{\partial\mathbf{E}}{\partial%20t}" alt="Maxwell 4" />

## プロフィール

<p float="left">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=hikarukitamura-0&show_icons=true&locale=en&layout=compact&theme=radical&cache_seconds=0&rand=1" width="350" />
  <img src="https://github-readme-stats.vercel.app/api?username=hikarukitamura-0&show_icons=true&show_icons=true&theme=radical&cache_seconds=0&rand=1" width="450" />
</p>

物理数学　→　電磁気学　→　特殊相対性理論　→　解析力学 ★今ココ★　→　量子力学　→　一般相対性理論　→　場の量子論　→　弦理論（ボゾン的？）　→　超弦理論　→　M理論　→→→→→　Theory of Everything...

### 自己紹介
舞鶴高専 電気情報工学科二年の北村光瑠と申します。
プログラミングはそこまで得意ではありません。

### 好きなもの
<br>
物理が非常に好きで、2026年第73回 応用物理学会に現地参加予定です。
<br>
とくに量子重力と、宇宙膨張による時間並進対称性の破れによる宇宙全体の保存則の成立について興味があります。
<br>
あと、好きな食べ物はラーメンです。



# 考察：ハミルトニアンの時間依存性と宇宙を内包する上位系の仮定

## 1. 着想のきっかけ：ポアンカレ・カルタン積分のシミュレーション
数値シミュレーションにおいて、相流が時間変化する系、すなわち**ハミルトニアンが時刻 $t$ に明示的に依存して変化する系**でポアンカレ・カルタン積分が成立するかを検証しようと考えたことが始まりです。

> **ポアンカレ・カルタン積分とは**
> 相空間に時間軸を加えた「$2n+1$次元相空間」における不変量です。通常のポアンカレ不変量 $\oint p dq$ を拡張した $\oint (p dq - H dt)$ で表されます。ハミルトニアン $H$ が時間に依存する場合でも、この積分値は相空間内の軌道の円筒に沿って保存されます。

この「時間依存するハミルトニアン」を具体的にどう記述するか検討する中で、**二重振り子**の系に注目しました。

## 2. 二重振り子のモデル化と「開いた系」の視点
二重振り子の「下側の振り子」のみを観測対象とすれば、それは外部（上の振り子）とエネルギーをやり取りする「開いた系」として記述されます。
* **下側の振り子：** 単体で見ればエネルギーが変動し、ハミルトニアンが時間依存する。
* **系全体：** 上下の振り子を合わせた全体系では、時間並進対称性が保たれ、エネルギーは保存される。

この性質から、「エネルギーが変動する時間依存系」は、より大きな保存系の一部（部分系）として捉え直せるという着想を得ました。



## 3. 宇宙論への応用：局所的時間並進対称性の破れ
現在、宇宙膨張に伴う赤方偏移などの現象が実際に観測されています。一般相対性理論の枠組みでは、膨張宇宙（FLRW計量）は時間並進対称性が破れており、ネーターの定理に基づけば、宇宙全体のエネルギー保存則は厳密には成立しません。

ここで、我々の観測可能な宇宙を二重振り子の「下側の振り子」のような**開いた系**と仮定します。
* **仮説：** 我々の宇宙を内包する「より大きな集合（高次元バルク空間など？）」を想定し、その全体系において時間並進対称性が保たれていると考える。
* **展望：** 外部系との相互作用を、FLRW計量等を拡張し計算できれば、宇宙のエネルギー変動を全体系の保存則の一部として正当化できるのではないか。



## 4. 課題：自由度の増大について
宇宙をさらに大きな系の一部と見なせば、論理的な保存則の整合性は確保できます。しかし、このアプローチは**「理論の自由度が高すぎて、何でも説明できてしまう」**という懸念があります。
モデルに物理的な実効性を持たせるためには、この自由度を制限するような観測的な制約、あるいは数学的な境界条件をどう設定すべきかが重要な課題であると考えています。


この考え方に近い実際の学説として、ブレーンワールドやADM形式、弦理論における余剰次元のカラビヤウ多様体による丸め込みの方法の候補が多すぎること（ランドスケープ問題）などがあるらしいです。

---
※ラグランジアン $L(q, \dot{q}, t)$ が時間に依存する場合、ルジャンドル変換 $H = \sum p\dot{q} - L$ を通じて、ハミルトニアン $H$ も必ず時間依存します。


