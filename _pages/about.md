---
layout: single
title: "Presentación"
permalink: /
author_profile: true
---
### Sobre mí

<p style="text-align: justify;">
<p style="text-align: justify;">
Mi formación se ha desarrollado en dos trayectorias en paralelo, Física y Matemáticas, y esa doble base ha guiado mi trabajo académico y docente. En Física, mis intereses evolucionaron hacia el estudio de materiales, nanomateriales y, finalmente, hacia la espectroscopía como una herramienta central para comprender sistemas complejos. Durante este recorrido trabajé en el <a href="https://www.iim.unam.mx/" target="_blank">Instituto de Investigaciones en Materiales</a> en la simulación de nanoestructuras mediante métodos <em>ab initio</em>, y más adelante en el <a href="https://www.icat.unam.mx/" target="_blank">Instituto de Ciencias Aplicadas y Tecnología</a>, donde me enfoqué en espectroscopía infrarroja y Raman, así como en el procesamiento de señales mediante métodos estadísticos e inteligencia artificial. En paralelo, mi formación matemática me llevó hacia la estadística y las finanzas cuantitativas, área que complementé con certificaciones especializadas en el <a href="https://www.nyif.com/" target="_blank">New York Institute of Finance</a> y los exámenes del <a href="https://www.garp.org/" target="_blank">Global Association of Risk Professionals</a> y del <a href="https://www.cfainstitute.org/" target="_blank">CFA Institute</a>, además de experiencia práctica. Durante una etapa profesional trabajé como científico de datos y, por un breve periodo, como consultor financiero, experiencias que han contribuido de manera directa a mi acumulación de experiencia en el área cuantitativa. Actualmente continúo ampliando mi formación académica y científica, mientras asumo con seriedad mi responsabilidad docente y administro algunas carteras de inversión como parte de mi práctica aplicada.
</p>
</p>


### ¿Tienes curiosidad de saber lo que es el DFT?
<div style="text-align:center;">
<iframe width="720" height="405"
src="https://www.youtube.com/embed/QGyfGCZT110"
title="Introduction to Density Functional Theory"
frameborder="0"
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>
</div>

Breve Resumen: 
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



<div style="text-align:center;">
<iframe width="720" height="405"
src="https://www.youtube.com/embed/QGyfGCZT110"
title="Introduction to Density Functional Theory"
frameborder="0"
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen>
</iframe>
</div>

<p style="text-align: justify;">
La espectroscopía constituye una de las herramientas experimentales fundamentales para estudiar la estructura y la dinámica de la materia. Su principio general consiste en analizar la interacción entre la radiación electromagnética y un sistema físico con el fin de extraer información sobre su estructura electrónica, vibracional o molecular. Desde el punto de vista cuántico esta interacción puede describirse mediante un Hamiltoniano de la forma \( \hat H = \hat H_0 + \hat H_{\text{int}} \), donde \( \hat H_0 \) representa el sistema en ausencia de radiación y \( \hat H_{\text{int}} \) describe el acoplamiento con el campo electromagnético. En el régimen dipolar eléctrico este término toma la forma \( \hat H_{\text{int}} = - \boldsymbol{\mu} \cdot \mathbf{E}(t) \), siendo \( \boldsymbol{\mu} \) el operador de momento dipolar molecular y \( \mathbf{E}(t) \) el campo eléctrico incidente. La absorción o dispersión de radiación ocurre cuando la energía del campo coincide con la diferencia entre niveles de energía del sistema, lo que se expresa como \( h\nu = E_f - E_i \). En espectroscopía vibracional estos niveles corresponden a modos vibracionales asociados a enlaces químicos cuya frecuencia, en la aproximación armónica, puede escribirse como \( \nu = \frac{1}{2\pi}\sqrt{\frac{k}{\mu}} \), donde \(k\) es la constante de fuerza del enlace y \(\mu\) la masa reducida del sistema vibracional. Estas vibraciones constituyen una especie de huella molecular que permite identificar estructuras químicas y estudiar propiedades estructurales de materiales.
</p>

<p style="text-align: justify;">
Entre las técnicas más utilizadas se encuentran la espectroscopía infrarroja y la espectroscopía Raman, ambas dedicadas al estudio de vibraciones moleculares pero basadas en mecanismos físicos distintos. La espectroscopía infrarroja se fundamenta en la absorción de radiación cuando una vibración molecular produce un cambio en el momento dipolar, lo cual se expresa mediante la condición \( \frac{\partial \mu}{\partial Q} \neq 0 \), donde \(Q\) representa la coordenada normal de vibración. Por esta razón IR resulta particularmente sensible a enlaces polares y a variaciones en la distribución de carga dentro de una molécula o un sólido. La espectroscopía Raman, en cambio, se basa en la dispersión inelástica de la luz incidente conocida como efecto Raman. En este proceso la radiación interactúa con la polarizabilidad electrónica del sistema y genera fotones dispersados cuya frecuencia difiere de la frecuencia incidente. Una vibración será activa en Raman cuando se cumple \( \frac{\partial \alpha}{\partial Q} \neq 0 \), donde \(\alpha\) representa el tensor de polarizabilidad molecular. Debido a estas diferencias ambas técnicas resultan complementarias, ya que IR detecta vibraciones asociadas a cambios en el momento dipolar mientras que Raman revela aquellas relacionadas con cambios en la polarizabilidad electrónica. La combinación de ambas proporciona una caracterización mucho más completa de moléculas, materiales cristalinos y nanoestructuras.
</p>

