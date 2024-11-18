---
icon: diagram-predecessor
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
---

# Subdominios

## <mark style="color:orange;">Detección  de subdominios con Subfinder y nuclei</mark>

```
subfinder -d ejemplo.com -o Ejem.txt && nuclei -t wp-xyz-takeover.yaml -l Ejem.txt
```

## <mark style="color:orange;">Rapiddns</mark>

Agregue esta sencilla función a su '.bash\_profile' para aprovechar la API de RapidDNS:

```
rapiddns() {
curl -s "
https://lnkd.in/gzbkHQ3W
" \
| grep -oP '_blank">\K[^<]*' \
| grep -v http \
| sort -u
}
```

Una vez agregado, simplemente corres la herramienta:

```
rapiddns netflix.com
```

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
