---
title: "Medios de Transmisión"
layout: post
permalink: /medios-de-transmision/
background: "#0a5"

slides:
 - title: "Clasificación de Medios de Transmisión"
   slide-data: "Existen dos tipos de medios de transmisión: <strong>guiados</strong> e <strong>inalámbricos</strong>, cada uno con características distintas para diferentes aplicaciones."
     
 - title: "Medios Guiados"
   slide-data: "Los medios guiados incluyen cables de par trenzado, coaxial y fibra óptica, adecuados para transmisión de datos en redes locales y de larga distancia."

 - title: "Par Trenzado"
   slide-data: "<ul><li><strong>UTP</strong>: Sin blindaje, económico, pero menos protegido contra interferencias.</li><li><strong>STP</strong>: Con blindaje para reducir interferencias, aunque es más caro y voluminoso.</li></ul>"
   
 - title: "Cable Coaxial"
   slide-data: "Este medio ofrece una mejor protección contra interferencias en comparación con el par trenzado. Se usa en redes de TV y Ethernet. Existen varias categorías específicas para aplicaciones distintas."

 - title: "Fibra Óptica"
   slide-data: "Utiliza luz para transmitir datos a alta velocidad con baja atenuación. Hay dos tipos principales:<ul><li><strong>Multimodo</strong>: Para distancias cortas.</li><li><strong>Monomodo</strong>: Ideal para distancias largas y ancho de banda elevado.</li></ul>"
   background: "#3498db"

 - title: "Medios no guiados (Inalámbricos)"
   slide-data: "Los medios no guiados incluyen ondas de radio, microondas e infrarrojo, útiles en comunicaciones de corta y larga distancia sin necesidad de cables físicos."

 - title: "Ondas de Radio"
   slide-data: "Adecuadas para transmisiones a larga distancia con señales omnidireccionales, útiles en radio AM, FM y televisión."

 - title: "Microondas"
   slide-data: "Ofrecen transmisión de datos de alta velocidad en distancias largas. Necesitan una línea de vista entre las antenas."

 - title: "Infrarrojo"
   slide-data: "Se usa en dispositivos de corto alcance como mandos a distancia. No atraviesa paredes, lo que ayuda a evitar interferencias en espacios cerrados."

 - title: "Aplicaciones y Rendimiento"
   slide-data: "Cada tipo de medio tiene aplicaciones específicas:<ul><li><strong>Par trenzado</strong>: Redes locales y líneas telefónicas.</li><li><strong>Fibra óptica</strong>: Ideal para redes de larga distancia por su velocidad y baja interferencia.</li></ul>"

---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
        <h1>{{slide.title}}</h1>{{ slide.slide-data }}
</section>               
{% endfor %}

