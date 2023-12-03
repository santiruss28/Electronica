Identificación que está normalizada por la Sociedad Americana de Instrumentación ISA (Instrumet Society of America). Es un estándar internacional, que se adecuan generalmente a las diferentes aplicaciones, la cual indica como se debe representar cada TAG de acuerdo a la variable que representa, asociado a este TAG se encuentra una descripción de la variable.

[[SCADA]]

Se debe almacenar la información obtenida a través del driver de telecomunicaciones. Se crea una variable que se denomina TAG asociada con una de las direcciones de memoria del PLC.

## Sintaxis
Es fundamental que cada TAG tenga un nombre único (no pueden existir 2 variables), además es prudente que el nombre indique qué tipo de valor se está tomando y de dónde se lo toma.
La norma ISA define cómo se debe armar un TAG:
![](https://i.imgur.com/Ol40hvV.png)

- **Descripción del sitio**:
Indica el lugar o predio dónde vamos a tomar el dato.
- **Descripción del equipo**
Dentro del predio pueden haber muchos equipos, esta descripción indica de qué equipos se trata.
- **Código de instrumento**
Código que identifica el instrumento. El código de instrumento no indica que tipo de actuador o sensor se trata.
- **Número de Lazo**
Número que identifique el número del lazo de control.
- **Descripción Auxiliar**
Información auxiliar que mejore el entendimiento de la TAG.


Para señales analógicas podemos tener una tabla de definición de señales como la siguiente:

| Tipo           | TAG            | Descripción                | Units                        | Min EU                        | Max EU                        | Min Raw                            | Max Raw                            | LoLo Alarm | Lo Alarm | Hi Alarm | HiHi Alarm | Esclavo | Dir |
| -------------- | -------------- | -------------------------- | ---------------------------- | ----------------------------- | ----------------------------- | ---------------------------------- | ---------------------------------- | ---------- | -------- | -------- | ---------- | ------- | --- |
| Tipio de señal | Nombre del TAG | Descripción de la variable | Tipo de unidades de medición | Valor mínimo de la señal real | Valor máximo de la señal real | Valor mínimo del valor electrónico | Valor mínimo del valor electrónico |            |          |          |            |         |     |
