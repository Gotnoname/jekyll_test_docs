---
  
title: Meldingsstruktur  

sidebar:
---

En Digitalpost forsendelse består av et hoveddokument med vedlegg.  
Disse dokumentene er beskyttet med kryptering og signering ende til ende
for å sikre konfidensialitet og integritet hele veien fra Avsender til
Mottaker.  
Hoveddokumentet med vedlegg er pakket inn som
[Dokumentpakke((Asic))]({{site.baseurl}}/docs/resources/begrep/ID-porten/index)

Sammen med Dokumentpakken består Digitalpost forsendelse av en
beskrivelse av forsendelsen.  
Dette er behandlingsregler som Postkasseleverandør skal bruke for å
presentere og behandle den digitale postforsendelsen til Mottaker.  
Dette er [StandardBusinessDocument]({{site.baseurl}}/docs/resources/begrep/ID-porten/index), som er
signert/integritetsbeskyttet fra Avsender til Postkasseleverandør.

ebMS 3.0 er brukt som [meldingsutvekslingsrammeverk]({{site.baseurl}}/docs/resources/begrep/ID-porten/index) fra Avsender til
Meldingsformidler.  
Så [eb:Messaging]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/transportlag/Messaging) og [Webservice
security](../oppslagstjenesten/ws-security/WebserviceSecurity.md) er signert/integritetsbeskyttet punkt til
punkt.


![](../felleslosninger/meldingsstruktur_enkel.jpg)
