---

title: Sending av digital post på vegne av andre  

sidebar: dpi_sidebar
redirect_from: /sdp_send_paa_vegne_av_andre
---

## Sending av Post på vegne av andre

Digital post til innbyggere har støtte for at en virksomhet kan sende
post på vegne av en annen.  
Dette kan brukes både dersom en virksomhet har en databehandler som skal
sende post på deres vegne eller i de tilfeller at en virksomhet har
underliggende enheter/virksomheter.  
Her er det beskrevet noen eksempler på hvordan en virksomhet kan sende
post på vegne av andre.

### Eksempel - bruk av databehandler

I dette eksemplet er Helfo Behandlingansvarlig og NAV er databehandler
for Helfo.  
Nav har den tekniske integrasjonen og kan bruke sitt
virksomhetssertifikat på vegne av Helfo dersom Helfo tillatter dette.  
Både Helfo og Nav er opprettet med kontoer hos postkasseleverandørene,
Helfo som Ansvarlig postavsender og Nav som Teknisk postavsender.

[![Bruk av databehandler]({{site.baseurl}}/images/helfo_eksempel.png)

### Eksempel - Sending fra underliggende avdeling

I dette eksemplet har Kreftregisteret ønske om at postavsender skal være
er en av de underliggende prosjektene de har (Tarmkreftscreening,
Masseundersøkelse mot livmorhalskreft, Mammografiprogrammet) i sin
virksomhet.  
De underliggende prosjektene er ikke egne selvstendige virksomheter med
eget organisasjonsnummer.  
Kreftregisteret er teknisk avsender og bruker sitt virksomhetssertifikat
for alle de underliggende prosjektene som er postavsender.  
Både Kreftregisteret og de underliggende prosjektene er opprettet med
kontoer hos postkasseleverandørene.  
Kreftregisteret bruker
[avsenderidentifikator]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/begrep/avsenderidentifikator) for å skille på
hvilket prosjekt som er postavsender.

[![Bruk av avsenderidentifikator]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/forretningslag/kreftregister_eksempel.png)
