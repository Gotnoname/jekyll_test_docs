---

title: FormidleDigitalPostForsendelse  

sidebar: dpi_sidebar
redirect_from: /sdp_formidledigitalpostforsendelse
---

## {{page.title }}

Mal/URI for P-Mode parametere som skal benyttes ved forretningsprosessen
FormidleDigitalPostForsendelse. Oversikten er basert på P-Mode
parametere som en AS4 Light Compliant MSH skal kunne forstå, men det er
ikke alle av disse som er relevante for et Sikker Digital Post. Disse er
markert med - ikke relevant -

Malen inneholder enkelte variabler som skal fylles ved instansiering av
et variabelsett. For disse er formen %variabelnavn% benyttet.

### Generelle parametere

| P-Mode | Beskrivelse | Verdi |
| --- | --- | --- |
| PMode.ID | Unik identifikator for paramtersettet | %[Sender]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/forretningslag/StandardBusinessDocument/Sender)%-"FormidleDigitalPostForsendelse"-%versjon/løpenummer%) |
| PMode.Agreement | Unik identifikator for samarbeidsprotokollen | ["http://begrep.difi.no/SikkerDigitalPost/1.0/transportlag/Meldingsutveksling/FormidleDigitalPostForsendelse"]({{pageMinorUrl}}) |
| PMode.MEP | Message Exchange Pattern | “http://www.oasis-open.org/committees/ebxml-msg/one-way” |
| PMode.MEPbinding | Retning på kommunikasjon, push eller pull | “http://www.oasis-open.org/committees/ebxml-msg/push” |
| PMode.Initiator.Party | Identifikator for den som initierar sendingen | %[Sender]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/forretningslag/StandardBusinessDocument/Sender)% |
| PMode.Initiator.Role | Rolle for den som initierar sendinga | [”Avsender“]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/begrep/Avsender) |
| PMode.Initiator.Authorization.username | \- ikke relevant - | \- ikke relevant - |
| PMode.Initiator.Authorization.password | \- ikke relevant - | \- ikke relevant - |
| PMode.Responder.Party | Identifikator for den som er mottaker | %[Receiver]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/forretningslag/StandardBusinessDocument/Receiver)% |
| PMode.Responder.Role | Rolle for den som mottar | “urn:sdp:meldingsformidler” |
| PMode.Responder.Authorization.username | \- ikke relevant - | \- ikke relevant - |
| PMode.Responder.Authorization.password | \- ikke relevant - | \- ikke relevant - |

### Protokoll

| P-Mode | Beskrivelse | Verdi |
| --- | --- | --- |
| PMode\[1\].Protocol.Address | | “HTTPS 1.1” |
| PMode\[1\].Protocol.SOAPVersion | | “SOAP 1.2”  |

### BusinessInfo

| P-Mode | Verdi |
| --- | --- |
| PMode\[1\].BusinessInfo.Service | “urn:sdp:service:sdp” |
| PMode\[1\].BusinessInfo.Action | “FormidleDigitalPost” |
| PMode\[1\].BusinessInfo.Properties\[\]: | \- ikke relevant - |

### ErrorHandling

| P-Mode | Verdi |
| --- | --- |
| PMode\[1\].ErrorHandling.Report.AsResponse | true  |
| PMode\[1\].ErrorHandling.Report.ProcessErrorNotifyProducer | true  |
| PMode\[1\].ErrorHandling.Report.DeliveryFailuresNotifyProducer | true  |

### Pålitlighet

Støtte ikke påkrevd i profilen.

### Sikkerhet

| P-Mode | Verdi |
| ---| --- |
| PMode\[1\].Security.WSSVersion | “1.1” |
| PMode\[1\].Security.X509.Sign | Timestamp, eb:Messaging, SOAP Body, Attachment |
| PMode\[1\].Security.X509.Signature.Certificate | %[Sender]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/forretningslag/StandardBusinessDocument/Sender) sitt sertifikat% |
| PMode\[1\].Security.X509.Signature.HashFunction | “SHA-256” |
| PMode\[1\].Security.X509.Signature.Algorithm | “RSA-SHA256” |
| PMode\[1\].Security.X509.Encryption.Encrypt | \- ikke relevant - |
| PMode\[1\].Security.X509.Encryption.Certificate | \- ikke relevant - |
| PMode\[1\].Security.X509.Encryption.Algorithm | \- ikke relevant - |
| PMode\[1\].Security.X509.Encryption.MinimumStrength | \- ikke relevant - |
| PMode\[1\].Security.UsernameToken.username | \- ikke relevant - |
| PMode\[1\].Security.UsernameToken.password | \- ikke relevant - |
| PMode\[1\].Security.UsernameToken.Digest | \- ikke relevant - |
| PMode\[1\].Security.UsernameToken.Nonce | \- ikke relevant - |
| PMode\[1\].Security.UsernameToken.Created | \- ikke relevant - |
| PMode\[1\].Security.PModeAuthorize | false |
| PMode\[1\].Security.SendReceipt | |
| Pmode\[1\].Security.SendReceipt.ReplyPattern | |

### Eksempler

[request_forretningsmelding_fra_postavsender_til_meldingsformidler](https://difi.github.io/felleslosninger/resources/begrep/sikkerDigitalPost/eksempler/soap/1_request_forretningsmelding_fra_postavsender_til_meldingsformidler.xml)
