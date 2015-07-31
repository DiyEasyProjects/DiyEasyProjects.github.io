---
layout: page-fullwidth
show_meta: false
header: false
permalink: "/products/"
---



<div class="row">

{% for product in site.data.products %}

    <div class="small-12 medium-4 columns">
      <div class="item-wrapper">
        <div class="img-wrapper">
          <a class="button expand add-to-cart">Add to Cart</a>
          <a href="{{ product.url }}"><img src="http://i.imgur.com/Mcw06Yt.png"></a>
        </div>  
        <a href="#"><h3>{{ product.title }}</h3></a>
        <h5>{{product.price}}</h5>
        <p>{{product.short_description}}</p>
      </div>  
    </div>


  {% endfor %}

  </div>
<!--   title: "Bookshelf"
subheadline: "A Step-by-Step Guide"
teaser: "This step-by-step guide helps you to customize Feeling Responsive to your needs." -->