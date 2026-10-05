<!-- ELUCENIA technical documentation · indice-de-choque · ja · no clinical/professional/rights approval -->

# ショック指数（修正版を含む）

[条件・出典・許諾](https://elucenia.org/ja/tools/indice-de-choque)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 心拍数

`fc`

拍/分 · 範囲: 20–250

### 収縮期血圧

`pas`

mmHg · 範囲: 30–300

### 拡張期血圧（修正指数用）

`pad`

mmHg · 任意 · 範囲: 10–200

## 方法の版

ショック指数/Allgöwer 1967 HR/SBP、修正指数/Liu 2012 HR/MAP

## 記載された計算式

ショック指数 = HR÷SBP（正常0.5–0.7）。

修正ショック指数 = HR÷MAP、MAP=DBP+(SBP−DBP)÷3（正常0.7–1.3）。

## 限界・対象集団

ショック指数は心拍数を収縮期血圧で割った値で、修正指数は平均動脈圧を使います。異なる比であり、それだけでショックや輸血の必要性を診断しません。Mutschler2013は成人外傷患者21,853人の救急到着時の指数を評価しました。Liu2012は静脈内輸液を受けた10–100歳の22,161人を後ろ向きに調べ、トリアージなしで蘇生された心肺停止例を除外しました。これらのコホートは、全年齢の小児、妊婦、その他の状況での普遍的な閾値を示しません。測定時点と条件を記録してください。コホート内の院内死亡との関連は、個人の自動的予測ではありません。

## 参考文献

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
