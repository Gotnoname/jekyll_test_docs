--- 
title: Repetisjoner  
permalink: sdp_repitisjoner.html
sidebar: begrep_sidebar
---

|---|---|
| Term | {{page.title}} |
| Definisjon | Gjentagelser etter et bestemt tidspunkt |
| Datatype | complexType |
| Kjelde | DIFI |
| Kommentar | Beskriver hvilke dager noe skal repeteres etter en definert dag, der [dagerEtter](dagerEtter.md) angir hvor mange dager etter tidspunktet det skal repeteres. dagerEtter=0 betyr samme dag. dagerEtter=7 betyr den syvende dagen etter en bestemt dag. Det kreves at alle dagerEtter er unike. For Sikker digital post er repetisjonene knyttet opp til [virkningsdato](virkningsdato.html). Det vil si at dagerEtter=0 betyr samme dag som [virkningsdato](virkningsdato.html). dagerEtter=7 betyr den syvende dagen etter [virkningsdato](virkningsdato.html) |

#### Eigenskapar

| Identifikator                    | Kardinalitet | Datatype               |
| -------------------------------- | ------------ | ---------------------- |
| [dagerEtter](dagerEtter.md) | 0..25        | xsd:nonNegativeInteger |

#### Xml eksempel

``` 
      <repetisjoner>
        <dagerEtter>0</dagerEtter>
        <dagerEtter>7</dagerEtter>
      </repetisjoner>

```
