---
layout: default
tagtitle: Java Development
tagline: All about Java
---


<!-- {% assign max_post_size = include.max  %}

{% capture my_variable %}
{{page.path | remove: "tags/" }}

{% endcapture %}

 {% assign tagvar = my_variable | remove: ".md" %}
 {{ tagvar }}

 
 {% assign s = site.tags.Java %} -->


 

 <ul class="post-list">
 {% for post in s limit:10 %}
   {% capture current_year %}{{ post.date | date: "%Y" }}{% endcapture %}
   {% if current_year != previous_year %}
   {% unless forloop.first %}
    
{% endunless %}
    <h1>{{ current_year }}</h1>
    <ul>
    {% assign previous_year = current_year %}
   {% endif %}




<li> <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }} - {{post.tagline}}</a>  
        <section  class="list_post_detailed">  
            {% include post-meta-info_detailed.html post_date=post.date post_lang=post.lang %}
        </section> 
      </li>
    
{% if forloop.last %}
        </ul>
{% endif %}

{% endfor %}

 </ul>