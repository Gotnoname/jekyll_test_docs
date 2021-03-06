--- 
title: OppdaterPostkasseRespons  

sidebar: begrep_sidebar
---

|---|---|
| Term          | {{page.title}} |
| Definisjon    | Respons sendt tilbake til Postkasseleverandør når kontaktregisteretet er oppdatert. |
| Datatype      | {{ page.datatype }} |
| Kilde         | DIFI |
| Kommentar     | Webservice response som Postkasseleverandør mottar fra Kontaktregisteret som svar på [OppdaterPostkasseForespoersel]({{site.baseurl}}/resources/begrep/oppslagstjenesten/OppdaterPostkasseForespoersel) |

#### Attributer

| Term        | Kardinalitet | Datatype                                              |
| ----------- | ------------ | ----------------------------------------------------- |
| status      | 1..1         | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
| beskrivelse | 0..1         | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |

#### Kodeverk for status

feiltype kan ha følgende verdi:

| Kodeverdi | Beskrivelse                                                                        |
| --------- | ---------------------------------------------------------------------------------- |
| OK        | Transaksjonen gikk ok                                                              |
| FEILET    | Det har oppstått en feil i behandlingen av forespørselen, se beskrivelse for årsak |

#### Kodeverk for beskrivelse

feiltype kan ha følgende verdi:

| Kodeverdi                       | Beskrivelse                                                                         |
| ------------------------------- | ----------------------------------------------------------------------------------- |
| RESERVERT                       | Brukeren er reservert                                                               |
| ALLEREDE\_AKTIV                 | Brukeren er allerede aktiv                                                          |
| INGEN\_POSTBOKS\_FUNNET         | Det ble ikke funnet noe postkasse på brukeren                                       |
| BRUKER\_IKKE\_FUNNET            | Innbyggeren ble ikke funnet                                                         |
| POSTKASSE\_EKSISTERER\_ALLEREDE | Postkasseinformasjon finnes allerede på denne brukeren                              |
| UGYLDIG\_SERTIFIKAT             | Sertifikatet i forespørselen er ikke på godkjent format                             |
| UGYLDIG\_PERSONNUMMER           | Personidentifikator i forespørsel er ikke på riktig format                          |
| UGYLDIG\_EPOSTADRESSE           | Epostadressen i forespørselen er ikke på riktig format                              |
| UGYLDIG\_ORGNR                  | Virksomhetsindentifikatoren i forespørselen er ikke på riktig format eller godkjent |
