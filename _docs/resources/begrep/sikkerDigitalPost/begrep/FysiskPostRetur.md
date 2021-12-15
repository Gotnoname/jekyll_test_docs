---
title: FysiskPostRetur  

sidebar: begrep_sidebar
---

|---|---|
|Term|{{page.title}}|
|Definisjon|Informasjon som brukes ved retur av post som av en eller annen grunn ikke kan levers til mottaker.|
|Kilde|DIFI|
|Kommentar|Informasjon som brukes ved retur av post som av en eller annen grunn ikke kan levers til mottaker.|

### Attributer

| Identifikator                                   | Kardinalitet | Datatype                                              |
| ----------------------------------------------- | ------------ | ----------------------------------------------------- |
| [mottaker]({{site.baseurl}}/docs/resources/begrep/felles/Mottaker)                   | 1..1         | [sdp:FysiskPostadresse]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/FysiskPostadresse)            |
| [postHaandtering]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/returPostHaandtering) | 1..1         | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
