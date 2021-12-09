---
title: Avsender  
permalink: sdp_avsender.html
sidebar: begrep_sidebar
---  

|---|---|
|Term|Avsender|
|Definisjon|Juridisk organisasjon/entitet som er Behandlingsansvarlig for innholdet i den digitale posten|
|Datatype|complexType|
|Kilde|DIFI|
|Kommentar|Avsender er den som er ansvarlig for innholdet i forsendelsen. Kan være forskjellige frå Databehandler (for eksempel kan SvarUT være databehandler på vegne av en kommune)|

#### Egenskaper

| --- | --- | --- |
| Identifikator | Kardinalitet | Datatype |                                                        
| [virksomhetsidentifikator](https://difi.github.io/felleslosninger/virksomhetsidentifikator.html)| 1..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
| [avsenderindentifikator](https://difi.github.io/felleslosninger/avsenderidentifikator.html) | 0..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |           
| fakturaReferanse | 0..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) \[maks 40\] |

#### Xml eksempel

``` 
    <avsender>
        <organisasjon authority="iso6523-actorid-upis">9908:123456789</organisasjon>
        <avsenderidentifikator>12345</avsenderidentifikator>
        <fakturaReferanse>123</fakturaReferanse>        
    </avsender>
```
