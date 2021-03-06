---
layout: page
title: Datasets
id: datasets
---

Add datasets to the Open Traits registry [here](https://github.com/open-traits-network/open-traits-network.github.io/issues/new?assignees=open-traits-network%2Feditors&labels=dataset+review&template=register-dataset.md&title=Please+add+%5Bname%5D+to+the+OTN+dataset+registry).

{% include editorial_status.html %}

|name|contact|description|traits|taxa|
|---|---|---|---|---|
{%- for dataset in site.datasets %}
| [{{ dataset.name }}]({{ dataset.id }})| {{ dataset.contactName | replace: "|","/" }} | {{ dataset.description }} | {{ dataset.traitList | replace: "|","/" }} | {{ dataset.taxaList | replace: "|","/"}} |  
{%- endfor %}

[<a href="https://github.com/open-traits-network/open-traits-network.github.io/tree/master/_datasets">dataset profiles</a>]
