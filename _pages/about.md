---
layout: single
title: "Presentación"
permalink: /
author_profile: true
---
### Sobre mí

<p style="text-align: justify;">
Mi formación se ha desarrollado en dos trayectorias en paralelo, Física y Matemáticas, y esa doble base ha guiado mi trabajo académico y docente. En Física, mis intereses evolucionaron hacia el estudio de materiales, nanomateriales y, finalmente, hacia la espectroscopía como una herramienta central para comprender sistemas complejos. Durante este recorrido trabajé en el Instituto de Materiales en la simulación de nanoestructuras mediante métodos ab initio, y más adelante en el Instituto de Ciencias Aplicadas y Tecnología, donde me enfoqué en espectroscopía infrarroja y Raman, así como en el procesamiento de señales mediante métodos estadísticos e inteligencia artificial. En paralelo, mi formación matemática me llevó hacia la estadística y las finanzas cuantitativas, área que complementé con certificaciones especializadas en el NYIF y los exámenes del GARP y CFA además de experiencia práctica. Además, durante una etapa profesional trabajé como científico de datos y, por un breve periodo, como consultor financiero, experiencias que han contribuido de manera directa a mi acumulación de experiencia en el área cuantitativa. Actualmente continúo ampliando mi formación académica y científica, mientras asumo con seriedad mi responsabilidad docente y administro algunas carteras de inversión como parte de mi práctica aplicada.
</p>


### ¿Tienes curiosidad de saber lo que es el DFT?

<p style="text-align: justify;">
La teoría del funcional de la densidad (Density Functional Theory, DFT) surge como una alternativa al tratamiento directo del problema cuántico de muchos electrones. En un sistema formado por \(N\) electrones bajo el potencial de los núcleos, la descripción completa está dada por la ecuación de Schrödinger estacionaria:
</p>
$$
\hat H \Psi(\mathbf r_1,\mathbf r_2,\dots,\mathbf r_N)
=
E
\Psi(\mathbf r_1,\mathbf r_2,\dots,\mathbf r_N),
$$
<p style="text-align: justify;">
Donde el Hamiltoniano electrónico puede escribirse como:
</p>
$$
\hat H
=
\sum_{i=1}^{N}
\left(
-\frac{\hbar^2}{2m}\nabla_i^2
+
V(\mathbf r_i)
\right)
+
\sum_{i<j}
\frac{e^2}{|\mathbf r_i-\mathbf r_j|}
$$
<p style="text-align: justify;">
La función de onda \(\Psi\) depende de \(3N\) coordenadas espaciales, lo que hace que el problema crezca exponencialmente con el número de partículas y se vuelva intratable incluso para sistemas relativamente pequeños. La idea fundamental de la teoría del funcional de la densidad consiste en reemplazar esta descripción en términos de la función de onda por una descripción basada únicamente en la densidad electrónica:
</p>
$$
n(\mathbf r)
=
N
\int
|\Psi(\mathbf r,\mathbf r_2,\dots,\mathbf r_N)|^2
\, d\mathbf r_2 \dots d\mathbf r_N
$$
<p style="text-align: justify;">
la cual depende solamente de tres variables espaciales. Los teoremas fundamentales de Hohenberg y Kohn establecen que la densidad electrónica del estado fundamental determina de manera única el potencial externo \(V(\mathbf r)\) y, por lo tanto, todas las propiedades físicas del sistema. En consecuencia, la energía total puede escribirse como un funcional de la densidad:
</p>
$$
E[n]
=
T[n]
+
U[n]
+
\int
V(\mathbf r)\,n(\mathbf r)\,d^3r
$$
<p style="text-align: justify;">
donde \(T[n]\) representa la energía cinética electrónica y \(U[n]\) la interacción entre electrones. El estado fundamental del sistema se obtiene minimizando este funcional de energía con respecto a todas las densidades admisibles. En la práctica, la formulación más utilizada es la propuesta por Kohn y Sham, que introduce un sistema ficticio de electrones no interactuantes cuya densidad reproduce exactamente la densidad del sistema real. Esto conduce a las ecuaciones de Kohn–Sham:
</p>
$$
\left[
-\frac{\hbar^2}{2m}\nabla^2
+
V_{\text{eff}}(\mathbf r)
\right]
\varphi_i(\mathbf r)
=
\varepsilon_i
\varphi_i(\mathbf r)
$$
<p style="text-align: justify;">
Donde la densidad se reconstruye como:
</p>
$$
n(\mathbf r)
=
\sum_i |\varphi_i(\mathbf r)|^2
$$
<p style="text-align: justify;">
Y el potencial efectivo incluye el potencial externo, el potencial de Hartree y el término de intercambio-correlación \(V_{\text{xc}}\), que contiene los efectos cuánticos de interacción electrónica. La determinación aproximada de este funcional de intercambio-correlación constituye el principal desafío de la teoría, pero también la razón de su enorme éxito como herramienta computacional para estudiar la estructura electrónica de átomos, moléculas, sólidos y nanoestructuras. De esta manera, DFT permite transformar el complejo problema de muchos cuerpos en un esquema computacionalmente manejable basado en la densidad electrónica como variable fundamental.
</p>



