---
 
title: SAMLAssertionV2  

sidebar:
redirect_from: /idport_samlassertionv2
---
|---|---|
| Identifikator | <https://begrep.difi.no/ID-porten/SAMLAssertionV2> |
| Term          | {{page.title}} |
| Definisjon    | Informasjon om en Person utlevert via ID |
| porten        | dersom Offentlig Virksomhet har tatt i bruk første versjon av kontaktregisteret |
| Datatype      | [SAML\_2.0\_Assertion](http://en.wikipedia.org/wiki/SAML_2.0#SAML_2.0_Assertions) |
| Kilde         | DIFI |
| Kommentar     | FORELDET PROFIL: Den informasjon som utleveres i ID |
| porten        | sin SAML2 profil ved Autentisering dersom Avsender er integrert mot første versjon av kontaktregisteret |

#### Attributer

| Term                     | Beskrivelse                                                                     | Kardinalitet |
| --- | --- | --- |
| uid                      | [personidentifikator]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/begrep/personidentifikator)                              | 1            |
| SecurityLevel            | [sikkerhetsnivaa]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/begrep/sikkerhetsnivaa)                                      | 1            |
| Culture                  | [språk]({{site.baseurl}}/resources/begrep/felles/spraak)                                                         | 1            |
| AuthMethod               | [Autentiseringsmetode]({{site.baseurl}}/resources/begrep/ID-porten/SAMLAssertionV1)                              | 1            |
| Email                    | [epostadresse]({{site.baseurl}}/resources/begrep/sikkerDigitalPost/begrep/epostadresse)                                            | 0..1         |
| MobilePhone              | [mobiltelefonnummer]({{site.baseurl}}/resources/begrep/felles/mobiltelefonnummer)                                | 0..1         |
| DigitalContactInfoStatus | Status                                                                          | 1            |
| OnBehalfOf               | Referanse til annen Offentlig Virksomhet som forespørselen er gjort på vegne av | 0..1         |

#### AuthnContextClassRef

Autentiseringsnivå er spesifisert i henhold til kodeverk for
[AuthnContextClassRef]({{site.baseurl}}/resources/begrep/ID-porten/SAMLAuthnRequest)

#### Kodeverk

##### Status

| DigitalContactInfoStatus | Beskrivelse                                                                                                 |
| --- | --- |
| SAMTYKKET\_GENERELT      | Bruker har samtykket til utlevering av Digital kontaktinformasjon til alle tjenesteeiere                    |
| SAMTYKKET\_SPESIFIKT     | Sluttbruker har samtykket til utlevering av Digital kontaktinformasjon til tjenesteeier.                    |
| IKKE\_SAMTYKKET          | Det er ikke registrert noe samtykke for sluttbruker                                                         |
| SAMTYKKE\_AVVIST         | Bruker har aktivt avvist samtykke om utlevering av Digital kontaktinformasjon                               |
| IKKE\_REGISTRERT         | Sluttbruker er ikke registrert i Digitalt kontaktregister.                                                  |
| SYSTEMFEIL               | ID-porten har ikke informasjon om Digital kontaktinformasjon, f.eks. ved feil i integrasjon mot registrert. |

#### Eksempel

```xml

   <saml:AttributeStatement>
      <saml:Attribute Name="uid">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">03015561903</saml:AttributeValue>
      </saml:Attribute>
      <saml:Attribute Name="Culture">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">nb</saml:AttributeValue>
      </saml:Attribute>
      <saml:Attribute Name="Email">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">03015561903-test@minid.norge.no</saml:AttributeValue>
      </saml:Attribute>
      <saml:Attribute Name="MobilePhone">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">03015561903</saml:AttributeValue>
      </saml:Attribute>   
      <saml:Attribute Name="DigitalContactInfoStatus">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">SAMTYKKET_GENERELT</saml:AttributeValue>
      </saml:Attribute>
      <saml:Attribute Name="AuthMethod">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">Minid-PIN</saml:AttributeValue>
      </saml:Attribute>
      <saml:Attribute Name="SecurityLevel">
         <saml:AttributeValue xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">3</saml:AttributeValue>
      </saml:Attribute>
   </saml:AttributeStatement>

```
