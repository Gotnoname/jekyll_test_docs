---
title: HentEndringerForespoersel  

sidebar: begrep_sidebar
redirect_from: /ot_hentendringerforespoersel
---

| --- | --- |
| Term          | {{page.title}} |
| Definisjon    | Forespørsel sendt fra Virksomhet for å hente endringer fra kontakt og reservasjonsregisteret |
| Datatype      | {{ page.datatype }} |
| Kilde         | DIFI |
| Kommentar     | Webservice forespørsel som Klient sender til Kontaktregisteret, forespørselen beskriver hvilke endringer Klienten ønsker. Se integrasjonsguiden for Oppslagstjenesten for tekniske detaljer om forespørselen og hvordan denne sendes. |

Responsen er en [HentEndringerRespons]({{site.baseurl}}/resources/begrep/oppslagstjenesten/HentEndringerRespons)

#### Attributer

| Term                                           | Kardinalitet |
| ---------------------------------------------- | ------------ |
| [fraEndringsNummer]({{site.baseurl}}/resources/begrep/felles/fraEndringsNummer) | 1..1         |
| [informasjonsbehov]({{site.baseurl}}/resources/begrep/felles/informasjonsbehov) | 0..\*        |

#### Kodeverk for [informasjonsbehov]({{site.baseurl}}/resources/begrep/felles/informasjonsbehov)

| Kodeverdi         | Beskrivelse                                                                                                                 |
| --- | --- |
| Person            | Person gir kun informasjon om Personen finnes i registeret og reservasjonsstatus. Person er implisitt og returneres alltid. |
| Kontaktinfo       | Kontaktinfo gir informasjon om Personers kontaktinformasjon. Kontaktinformasjon er implisitt og returneres alltid.          |
| Sertifikat        | Sertifikat gir informasjon om Person sitt sertifikat som skal brukes i forbindelse med kryptering av Sikker Digital Post    |
| SikkerDigitalPost | SikkerDigitalPost gir informasjon om Person, postkasse og postkasseleverandøren.                                            |

  - Dersom Informasjonsbehov ikke sendes inn er standard verdi: Person +
    Kontaktinfo
  - Eventuell overflødig eller dobbel spesifikasjon av informasjonsbehov
    ignoreres.

#### Xml eksempel

``` 
<ns:HentEndringerForespoersel fraEndringsNummer="1001">     
 <ns:informasjonsbehov>Kontaktinfo</ns:informasjonsbehov>
 <ns:informasjonsbehov>Sertifikat</ns:informasjonsbehov>
 <ns:informasjonsbehov>SikkerDigitalPost</ns:informasjonsbehov>
</ns:HentEndringerForespoersel>
```
