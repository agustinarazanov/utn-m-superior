---
layout: post
title: "Números complejos"
date: 2025-02-06 15:23:00 -0300
categories: jekyll update
---

Como veremos en las siguientes unidades, muchos modelos matemáticos de sistemas reales, consisten en ecuaciones en las que aparecen expresiones tales como $$x^2 + 9$$ que sabemos que no tienen raíces en el campo real pero sí las tienen en el conjunto C de los números complejos.

Veremos que además de permitirnos resolver operaciones tales como cálculo de raíces de índice par y radicando negativo, logaritmos de números negativos, y otras, con los números complejos podremos sumar fácilmente funciones senoidales de la misma frecuencia, determinar el tipo de respuesta de un sistema de acuerdo a los polos de su función de transferencia; utilizaremos exponenciales complejas para la Serie y Transformada de Fourier, que son herramientas muy utilizadas en la parte de comunicaciones, análisis de sistemas de control, etc.

En esta unidad, repasaremos el álgebra de los números complejos, es decir veremos como realizar las operaciones: suma, resta, multiplicación, división, potencia, raíces y logaritmos de números complejos.

-   [Esbozo histórico](#esbozo-histórico)
-   [Aplicaciones](#aplicaciones)
-   [Definición de un número complejo](#definición-de-un-número-complejo)

## Esbozo histórico

La primera referencia conocida a raíces cuadradas de números negativos proviene del trabajo de los matemáticos griegos, como Herón de Alejandría en el siglo I antes de Cristo, como resultado de una imposible sección de una pirámide. Los complejos se hicieron más patentes en el Siglo XVI, cuando la búsqueda de fórmulas que dieran las raíces exactas de los polinomios de grados 2 y 3 fueron encontradas por matemáticos italianos como Tartaglia, Cardano. Aunque sólo estaban interesados en las raíces reales de este tipo de ecuaciones, se encontraban con la necesidad de lidiar con raíces de números negativos. El término **imaginario** para estas cantidades fue acuñado por Descartes en el Siglo XVII. La existencia de números complejos no fue completamente aceptada hasta la más abajo mencionada interpretación geométrica que fue descrita por Wessel en 1799, redescubierta algunos años después y popularizada por Gauss. La implementación más formal, con pares de números reales fue dada en el Siglo XIX.

## Aplicaciones

Los números complejos se usan en ingeniería para una descripción adecuada de las señales periódicas variables. Veremos más adelante que cualquier onda sinusoidal, como por ejemplo una corriente o un voltaje de corriente alterna se puede representar como la parte real de una función de variable compleja de la forma: $$ f(t) = z e^{i \omega t} $$ donde $$ \omega $$ representa la frecuencia angular y el número complejo $$z$$ nos da la fase y la amplitud. Ingenieros eléctricos y físicos usan la letra $$j$$ para la unidad imaginaria en vez de $$i$$ que está típicamente destinada a la intensidad de corriente.

El campo complejo es igualmente importante en mecánica cuántica cuya matemática subyacente utiliza Espacios de Hilbert de dimensión infinita sobre **C** ($$ \mathbb{C} $$).

En la relatividad especial y la relatividad general, algunas fórmulas para la métrica del espacio-tiempo son mucho más simples si tomamos el tiempo como una variable imaginaria.

Cuando se estudian las soluciones de las ecuaciones diferenciales lineales con coeficientes constantes, es habitual encontrar primero las raíces (en general complejas) $$\lambda$$ del polinomio característico, lo que permite expresar la solución general del sistema en términos de funciones de base de la forma: $$ f(t) = e^{\lambda t} $$.

Los fractales son diseños artísticos de infinita complejidad. En su versión original, se los define a través de cálculos con números complejos en el plano.

## Definición de un número complejo

<iframe width="560" height="315" src="https://www.youtube.com/embed/IYz-ALBaqTc?si=b1m1WGHv4P5elfS5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

La radicación no es una operación cerrada en el conjunto de los números reales, pues si el radicando es negativo y el índice par, no existe solución, ya que ningún número real elevado a un exponente par da resultado negativo.

Por ello se define:

UNIDAD IMAGINARIA: $$ j=\sqrt{-1} \quad (j\ne\mathbb{R}) $$

Nota: es muy común que en matemática pura se llame $$i$$ a la unidad imaginaria, pero aquí nosotros al igual que en ingeniería electrónica, física y otras especialidades la llamaremos j pues i es la variable con que se representa a la corriente eléctrica.

En base a esta definición, podemos calcular: $$ \sqrt{-x} = j \sqrt{x} $$ con $$ x > 0 \land \sqrt{x} \in \mathbb{R} $$

Ejemplo: $$\sqrt{-4} = 2j$$ y este número es imaginario puro.

NÚMEROS IMAGINARIOS PUROS: son todos los números de la forma $$j b$$ con $$ b \in \mathbb{R} $$.

Nota: a los números imaginarios puros, también se les suele decir solamente imaginarios.

Sumando un número real con un imaginario, obtenemos la forma general de un **Número Complejo**:

NÚMEROS COMPLEJOS: son todos los números de la forma $$ z = a + j b $$ con $$ a,b \in \mathbb{R} $$.

Nota: esta forma de denotar a los complejos se llama FORMA BINOMICA, pero también se los puede escribir en forma de par ordenado de números reales: $$ z = (a; b) $$

Ejemplos de números complejos:

$$
z_1 = 5 - j3 = (5; -3) \quad
z_2 = -1 + j7 = (-1; 7) \quad
z_3 = 4j = (0; 4) \quad
z_4 = -5 = (-5; 0)
$$

PARTE REAL Y PARTE IMAGINARIA DE UN COMPLEJO:

Sea $$ z = a + j b $$ con $$ a, b \in \mathbb{R} \Rightarrow $$ Parte real de z: $$ a = Re(z) $$ Parte imaginaria de z: $$ b = Im (z) $$
