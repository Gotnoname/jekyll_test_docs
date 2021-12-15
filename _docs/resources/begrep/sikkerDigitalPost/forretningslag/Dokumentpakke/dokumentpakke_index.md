---
title: Dokumentpakke (ASiC)  

sidebar: dpi_sidebar
---

## Introduksjon

Dokumentpakke inngår kun i
[DigitalPostMeldinger]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/DigitalpostMelding.png).

[Associated Signature Container
(ASiC)](http://www.etsi.org/deliver/etsi_ts/102900_102999/102918/01.03.01_60/ts_102918v010301p.pdf)
er et pakkeformat som er designet for å ivareta integritet til innholdet
over lang tid. Kort fortalt så definerer standarden hvordan man skal
sette sammen en zip fil med en filstruktur der man lager en digital
signatur hver enkel fil med en kombinasjon av et digitalt fingeravtrykk
av filen og et PKI sertifikat eid av en virksomheten.  
Dette medfører at man kan verifisere at filene kommer fra rett
virksomhet, og om filene har blitt endret.

Les mer om [hvordan dokumenter som sendes i Sikker digital post er
beskyttet](sikkerhet_index.html)

Sikker Digital Post har definert et eget begrep [Manifest]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentpakke/Manifest) som
inneholder metadata relatert til hver fil.

### Innhold

| Fil                      | Kardinalitet | Beskrivelse                                                                                                                      |
| ------------------------ | ------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| hoveddokument            | 1..1         | fil - se: krav til [filnavn og dokumentformat]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentformat/index)                                                               |
| [manifest.xml]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentpakke/Manifest) | 1..1         | [manifest]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentpakke/Manifest)                                                                                                             |
| vedlegg                  | 0..200       | fil - se: krav til [filnavn og dokumentformat]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentformat/index)                                                               |
| META-INF/signatures.xml  | 1..1         | [XAdES](http://www.etsi.org/deliver/etsi_ts%5C101900_101999%5C101903%5C01.04.02_60%5Cts_101903v010402p.pdf) signaturer av filene |

### Begrensninger

  - Dokumentpakken kan ikke overstige 30Mb
  - Dokumentpakken kan inneholde et hoveddokument
  - Dokumentpakken kan ha inntil 200 vedlegg
  - Avsender kan ikke definere rekkefølgende på vedleggene, sorteringen
    av disse håndteres av postkassen.

### Eksempel

  - [Manifest]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/eksempler/sdpManifest.xml)
  - [Full dokumentpakke]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/eksempler/post.asice.zip)

### Refererte standarder

  - [Associated Signature Container
    (ASiC)](http://www.etsi.org/deliver/etsi_ts/102900_102999/102918/01.03.01_60/ts_102918v010301p.pdf)
  - [XAdES](http://www.etsi.org/deliver/etsi_ts%5C101900_101999%5C101903%5C01.04.02_60%5Cts_101903v010402p.pdf)
