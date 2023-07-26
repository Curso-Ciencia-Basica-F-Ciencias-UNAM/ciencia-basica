---
title: "{{ replaceRE "-0?" " " .Name | title }}"
date: {{ .Date }}
weight: {{ add ( int ( index ( findRE `[^0]?\d$` .Name ) 0 ) ) 10 }}
draft: true
---

# {{ replaceRE "-0?" " " .Name | title }}

**Subtítulo**

{{<hint info>}}
**Contenido:** ? videos  
**Duración estimada:** ? 
{{</hint>}}

---

## Introducción

## Sección

{{<youtube id="">}}
