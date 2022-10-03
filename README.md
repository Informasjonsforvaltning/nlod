# Norwegian Licence for Open Government Data (NLOD)

Repo for revisjon av lisensen.

## Struktur

```Shell
├── 1.0
│   ├── en
│   │   └── index.adoc    # engelsk lisens-tekst (juridisk)
│   ├── no
│   │   └── index.adoc    # norsk lisens-tekst (juridisk)
├── 2.0
│   ├── en
│   │   └── index.adoc    # engelsk lisens-tekst (juridisk)
│   ├── no
│   │   └── index.adoc    # norsk lisens-tekst (juridisk)
└── index.adoc            # norsk/engelsk oppsummering med lenke til versjonar og språk
```

## Bygge lokalt

For å bygge alle sidene på begger språk lokalt:

```Shell
% docker run -it -v $(pwd):/documents asciidoctor/docker-asciidoctor
asciidoctor -D docs -o index.html -a lang=nb docs/index.adoc
asciidoctor -D docs/1.0/no -o index.html -a lang=nb docs/1.0/no/index.adoc
asciidoctor -D docs/1.0/en -o index.html -a lang=en docs/1.0/en/index.adoc
asciidoctor -D docs/2.0/no -o index.html -a lang=nb docs/2.0/no/index.adoc
asciidoctor -D docs/2.0/en -o index.html -a lang=en docs/2.0/en/index.adoc
```
