# Norwegian Licence for Open Government Data (NLOD)

Repo for revisjon av lisensen.

## Struktur

```Shell
├── en
│   ├── 2.0
│   │   └── index.adoc    # engelsk lisens-tekst (juridisk)
│   └── index.adoc        # engelsk oppsummering
├── no
│   ├── 2.0
│   │   └── index.adoc    # norsk lisens-tekst (juridisk)
│   └── index.adoc        # norks oppsummering
├── index.adoc            # landingsside, evt redirect
```

## Bygge lokalt

```Shell
% docker run -it -v $(pwd):/documents asciidoctor/docker-asciidoctor
# asciidoctor -D build -R docs 'docs/**/*.adoc'
```
