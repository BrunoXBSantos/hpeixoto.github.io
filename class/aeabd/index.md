---
layout: default
title: AEABD
image: img/aebd.png
---

<h3 style="text-align:center;">Administração e Exploração Avançada de Base de Dados</h3>

---

{% for class in site.data.aeabd.class %}

<h4> <a href="" target="_blank">{{class.code}} - {{class.title}}</a></h4>   
<i class="fa fa-calendar"></i> {{ class.date }} 
<ul>
    <li> <a href="{{ class.plan }}" target='_blank'> Planeamento da Aula </a></li>
    {% if class.slides %} 
        <li> <a href="{{ class.slides }}" target='_blank'> Slides </a> </li>
    {% endif %}
    {% if class.exercise %} 
        <li> <a href="{{ class.exercise }}" target='_blank'> Ficha de Exercícios </a> </li>
    {% endif %}
    {% if class.material %} 
        <li> <a href="{{ class.material }}" target='_blank'> Material de Apoio </a> </li>
    {% endif %}
</ul>  
<strong> tópicos: </strong> {{class.topics}} 

---

{% endfor %}