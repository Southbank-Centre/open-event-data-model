---
layout: page
title: Schema
url: /schema/
permalink: /schema/

breadcrumb: Schema
---

##Entities
The schemas are a set of 'types', each associated with a set of properties.

<ul>
{% for entity in site.entities %}
      <li><a href="{{ entity.url }}">{{ entity.title }}</a></li>
{% endfor %}
</ul>

##Design Principles

The OEDM was developed around a core set of design principles. These are recommendations for how to implement the OEDM and serve as the framework for managing and extending the model.

1. The OEDM is designed to facilitate communications between systems and organisations. As such, it is agnostic as to how data is stored and managed within individual systems.
2. The OEDM is designed to be flexible and extensive. As such, it only requires a small core of standard entities and attributes. Users can extend these through additional attributes or specifying taxonomies for various attributes.
3. The OEDM should be implemented through standard APIs or exchange protocols, such as JSON, XML or RDF.

##Conceptual Model

This is the conceptual model for the OEDM. Each entity has its own page describing it and the core attributes.

<img class="img-concep" src="/images/OEDM-conceptual-entity-model.jpeg"/>
