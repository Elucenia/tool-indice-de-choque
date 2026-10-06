<!-- ELUCENIA technical documentation · indice-de-choque · fr · no clinical/professional/rights approval -->

# Indice de choc (et indice modifié)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/indice-de-choque)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Fréquence cardiaque

`fc`

bpm · intervalle: 20–250

### Pression systolique

`pas`

mmHg · intervalle: 30–300

### Pression diastolique (pour l’indice modifié)

`pad`

mmHg · facultatif · intervalle: 10–200

## Édition de la méthode

Shock Index/Allgöwer 1967 FC/PAS et indice modifié/Liu 2012 FC/PAM

## Formule documentée

Indice de choc = FC ÷ PAS (normal : 0,5–0,7).

Indice de choc modifié = FC ÷ PAM, avec PAM = PAD + (PAS − PAD) ÷ 3 (normal : 0,7–1,3).

## Limites et population

L’indice de choc utilise la fréquence cardiaque divisée par la pression systolique ; sa version modifiée utilise la pression artérielle moyenne. Ces rapports sont différents et ne diagnostiquent pas à eux seuls un choc ou un besoin de transfusion. Mutschler 2013 a évalué l’indice à l’arrivée aux urgences chez 21 853 adultes traumatisés ; Liu 2012 a étudié rétrospectivement 22 161 patients de 10 à 100 ans ayant reçu des liquides intraveineux et exclu les arrêts cardiorespiratoires réanimés sans triage. Ces cohortes ne démontrent pas de seuils universels pour tous les âges pédiatriques, la grossesse ou d’autres situations. Consignez le moment et les conditions des mesures ; les associations à la mortalité hospitalière d’une cohorte ne sont pas des prévisions individuelles automatiques.

## Références

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Pas de choc (IC < 0,6)


### 2

Choc léger (IC 0,6 à < 1,0)

| Détails du résultat | |
| --- | --- |
| Indice de choc modifié (FC/PAM) | 1,18 (0,7 à 1,3) |


### 3

Choc modéré (IC 1,0 à < 1,4)


### 4

Choc grave (IC ≥ 1,4)

