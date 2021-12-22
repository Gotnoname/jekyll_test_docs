---
title: Forretningsmeldinger
permalink: dpi_forretiningsmelding_index.html
sidebar: dpi_timo_sidebar
---

![](/images/dpi/underarbeide.png)

## Forretningsmeldingene i Sikker Digital Post

Alle meldinger er beskrevet i [Standard Business
Document](dpi_sbd_index.html). Denne klassen
inneholder to klasser:

  - Det ene er
    [StandardBusinessDocumentHeader](dpi_sbdh.html)
    som er felles for alle meldinger. 
  - Den andre er Meldingsklassen som enten er av typen Digital, Utskrift, FlyttetDigitalpost, Feil
    eller en [kvittering](dpi_kvitteringer.html). Kvittering kan være av typen
    LeveringsKvittering, VarslingfeiletKvittering, ÅpningsKvittering,  eller
    MottaksKvittering.


### Meldingstypene

Meldingstypen er definert i
[DocumentIdentification](dpi_documentidentification.html)
og er en av følgende:

| Type | Beskrivelse |
| --- | --- |
| [Digital](dpi_digital.html) | Forsendelse av digital post |
| [Utskrift](dpi_utskrift.html) | Forsendelse av melding til utskrift |
| [LeveringsKvittering](dpi_leveringskvittering.html) | Kvittering på at digital post er tilgjengeliggjort eller at en fysisk post er postlagt |
| [ÅpningsKvittering](dpi_aapningskvittering.html) | Kvittering fra Innbygger for at digital post er åpnet |
| [Varslingfeilet](dpi_varslingfeiletkvittering.html) | Kvittering for at en spesifisert varsling ikke har blitt sendt |
| [MottaksKvittering](dpi_mottakskvittering.html) | Kvittering fra utskrift og forsendelsestjenesten om at melding er mottatt og lagt til print |
| [ReturpostKvittering](dpi_returpostkvittering.html) | Kvittering fra utskrift og forsendelsestjenesten om at posten ikke har blitt levert til Mottaker. |
| [Feil](dpi_feil.html) | Generell melding om at det har skjedd en feil. |
| [FlyttetDigitalpost](dpi_flyttetdigitalpost.html) | For flytting av post fra en postkasse til en annen. Brukes kun i mellom postkasseleverandørene |



