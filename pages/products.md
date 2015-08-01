---
layout: page-fullwidth
show_meta: false
header: false
permalink: "/products/"
---



<div class="row">
        ​<a href="https://gum.co/zvKqj" class="gumroad-button">Buy my
> product</a>
{% for product in site.data.products %}

    <div class="small-12 medium-4 columns">
      <div class="item-wrapper">
        <div class="img-wrapper">
          <a class="button expand add-to-cart">Add to Cart</a>
          <a href="{{ site.url }}{{ site.baseurl }}/pages/{{ product.name }}"><img src="{{site.urlimg}}/thumb/{{ product.image }}"></a>
        </div>  

        <a href="https://gum.co/XXXX"><h3>{{ product.title }}</h3></a>
        <h5>{{product.price}}</h5>
        <p>{{product.short_description}}</p>
      </div>  
    </div>


  {% endfor %}

  </div>
<!--   title: "Bookshelf"
subheadline: "A Step-by-Step Guide"
teaser: "This step-by-step guide helps you to customize Feeling Responsive to your needs." -->