---
title: Aktører og Roller  

sidebar: dpi_sidebar
---

## Aktør

Tabellen under inneholder en oversikt over hovedaktørene i prosessen med
å utveksle Sikker Digital Post:

| Aktør     | URN     | Identifikator    | Beskrivelse  |
| --- | --- | --- | --- |
| Offentlig virksomhet          | urn:sdp:offentligvirksomhet         | (Her skal det være link til virksomhetsidentifikator under felles. ) | Offentlig virksomhet eller annen virksomhet som utfører en offentlig oppgave på vegne av en offentlig virksomhet                            |
| Tilbyder av meldingsformidler | urn:sdp:forvalter-meldingsformidler | (Her skal det være link til virksomhetsidentifikator under felles. ) | Virksomhet (offentlig eller privat) som tilbyr en meldingsformidlingstjeneste, enten direkte eller via underleverandør                      |
| Tilbyder av postkassetjeneste | urn:sdp:forvalter-postkasse         |(Her skal det være link til virksomhetsidentifikator under felles. ) | Virksomhet (offentlig eller privat) som tilbyr postkassetjenester, enten direkte eller via underleverandører                                |
| Tilbyder av utskriftstjeneste | urn:sdp:forvalter-utskrift          | (Her skal det være link til virksomhetsidentifikator under felles. ) | Virksomhet (offentlig eller privat) som tilbyr utskriftstjeneste, enten direkte eller via underleverandører                                 |
| Sentralforvalter              | urn:sdp:sentralforvalter            |(Her skal det være link til virksomhetsidentifikator under felles. ) | Ansvarlig for forvaltning/kontroll av forholdet mellom offentlig virksomheter, mottaker og tilbydere av meldingsformidler/postkassetjeneste |
| Innbygger                     | urn:sdp:innbygger                   | [personidentifikator]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/personidentifikator)           | Mottaker av postforsendelsen                                                                                                                |

Begrepet **Ansvarlig enhet** har også blitt brukt:

\- **Ansvarlig enhet** brukes av **Behandlingsansvarlig** virksomheter
med et stort virkeområder som ønsker å differensiere Avsendere til
Innbygger avhengig av de interne enhetene som sender posten, i de
tilfeller der det ikke er mulig eller lite hensiktsmessig at interne
enheten selv er identifisert som behandlingsansvarlig (ved å ha et eget
sertifikat).  
**Ansvarlig enhet** blir satt av **Behandlingsansvarlig** ved bruk av en
identifikator. Dette gjøres som en del av klargjøring av en
postmelding.  
Eksempel: Behandlingsansvarlig er NAV og Ansvarlig enhet er NAV
Hjelpemiddelsentral Oslo og Akershus.

## Roller

| Rolle    | URN     | Beskrivelse    |                                   
| --- | --- | --- |
| Avsender\[1\]     | urn:sdp:avsender             | Offentlig virksomhet som skal sende en digital postmelding til en mottaker |
| Behandlingsansvarlig\[1\] | urn:sdp:behandlingsansvarlig | Offentlig virksomhet som produserer informasjon/brev/post som skal fomidles. Vil i de aller fleste tilfeller være synonymt med Avsender                                                                                                                                       |
| Databehandler\[1\]        | urn:sdp:databehandler        | Virksomhet (offentlig eller privat) som har en kontraktfestet avtale med Behandlingsansvarlig med formål å dekke hele eller deler av prosessen med å formidle en digital postmelding fra Behandlingsansvarlig til Meldingsformidler. Det kan være flere databehandlere som har ansvar for forskjellige steg i prosessen med å formidle en digital postmelding. |
| Meldingsformidler         | urn:sdp:meldingsformidler    | Ansvarlig for formidling, sporing og rapportering av postforsendelser.                                                                                                                            |
| Postkasse\[2\]            | urn:sdp:postkasse            | Ansvarlig for å tilgjengeliggjøre og oppbevare post til mottaker, samt å varsle mottaker når det er kommet ny post., eventuelt: Ansvarlig for print og forsendelse av papir post til mottaker.                                                       |
| Mottaker                  | urn:sdp:mottaker             | Innbyggeren som er mottaker av en digital postmelding                                                                                                                                                                                                                                                                                                          |

<!-- TODO: Bør inn med figur som viser samanhengen -->
<!-- TODO:Endre linkingen -->
1.  Avsenderrollen kan være en sammensatt rolle bestående av Avsender,
    Behandlingsansvarlig og/eller en eller flere databehandlere. For å
    forenkle dokumentasjonen er denne kompleksiteten skjult bak rollen
    Avsender, med egne kommentarer i de tilfeller der flere aktører i
    rollen Avsender medfører utfordringer.



2.  Printleverandør for utskrift og fysisk forsendelse av post blir i
    dokumentasjonen håndtert som en postkasse, med egne kommentarar der
    dette medfører utfordringer.
