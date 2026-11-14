### Kohei Shintani, Ph.D.

自動車工学と機械学習の橋渡しを研究しています。<br>
**生成AIによる3D設計 ・ 構造最適化 ・ ベイズ能動学習 ・ 低次元サロゲートモデル**<br>
Research bridging automotive engineering and machine learning.<br>
Generative-AI 3D design, structural optimization, Bayesian active learning, and reduced-order surrogate models.

**Site:** [ks278810.github.io/website](https://ks278810.github.io/website/) ·
**LinkedIn:** [kohei-shintani-9b20a6175](https://www.linkedin.com/in/kohei-shintani-9b20a6175/) ·
**ResearchGate:** [Kohei-Shintani](https://www.researchgate.net/profile/Kohei-Shintani)

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/robotools-band-dark.png"><img src="assets/robotools-band.png" width="880" alt="RoboTools"></picture></p>

公開中の5つは、ブラウザだけで動きます。データのアップロードは不要です。<br>
<sub>The five public tools run only in your browser. No data upload is needed.</sub>

<table width="100%">
<tr>
<td align="center" valign="top" width="50%">
<a href="https://ks278810.github.io/BayesRobo/"><img src="assets/bayesrobo.gif" width="390" alt="BayesRobo の操作画面"></a><br>
<b><a href="https://ks278810.github.io/BayesRobo/">BayesRobo</a></b><br>
<b>次に試す条件を、ベイズ最適化で提案する。</b><br>
<sub>Suggests what to try next.</sub>
<p align="left">CSVを渡すと、ガウス過程で結果を予測するモデルをその場で学習します。最適値を追うか、データの少ない領域を埋めるかを選ぶと、次に実験や計算をする条件を提案します。<br>
<sub>Drop a CSV and it fits a Gaussian-process surrogate in the browser. Choose between chasing the optimum and filling sparse regions, and it proposes the next point to run.</sub></p>
</td>
<td align="center" valign="top" width="50%">
<a href="https://ks278810.github.io/surrobot/"><img src="assets/surrobot.gif" width="390" alt="SurRobo の操作画面"></a><br>
<b><a href="https://ks278810.github.io/surrobot/">SurRobo</a></b><br>
<b>予測モデルを自動で作り、勝者を選ぶ。</b><br>
<sub>Builds the models and picks the winner.</sub>
<p align="left">CSVをドロップすると、線形回帰、LightGBM、ガウス過程、ニューラルネットを自動で比べ、最も精度の高いモデルを選びます。特徴量の重要度と予測結果を確認でき、モデルは持ち帰れます。<br>
<sub>Drop a CSV and it compares linear regression, LightGBM, Gaussian process and a neural net, then picks the most accurate. Feature importance and predictions are shown, and the model can be downloaded.</sub></p>
</td>
</tr>
<tr>
<td align="center" valign="top" width="50%">
<a href="https://ks278810.github.io/surrobo-s/"><img src="assets/surrobo-s.gif" width="390" alt="SurRobo-S の操作画面"></a><br>
<b><a href="https://ks278810.github.io/surrobo-s/">SurRobo-S</a></b><br>
<b>データの裏にある式を、見つけ出す。</b><br>
<sub>Finds the formula behind your data.</sub>
<p align="left">CSVをドロップして目的の列を選ぶと、列どうしの関係を表す数式を探します。見つかった式は、Python、C、Excel のコードで持ち帰れます。<br>
<sub>Drop a CSV and pick the target column, and it searches for a formula that fits. The formula can be taken away as Python, C or Excel code.</sub></p>
</td>
<td align="center" valign="top" width="50%">
<a href="https://ks278810.github.io/adrobo/"><img src="assets/adrobo.gif" width="390" alt="AdRobo の操作画面"></a><br>
<b><a href="https://ks278810.github.io/adrobo/">AdRobo</a></b><br>
<b>時系列データの「いつもと違う」区間を、見つける。</b><br>
<sub>Spots unusual stretches in your time series.</sub>
<p align="left">CSVをドロップして正常な区間を選ぶと、時系列の中から異常な区間を探します。TeVAE、ScatterAD など5つの手法を比べられ、異常の原因になった列も確認できます。<br>
<sub>Drop a CSV and mark the normal stretch, and it finds the anomalous ones. Five methods, including TeVAE and ScatterAD, can be compared, and the columns behind each anomaly are shown.</sub></p>
</td>
</tr>
<tr>
<td align="center" valign="top" width="50%">
<a href="https://ks278810.github.io/sigrobo/"><img src="assets/sigrobo.gif" width="390" alt="SigRobo の操作画面"></a><br>
<b><a href="https://ks278810.github.io/sigrobo/">SigRobo</a></b><br>
<b>時系列の予測を、同じ条件で比べる。</b><br>
<sub>Compares forecasting models under the same conditions.</sub>
<p align="left">CSVをドロップして予測したい列を選ぶと、複数のモデルを同じ条件で学習して比べます。単純な予測との比較と点検まで自動で行い、同時刻の系列、先の予測、系列から1つの値、の3つの課題に対応します。<br>
<sub>Drop a CSV and pick the target, and it trains several models under the same conditions and compares them. It checks against a naive forecast and supports three tasks: sequence to sequence, forecasting, and sequence to scalar.</sub></p>
</td>
<td align="center" valign="top" width="50%">
<img src="assets/surrobo-d.gif" width="390" alt="SurRobo-D の操作画面"><br>
<b>SurRobo-D</b><br>
<b>作った予測モデルを、exe 1つで渡す。</b><br>
<sub>Ships your model as a single exe.</sub>
<p align="left">CSVから予測モデルを学習し、蒸留、つまり小さなモデルへの写し取りで軽くします。仕上がったモデルは、exe 1つにして渡せます。<br>
<sub>It trains a prediction model from a CSV and slims it down by distillation, which copies the model into a smaller one. The finished model ships as a single exe.</sub></p>
</td>
</tr>
</table>

<p align="center"><sub>SurRobo-D は GPU が必要なため、公開デモはありません。 / SurRobo-D needs a GPU, so there is no public demo.</sub></p>

#### 研究 / Research

**生成AIによる3D設計 / Generative-AI 3D design**

- [VehicleSDF](https://arxiv.org/abs/2410.18986) — 制約つきの工学設計のための3D生成モデル。NeurIPS 2024 ワークショップ<br>A 3D generative model for constrained engineering design. NeurIPS 2024 workshop.
- WheelSDF — ホイール設計のための3D形状生成。ASME IDETC-CIE 2025<br>Implicit-representation 3D shape generation for wheel design.

**構造最適化 / Structural optimization**

- Data-driven topology optimization using a multitask conditional variational autoencoder with persistent homology<br>*Structural and Multidisciplinary Optimization*, 2024<br>データ駆動のトポロジー最適化。マルチタスク条件付きVAEと永続ホモロジー。
- Multimaterial homologous topology optimization of large telescope structure under multiple elevation conditions<br>*Structural and Multidisciplinary Optimization*, 2024<br>大型望遠鏡構造の、複数の仰角条件でのマルチマテリアルなトポロジー最適化。
- Robust topology optimization of multi-material lattice structures under material and load uncertainties<br>*Frontiers of Mechanical Engineering*, 2019<br>材料と荷重のばらつきに強い、多材料格子構造のロバストトポロジー最適化。

ResearchGate の登録数で60本、特許9件。全リストは [Site](https://ks278810.github.io/website/#research) の「すべて表示」にあります。<br>
<sub>60 papers as registered on ResearchGate, and 9 patents. The full list is on the site.</sub>

#### ResearchRobo ・ 調べものを、出典つきのレポートに
<sub>Research, turned into a sourced report.</sub><br>

<a href="https://ks278810.github.io/research-robo/"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/researchrobo-dark.png"><img src="assets/researchrobo.png" width="880" alt="ResearchRobo エンジニアのためのベンチマーク調査ツール"></picture></a>

> 調べたいことを書くだけ。AIチャットのDeep Researchを、出典と突き合わせて検査したレポートに変える無料のプロンプトキット。登録不要、CC BY 4.0。原資料の再確認まではしないため、重要な数値は原資料でも確かめてください。別にAIチャットの有料プランが必要です。
>
> Just write your research question. A free prompt kit that turns AI chat Deep Research into a report checked against its sources. No sign-up, CC BY 4.0. It does not re-open the original sources, so check key numbers there. A paid AI chat plan is needed separately.

[ResearchRobo を開く / Open ResearchRobo](https://ks278810.github.io/research-robo/)

#### その他のツール / Other tools

- **[FMUTuner](https://ks278810.github.io/FMUTuner/)** — FMUのパラメータを、試験データに合わせて調整。公開デモは、記録済みの1回分の再生です。<br>Tunes FMU parameters to test data. The public demo replays one recorded fit.
- **[ClearCut](https://github.com/KS278810/ClearCut)** — 動画と画像の背景を除去。<br>Removes the background from video and images.
