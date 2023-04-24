---
title: Site Search
layout: search
permalink: /search/
# see _data/search-config.csv for display options
# Lunr.js search will be added below the content in this file
---

## Full metadata search:

{%- assign fields = site.data.config-search | where_exp: 'field', 'field.index == true and field.lang contains page.lang' | map: 'field' -%}

{{ fields }}
