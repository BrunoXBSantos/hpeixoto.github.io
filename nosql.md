---
layout: default
title: noSQL
image: img/nosql.png
---



{% for class in site.data.nosql.class %}

<h4> <a href="" target="_blank">{{class.code}} - {{class.title}}</a></h4>   
<i class="fa fa-calendar"></i> {{ class.date }} 
<ul>
    <li> <a href="{{ class.plan }}"> Planeamento da Aula </a></li>
    {% if class.slides %} 
        <li> <a href="{{ class.slides }}"> Slides </a> </li>
    {% endif %}
    {% if class.exercise %} 
        <li> <a href="{{ class.exercise }}"> Ficha de Exercícios </a> </li>
    {% endif %}
    {% if class.material %} 
        <li> <a href="{{ class.material }}"> Material de Apoio </a> </li>
    {% endif %}

</ul>  
<strong> tópicos: </strong> {{class.topics}} 

---

{% endfor %}