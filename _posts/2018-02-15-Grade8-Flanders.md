---
title: A Dog of Flanders
layout: post
permalink: /8/Flanders

 
slides:
 - title: A Dog of Flanders
   slide-data: Aaron,Dominik,Jack,Jenny,Julie and Tom                       （The names are arranged in the alphabet order without priority）
   image: 'https://scris.top/slides/images/Flanders/girldog.jpg'
     
 - title: Slide 2
   slide-data: This is second slide
   background: '#f1c40f'
   
 - title: Slide 3
   slide-data: This is third slide
   background: '#9b59b6'
   
 - title: Slide 4
   slide-data: This is fourth slide
   background: '#3498db'
   
 - title: Slide 5
   slide-data: This is fifth slide
   background: '#2ecc71'
   
 - title: Slide 6
   slide-data: This is sixth slide
   background: '#1abc9c'

 - title: Slide 7
   slide-data: This is seventh slide
   background: '#e67e22'
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
