---
title: Standard Business Document  
permalink: standardbusinessdocument_index.html
sidebar: dpi_sidebar
---

|---|---|
| Identifikator | |
| Term          | {{page.title}} |
| Definisjon    | Forretningsmeldingen i en forsendelse inkludert adresseringsinformasjon. |
| Forkortelse   | SBD |
| Kilde         | [GS1](http://www.gs1.org) |

### Standard Business Document (SBD)

[Standard Business
Document](http://www.gs1.org/ecom/standards/guidelines#s2) er en
[GS1](http://www.gs1.org) standard utviklet for å forenkle utveksling av
dokumenter i en B2B kontekst.  
Standardkonvolutten inneholder informasjon for identifisering,
adressering og ruting av forretningsmeldingen. SBD er obligatorisk i
neste versjon av PEPPOL infrastrukturen for fakturaformidling.

I sikker digital post blir Standard Business Document brukt til å sende:

* informasjonen som meldingsformidler trenger for å formidle
meldingen
* identifisering og knytningen mellom forretningsmeldingen
* informasjon som postboksen trenger for å presentere og håndtere
dokumentpakken

### Klassediagram

[![](uml_diagram.jpg)](uml_diagram.jpg)

### Attributter

| Identifikator                                                    | Kardinalitet | Datatype                    | Kommentar                                                                          |
| ---------------------------------------------------------------- | ------------ | --------------------------- | ---------------------------------------------------------------------------------- |
| [StandardBusinessDocumentHeader](sdp_standardbusinessdocumentheader.html) | 1..1         | sh:StandardBusinessDocument | Informasjon for å formidle postforsendelsen                                        |
| [Melding](sdp_index.html)      | 0..1         | [Melding](sdp_index.html) | Forretningsmelding identifisert i [DocumentIdentification](sdp_documentidentification.html) |
