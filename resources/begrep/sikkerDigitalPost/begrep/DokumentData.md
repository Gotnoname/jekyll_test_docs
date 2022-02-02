---
title: DokumentData  

sidebar: begrep_sidebar
redirect_from: /sdp_dokumentdata
---

|---|---|
|Term|{{page.title}}|
|Definisjon|Strukturert data for beriket visning i innbyggers postkasse|
|Datatype|complexType|
|Kjelde|DIFI|

#### Eigenskapar

| --- | --- | --- | --- |
| Identifikator | Kardinalitet | Datatype   | Beskrivelse                                                                  |
| href          | 1..1         | xsd:string | Filnavn på data-dokumentet i dokumentpakken                                  |
| mime          | 1..1         | xsd:string | Utvidelsens mime-type. SKAL LINKE TIL /forretningslag/Utvidelser.md |

#### Xml eksempel

``` 
<data href="lenke.xml" mime="application/vnd.difi.dpi.lenke+xml" />
```