### ¿Te interesa la Espectroscopía?



<p style="text-align: justify;">
La espectroscopía constituye una de las herramientas experimentales fundamentales para investigar la estructura y la dinámica de la materia. En términos generales su objetivo es estudiar la interacción entre la radiación electromagnética y los sistemas físicos con el fin de obtener información sobre su composición, estructura molecular, estados electrónicos o dinámicas vibracionales. Desde el punto de vista cuántico esta interacción se describe mediante el Hamiltoniano:
</p>
$$
\hat H = \hat H_0 + \hat H_{\text{int}}
$$
<p style="text-align: justify;">
Donde \( \hat H_0 \) describe el sistema en ausencia de radiación y \( \hat H_{\text{int}} \) representa el acoplamiento entre el campo electromagnético y el sistema material. En el régimen dipolar eléctrico este término de interacción puede escribirse como:
</p>
$$
\hat H_{\text{int}} = - \boldsymbol{\mu} \cdot \mathbf{E}(t),
$$
<p style="text-align: justify;">
Donde \( \boldsymbol{\mu} \) es el operador de momento dipolar molecular y \( \mathbf{E}(t) \) el campo eléctrico incidente. La absorción o dispersión de radiación ocurre cuando la energía del campo electromagnético coincide con la diferencia entre niveles de energía del sistema. Esta condición puede expresarse como:
</p>
$$
h\nu = E_f - E_i
$$
<p style="text-align: justify;">
En el caso de la espectroscopía vibracional estos niveles corresponden a modos vibracionales asociados a enlaces químicos. Para una aproximación armónica simple las frecuencias vibracionales de una molécula pueden describirse mediante:
</p>
$$
\nu = \frac{1}{2\pi}\sqrt{\frac{k}{\mu}}
$$
<p style="text-align: justify;">
Donde \(k\) representa la constante de fuerza del enlace y \(\mu\) la masa reducida del sistema vibracional. Estas vibraciones constituyen una especie de huella molecular que permite identificar estructuras químicas y estudiar propiedades estructurales de materiales. La espectroscopía infrarroja se basa en la absorción de radiación cuando un modo vibracional produce un cambio en el momento dipolar de la molécula. Una transición vibracional será activa en el espectro infrarrojo cuando se cumple la condición
</p>
$$
\frac{\partial \mu}{\partial Q} \neq 0
$$
<p style="text-align: justify;">
Donde \(Q\) representa la coordenada normal de vibración. Como consecuencia la espectroscopía infrarroja resulta particularmente sensible a enlaces polares y a variaciones en la distribución de carga electrónica dentro de una molécula o un sólido. La espectroscopía Raman se basa en un mecanismo distinto relacionado con la dispersión inelástica de la luz incidente conocida como efecto Raman. Durante este proceso la radiación interactúa con la polarizabilidad electrónica del sistema y produce fotones dispersados cuya frecuencia difiere de la frecuencia incidente. Un modo vibracional será activo en Raman cuando se cumple:
</p>
$$
\frac{\partial \alpha}{\partial Q} \neq 0
$$
<p style="text-align: justify;">
Donde \(\alpha\) representa el tensor de polarizabilidad molecular. Como resultado Raman es especialmente sensible a vibraciones asociadas a cambios en la deformación electrónica de la molécula o del cristal.
</p>
<p style="text-align: justify;">
Debido a estas diferencias en los mecanismos físicos subyacentes las espectroscopías infrarroja y Raman se consideran técnicas complementarias. La espectroscopía infrarroja detecta vibraciones que implican cambios en el momento dipolar mientras que Raman revela aquellas asociadas a cambios en la polarizabilidad electrónica. La combinación de ambas técnicas permite obtener una caracterización mucho más completa de estructuras moleculares, materiales cristalinos y nanoestructuras lo que ha convertido a estas herramientas en métodos fundamentales en ciencia de materiales, química, biología y nanociencia.
</p>
