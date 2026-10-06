<!-- ELUCENIA technical documentation · indice-de-choque · en · no clinical/professional/rights approval -->

# Shock index (and modified shock index)

[conditions, sources and permissions](https://elucenia.org/en/tools/indice-de-choque)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Heart rate

`fc`

bpm · range: 20–250

### Systolic blood pressure

`pas`

mmHg · range: 30–300

### Diastolic pressure (for the modified index)

`pad`

mmHg · optional · range: 10–200

## Method edition

Shock Index/Allgöwer 1967 HR/SBP and Modified Shock Index/Liu 2012 HR/MAP

## Documented formula

Shock index = HR ÷ SBP (normal: 0.5–0.7).

Modified shock index = HR ÷ MAP, where MAP = DBP + (SBP − DBP) ÷ 3 (normal: 0.7–1.3).

## Limits and population

Shock index uses heart rate divided by systolic pressure; modified shock index uses mean arterial pressure. These are different ratios and do not by themselves diagnose shock or a need for transfusion. Mutschler 2013 assessed the index on emergency-department arrival in 21,853 adults with trauma; Liu 2012 retrospectively studied 22,161 patients aged 10–100 who received intravenous fluids and excluded resuscitated cardiorespiratory arrests without triage. These cohorts do not establish universal cutoffs for children of all ages, pregnant people or other situations. Record the timing and measurement conditions; cohort associations with in-hospital mortality are not automatic individual predictions.

## References

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

No shock (SI < 0.6)


### 2

Mild shock (SI 0.6 to < 1.0)

| Result details | |
| --- | --- |
| Modified shock index (HR/MAP) | 1.18 (0.7 to 1.3) |


### 3

Moderate shock (SI 1.0 to < 1.4)


### 4

Severe shock (SI ≥ 1.4)

