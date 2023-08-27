---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

```{code-cell}
:tags: [remove-input]

from myst_nb import glue
import datetime
import locale
locale.setlocale(locale.LC_TIME, "nl-NL")
now_time = datetime.datetime.now()
publish_date_time = now_time.strftime('%Y-%m-%dT%H:%M') + datetime.datetime.now(datetime.timezone.utc).astimezone().strftime('%z')
publish_day = now_time.strftime('%A')
publish_time = now_time.strftime('%H:%M')

glue("pub_date_time", publish_date_time, display=False)
glue("pub_day", publish_day, display=False)
glue("pub_time", publish_time, display=False)
```


# Eerste hoofdstuk uit test-pagina-github

Dit is dus een test boek om te zien hoe het bijwerken van het boek naar github werkt.


```{tableofcontents}
```


Dit boek is gepubliceerd op {glue:text}`pub_day` om {glue:text}`pub_time` ({glue:text}`pub_date_time`).