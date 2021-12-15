---

title: PartyInfo  

sidebar: dpi_sidebar
---

## {{page.title}}

  - Identifikator  
    “http://begrep.difi.no{{ page.url | remove:”.html"
    }}":{{page.title}}
  - Term  
    {{page.title}}
  - Definisjon  
    Informasjon om mottaker/avsender
  - Datatype  
    complexType
  - Kilde  
    [ebMS 3.0](http://docs.oasis-open.org/ebxml-msg/ebms/v3.0/core/ebms-header-3_0-200704.xsd)

### Egenskaper

Består av to elementer som identifiserer avsender (eb:From) og mottaker
(eb:To), som hver har følgende egenskaper

| Identifikator | Type | Kardinalitet | Kommentar |
| --- | --- | --- | --- |
| PartyId | [Virksomhetsidentifikator]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/virksomhetsidentifikator) | 1..1 | |
| Role | [Konstant]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Aktorer) | 1..1 | Definerer rollen i meldingsutvesklingen |

### Kodeverdier for konstanten Role

Role skal benytte URN som angitt i listen over
[aktører]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/forretningslag/Aktorer). Merk at avsender av en Digital
Forsendelse ofte er enten en behandlingsansvarlig (produsent av
meldingen) eller databehandler (som formidler meldingen etter avtale med
behandlingsansvarlig)

### Xml eksempel

``` brush: xml; toolbar: false
    <eb:PartyInfo>
        <eb:From>
            <eb:PartyId type="urn:oasis:names:tc:ebcore:partyid-type:iso6523:9908">%%ORG_NR_PK%%</eb:PartyId>
            <eb:Role>urn:sdp:postkasse</eb:Role>
        </eb:From>
        <eb:To>
            <eb:PartyId type="urn:oasis:names:tc:ebcore:partyid-type:iso6523:9908">%%ORG_NR_MF%%</eb:PartyId>
            <eb:Role>urn:sdp:meldingsformidler</eb:Role>
        </eb:To>
    </eb:PartyInfo>                
```
