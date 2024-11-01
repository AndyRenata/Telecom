---
title: "Medios de Transmisión"
layout: post
permalink: /medios-de-transmision/
background: "#0a5"
font: "Arial, sans-serif" # Cambia la fuente para todas las diapositivas

slides:
 - title: "Introducción a los Medios de Transmisión"
   slide-data: "Los medios de transmisión son fundamentales en la comunicación de datos. Se dividen en dos tipos: <strong>medios guiados</strong> (con cables) e <strong>medios no guiados</strong> (inalámbricos), cada uno adecuado para aplicaciones específicas."
   background: "#2980b9"
   image: "https://github.com/AndyRenata/telecom/blob/master/images/OIP.jpeg?raw=true"

 - title: "Medios Guiados"
   slide-data: "Este tipo de medio utiliza cables físicos para transmitir datos. Incluye cables de par trenzado, coaxial y fibra óptica, los cuales se usan para diferentes distancias y tasas de transmisión."
   background: "#2ecc71"
  

 - title: "Cables de Par Trenzado"
   slide-data: "<p>El cable de par trenzado es común en redes locales (LAN). Existen dos tipos principales:</p><ul><li><strong>UTP (Unshielded Twisted Pair)</strong>: Sin blindaje, económico, pero menos protegido contra interferencias.</li><li><strong>STP (Shielded Twisted Pair)</strong>: Incluye blindaje, ofrece más protección pero es más costoso.</li></ul><p>Ambos tipos de cables vienen en diferentes categorías, como CAT5 y CAT6, que indican su capacidad de transmisión.</p>"
   background: "#f1c40f"
   image: "https://github.com/AndyRenata/telecom/blob/master/images/descargar.jpeg?raw=true"
   
 - title: "Cable Coaxial"
   slide-data: "El cable coaxial proporciona un mejor blindaje contra interferencias y se usa ampliamente en redes de televisión y conexiones Ethernet. Existen categorías como RG-59 (para TV) y RG-6 (para aplicaciones de mayor calidad)."
   background: "#d35400"
   image: https://github.com/AndyRenata/telecom/blob/master/images/Cable%20Coaxial.jpeg

 - title: "Fibra Óptica"
   slide-data: "<p>La fibra óptica es ideal para largas distancias y velocidades altas, utilizando luz para la transmisión de datos. Hay dos tipos:</p><ul><li><strong>Multimodo</strong>: Para distancias cortas, como en redes de área local.</li><li><strong>Monomodo</strong>: Para distancias largas, excelente para alta capacidad de datos.</li></ul><p>Es resistente a interferencias electromagnéticas.</p>"
   background: "#8e44ad"
   image: https://github.com/AndyRenata/telecom/blob/master/images/Fibra%20%C3%93ptica.jpeg

 - title: "Medios No Guiados"
   slide-data: "Los medios no guiados son los que transmiten datos sin el uso de cables. Incluyen las ondas de radio, microondas y el infrarrojo. Son ideales para aplicaciones móviles y de corta distancia."
   background: "#27ae60"
   image: https://github.com/AndyRenata/telecom/blob/master/images/Medios%20No%20Guiados.jpeg

 - title: "Ondas de Radio"
   slide-data: "<p>Las ondas de radio permiten transmisiones a larga distancia y son omnidireccionales, ideales para radio AM/FM y transmisión de TV.</p><p>Ejemplos de uso: transmisión de radio, redes Wi-Fi y sistemas de comunicaciones satelitales.</p>"
   background: "#c0392b"
   image: https://github.com/AndyRenata/telecom/blob/master/images/Ondas%20de%20Radio.jpeg

 - title: "Microondas"
   slide-data: "Las microondas son unidireccionales y requieren una línea de vista clara entre las antenas transmisora y receptora. Usos comunes incluyen redes de satélites y telefonía móvil."
   background: "#16a085"
   image: https://github.com/AndyRenata/telecom/blob/master/images/Diagrama%20de%20torre%20de%20microondas.jpeg

 - title: "Infrarrojo"
   slide-data: "El infrarrojo es ideal para dispositivos de corto alcance como controles remotos. No atraviesa paredes, lo cual ayuda a reducir interferencias en entornos cerrados."
   background: "#7f8c8d"
   note: "Imagen sugerida: Icono de señal infrarroja en el centro (tamaño 150x150px)."

 - title: "Aplicaciones y Rendimiento de los Medios"
   slide-data: "Cada tipo de medio tiene aplicaciones específicas en función de su rendimiento y capacidad. Por ejemplo:<ul><li><strong>Par Trenzado</strong>: Ideal para redes locales y telefonía.</li><li><strong>Fibra Óptica</strong>: Excelente para transmisión de datos a larga distancia y en redes de alta velocidad.</li></ul>"
   background: "#2980b9"
   note: "Imagen sugerida: Gráfico de rendimiento comparativo en la esquina inferior derecha (tamaño 250x150px)."
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}" style="font-family: {{page.font}};">
        <h1 style="font-size: 2em; text-align: left; margin-bottom: 0.5em;">{{slide.title}}</h1>
        <div style="font-size: 1.2em; margin-top: 1em;">{{ slide.slide-data }}</div>
        {% if slide.note %}<div style="font-size: 0.8em; color: #555; margin-top: 1em;"><em>Nota:</em> {{ slide.note }}</div>{% endif %}
</section>               
{% endfor %}
