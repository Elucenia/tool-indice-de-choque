<!-- ELUCENIA technical documentation · indice-de-choque · zh · no clinical/professional/rights approval -->

# 休克指数（及改良值）

[条件、来源与许可](https://elucenia.org/zh/tools/indice-de-choque)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 心率

`fc`

次心搏/分钟 · 范围: 20–250

### 收缩压

`pas`

mmHg · 范围: 30–300

### 舒张压（用于改良指数）

`pad`

mmHg · 选填 · 范围: 10–200

## 方法版本

休克指数/Allgöwer 1967 HR/SBP及改良指数/Liu 2012 HR/MAP

## 已记录的公式

休克指数 = HR÷SBP（正常0.5–0.7）。

改良休克指数 = HR÷MAP，其中MAP=DBP+(SBP−DBP)÷3（正常0.7–1.3）。

## 限制与适用人群

休克指数为心率除以收缩压；改良指数使用平均动脉压。两者是不同的比值，不能单独诊断休克或输血需要。Mutschler2013评估了21,853名成年创伤患者到达急诊时的指数；Liu2012回顾性研究了22,161名接受静脉补液的10至100岁患者，并排除了未分诊即复苏的心肺骤停病例。这些队列不能证明对所有年龄儿童、孕妇或其他情境均适用的阈值。请记录测量时间与条件；队列中与院内死亡的关联不能自动预测个人结局。

## 参考文献

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

无休克（IC < 0.6）


### 2

轻度休克（IC 0.6 至 < 1.0）

| 结果详情 | |
| --- | --- |
| 修正休克指数（FC/PAM） | 1.18（0.7 至 1.3） |


### 3

中度休克（IC 1.0 至 < 1.4）


### 4

重度休克（IC ≥ 1.4）

