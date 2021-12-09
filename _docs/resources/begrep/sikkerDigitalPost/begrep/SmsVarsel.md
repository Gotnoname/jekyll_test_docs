---
title: SmsVarsel  
permalink: sdp_smsvarsel.html
sidebar: begrep_sidebar
---

|---|---|
| Term | {{page.title}} |
| Definisjon | Informasjon om hvordan man skal varsle sluttbruker på sms |
| Datatype | complexType |
| Kjelde | DIFI |
| Kommentar | Beskriver når det skal sendes sms varsel fra postkassen etter at posten er tilgjengeliggjort. Denne tjenesten vil medføre kostnader for Avsender |

#### Eigenskapar

| Identifikator                                    | Kardinalitet | Datatype                                              |
| --- | --- | --- |
| [mobiltelefonnummer](../../felles/mobiltelefonnummer.md) | 1..1     | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
| [Varslingstekst](varslingstekst.html)        | 1..1     | [Varslingstekst](varslingstekst.html)        |
| [Repetisjoner](Repetisjoner.md)                     | 1..1         | [sdp:Repetisjoner](Repetisjoner.md)                    |

#### Xml eksempel

``` 
    <smsVarsel>
      <mobiltelefonnummer>12121212</mobiltelefonnummer>
      <varslingsTekst lang="no">Viktig melding fra Staten</varslingsTekst>
      <repetisjoner>
        <dagerEtter>0</dagerEtter>
        <dagerEtter>7</dagerEtter>
      </repetisjoner>
    </smsVarsel>
 
```
