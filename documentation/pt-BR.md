<!-- ELUCENIA technical documentation · indice-de-choque · pt-BR · no clinical/professional/rights approval -->

# Índice de choque (e modificado)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/indice-de-choque)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Frequência cardíaca

`fc`

bpm · intervalo: 20–250

### Pressão sistólica

`pas`

mmHg · intervalo: 30–300

### Pressão diastólica (para o índice modificado)

`pad`

mmHg · opcional · intervalo: 10–200

## Edição do método

Shock Index/Allgower 1967 FC/PAS e Modified Shock Index/Liu 2012 FC/PAM

## Fórmula documentada

Índice de choque = FC ÷ PAS (normal: 0,5 a 0,7).

Índice de choque modificado = FC ÷ PAM, com PAM = PAD + (PAS − PAD) ÷ 3 (normal: 0,7 a 1,3).

## Limites e população

O índice de choque usa frequência cardíaca dividida pela pressão sistólica; o modificado usa a pressão arterial média. São relações diferentes e não diagnosticam, sozinhas, choque ou necessidade de transfusão. Mutschler 2013 avaliou o índice na chegada à emergência em 21.853 adultos traumatizados; Liu 2012 estudou retrospectivamente 22.161 pacientes de 10 a 100 anos que receberam fluidos intravenosos e excluiu paradas cardiorrespiratórias ressuscitadas sem triagem. Essas coortes não demonstram limites universais para crianças de todas as idades, gestantes ou outras situações. Registre o momento e as condições das medidas; associações de mortalidade hospitalar de uma coorte não são previsão individual automática.

## Referências

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Sem choque (IC < 0,6)


### 2

Choque leve (IC 0,6 a < 1,0)

| Detalhes do resultado | |
| --- | --- |
| Índice de choque modificado (FC/PAM) | 1,18 (0,7 a 1,3) |


### 3

Choque moderado (IC 1,0 a < 1,4)


### 4

Choque grave (IC ≥ 1,4)

