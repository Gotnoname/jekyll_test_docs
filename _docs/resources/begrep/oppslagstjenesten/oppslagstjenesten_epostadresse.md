---
title: Epostadresse  

sidebar:
---

| --- | --- |
| Identifikator  | http://begrep.difi.no/Oppslagstjenesten/5.0.0/5.0/Epostadresse |
|Term | Epostadresse |
| Definisjon  | Informasjon om en Person sitt Epostadresse registrert i kontakt og reservasjonsregisteret |
| Datatype  | complexType |
| Kilde | DIFI |
| Kommentar | Informasjon om en Person sitt Epostadresse registrert i kontakt og reservasjonsregisteret. Epost-addressen blir validert vha. biblioteket [ApacheCommons](http://commons.apache.org/proper/commons-validator/) |

#### Attributer

| --- | --- |
| Term | Kardinalitet |
| [epostadresse]({{site.baseurl}}/docs/resources/begrep/sikkerDigitalPost/begrep/epostadresse)     | 0..1 |
| [sistOppdatert]({{site.baseurl}}/docs/resources/begrep/felles/sistOppdatert)   | 0..1 |
| [sistVerifisert]({{site.baseurl}}/docs/resources/begrep/felles/sistVerifisert) | 0..1 |
 



#### Xml eksempel

```
<ns2:Epostadresse sistOppdatert="2014-02-25T13:08:00.000+01:00" sistVerifisert="2013-10-21T10:09:28.000+02:00">01012295312_test@minid.difi.no</ns2:Epostadresse>
```
