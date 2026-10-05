<!-- ELUCENIA technical documentation · indice-de-choque · es · no clinical/professional/rights approval -->

# Índice de choque (y modificado)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/indice-de-choque)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Frecuencia cardíaca

`fc`

bpm · intervalo: 20–250

### Presión sistólica

`pas`

mmHg · intervalo: 30–300

### Presión diastólica (para el índice modificado)

`pad`

mmHg · opcional · intervalo: 10–200

## Edición del método

Shock Index/Allgöwer 1967 FC/PAS y índice modificado/Liu 2012 FC/PAM

## Fórmula documentada

Índice de choque = FC ÷ PAS (normal: 0,5–0,7).

Índice de choque modificado = FC ÷ PAM, con PAM = PAD + (PAS − PAD) ÷ 3 (normal: 0,7–1,3).

## Límites y población

El índice de choque usa frecuencia cardíaca dividida por presión sistólica; el modificado usa presión arterial media. Son relaciones distintas y no diagnostican por sí solas choque ni necesidad de transfusión. Mutschler 2013 evaluó el índice al llegar a urgencias en 21.853 adultos traumatizados; Liu 2012 estudió retrospectivamente 22.161 pacientes de 10 a 100 años que recibieron fluidos intravenosos y excluyó paradas cardiorrespiratorias reanimadas sin triaje. Estas cohortes no demuestran límites universales para niños de todas las edades, gestantes u otras situaciones. Registre el momento y las condiciones de medición; las asociaciones de mortalidad hospitalaria de una cohorte no son predicciones individuales automáticas.

## Referencias

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
