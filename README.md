
# Useful Shopify Code Snippets

This is a list of useful Shopify Snippets that I often reference while developing Shopify themes. Feel Free to contribute.

* [Add Custom Badge on Products using product tag](#add-custom-badge-on-products-using-product-tag)

## Add Custom Badge on Products using product tag
This code adds a limited badge on products with "limited" tag on them. Add this in product template.
```html
{% for mytag in product.tags %}
  {% if mytag == 'limited' %}
    <img class="limited-badge" src="{{ 'limited-badge.png' | asset_url }}" alt="Limited Badge">
  {% endif %}
{% endfor %}

## Header - v1
This outuputs a responsive sticky header with the business logo in the centre
The files are in the folder "header.v1"