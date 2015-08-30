---
layout: page-fullwidth
permalink: "/products/"
---



<div class="row">

{% for product in site.data.products %}

    <div class="small-12 medium-4 columns">
      <div class="item-wrapper">
        <div class="img-wrapper">
          <a href="{{product.gumroad}}" class="gumroad-button button expand add-to-cart">Add to Cart</a>
          <a href="{{ site.url }}{{ site.baseurl }}/pages/{{ product.name }}"><img class=" medium-centered" src="{{site.urlimg}}/thumb/{{ product.image }}"></a>
        </div>  

        <a href="{{ site.url }}{{ site.baseurl }}/pages/{{ product.name }}"><h3 class="bold">{{ product.title }}</h3></a>
        <p class="x2">Retail: <span class="line-trough">{{product.retail}}</span>, 
        <strong class="x3">Today's Price: {{product.price}}</strong></p>
        <!-- <p>{{product.short_description}}</p> -->
      </div>  
    </div>


  {% endfor %}

  </div>
<!--   title: "Bookshelf"
subheadline: "A Step-by-Step Guide"
teaser: "This step-by-step guide helps you to customize Feeling Responsive to your needs." -->