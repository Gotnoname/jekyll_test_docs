---

title: UserMessage  

sidebar: dpi_sidebar
---

## {{page.title}}

  - Term  
    {{page.title}}
  - Definisjon  
    ebMS 3.0 relaterte metadata om en transporten av
    forretningsmeldingen
  - Kilde  
    [ebMS 3.0](http://docs.oasis-open.org/ebxml-msg/ebms/v3.0/core/os/ebms_core-3.0-spec-os.html)

### eb:Messaging

UserMessage blir brukt når innholdet i SOAP-meldingen er en
forretningsmelding. I sikker digial post er type forretningsmelding
definert i [meldingen]({{site.baseurl}}/docs/resources/begrep/ID-porten/index).  
eb:UserMessage skal bygges opp ved å tolke innholdet i meldingen som
skal formidles, samt settinger angitt i
[P-Modes]({{site.baseurl}}/docs/resources/begrep/ID-porten/index)

### Attributter

| Identifikator | Kardinalitet | Datatype | Kommentar |
| --- | --- | --- | --- |
| mpc | 1..1 | xs:anyURI | Konstantverdi som angir kanal som skal benyttes |
| [MessageInfo]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/transportlag/UserMessage/MessageInfo) | 1..1 | eb:MessageInfo | Intern identifikator og timestamp |
| [PartyInfo]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/transportlag/UserMessage/PartyInfo) | 1..1 | eb:PartyInfo | Informasjon om avsender og mottaker |
| [CollaborationInfo]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/transportlag/UserMessage/CollaborationInfo) | 1..1 | eb:CollaborationInfo | Informasjon om avtalt samhandlingsmønster for meldingen |
| [PayloadInfo]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/transportlag/UserMessage/PayloadInfo) | 1..1 | eb:PayloadInfo | Informasjon om selve forretningsmeldingen |

### Eksempel

  - [SOAP forretningsmelding fra avsender til
    meldingsformidler](/resources/begrep/sikkerDigitalPost/eksempler/soap/1_request_forretningsmelding_fra_postavsender_til_meldingsformidler.xml)
