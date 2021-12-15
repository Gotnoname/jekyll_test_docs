---
title: FysiskpostInfo  

sidebar: begrep_sidebar
---

|---|---|
|Term|{{page.title}}|
|Definisjon|Informasjon relatert til presentasjon og behandling av en sikker digital post melding|
|Kilde|DIFI|
|Kommentar|Dette er informasjon om den Digitalpostforsendelsen som vil bli brukt av Postkasseleverandør for å presentere og behandle den digitale posten. Den ikkeSensitiveTittelen vil bli brukt i dialogen med Innbygger dersom ikke Innbygger er autentisert på tilstrekkelig nivå. Den ikkeSensitiveTittelen vil også bli brukt i varsling til Innbygger. Når den digitale posten er dekryptert og innbygger er autentisert på tilstrekkelig sikkerhetsnivå så vil Tittel i [Manifest-filen]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Dokumentpakke/Manifest) brukes.|

### Attributer

| --- | --- | --- |
| Identifikator                           | Kardinalitet | Datatype                                              |
| [mottaker]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/FysiskPostadresse)           | 1..1         | [sdp:FysiskPostadresse]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/FysiskPostadresse)            |
| [utskriftstype]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/utskriftstype)        | 1..1         | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
| [retur]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/FysiskPostRetur)                | 1..1         | [sdp:FysiskPostRetur]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/FysiskPostRetur)                |
