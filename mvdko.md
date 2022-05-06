# mv:dk Data Model

---

1. [Classes](#classes)
2. [Object Properties](#object-properties)

---

## Classes

### mvdko:MediaResource

| mvdko:MediaResource |                 |
| ------------------- | --------------- |
| rdf:type            | owl:Class       |
| rdfs:subClassOf     |                 |
| rdfs:label@en       | Media Resource  |
| rdfs:label@de       | Medienressource |
| skos:definition@de  |                 |
| skos:example@de     |                 |
| rdfs:comment        |                 |

### mvdko:Agent

| mvdko:Agent        |           |
| ------------------ | --------- |
| rdf:type           | owl:Class |
| rdfs:subClassOf    |           |
| rdfs:label@en      | Agent     |
| rdfs:label@de      | Akteur*in |
| skos:definition@de |           |
| skos:example@de    |           |
| rdfs:comment       |           |

### mvdko:RightsStatement

| mvdko:RightsStatement |                  |
| --------------------- | ---------------- |
| rdf:type              | owl:Class        |
| rdfs:subClassOf       |                  |
| rdfs:label@en         | Rights Statement |
| rdfs:label@de         | Rechteangabe     |
| skos:definition@de    |                  |
| skos:example@de       |                  |
| rdfs:comment          |                  |

### mvdko:Location

| mvdko:Location     |           |
| ------------------ | --------- |
| rdf:type           | owl:Class |
| rdfs:subClassOf    |           |
| rdfs:label@en      |           |
| rdfs:label@de      | Ort       |
| skos:definition@de |           |
| skos:example@de    |           |
| rdfs:comment       |           |

### mvdko:Event

| mvdko:Event        |           |
| ------------------ | --------- |
| rdf:type           | owl:Class |
| rdfs:subClassOf    |           |
| rdfs:label@en      | Event     |
| rdfs:label@de      | Ereignis  |
| skos:definition@de |           |
| skos:example@de    |           |
| rdfs:comment       |           |

### mvdko:CreativeConcept

| mvdko:CreativeConcept |                                                                                                                                                                                                                                     |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| rdf:type              | owl:Class                                                                                                                                                                                                                           |
| rdfs:subClassOf       |                                                                                                                                                                                                                                     |
| rdfs:label@en         | Creative Concept                                                                                                                                                                                                                    |
| rdfs:label@de         | Kreatives Konzept                                                                                                                                                                                                                   |
| skos:definition@de    | Klasse für verschiedene Formen von künstlerischen und/oder kreativen Konzepten wie klassischen Schriftwerken, Bühnenwerken, Inszenierungen, Produktionen, Performancekonzepten, etc. im Rahmen der Domäne der Darstellenden Künste. |
| skos:example@de       |                                                                                                                                                                                                                                     |
| rdfs:comment          |                                                                                                                                                                                                                                     |

### mvdko:Person

| mvdko:Person       |             |
| ------------------ | ----------- |
| rdf:type           | owl:Class   |
| rdfs:subClassOf    | mvdko:Agent |
| rdfs:label@en      | Person      |
| rdfs:label@de      | Person      |
| skos:definition@de |             |
| skos:example@de    |             |
| rdfs:comment       |             |

### mvdko:TimeSpan

| mvdko:TimeSpan     |           |
| ------------------ | --------- |
| rdf:type           | owl:Class |
| rdfs:subClassOf    |           |
| rdfs:label@en      | Timespan  |
| rdfs:label@de      | Zeitraum  |
| skos:definition@de |           |
| skos:example@de    |           |
| rdfs:comment       |           |

### mvdko:MediaCarrier

| mvdko:MediaCarrier |               |
| ------------------ | ------------- |
| rdf:type           | owl:Class     |
| rdfs:subClassOf    |               |
| rdfs:label@en      | Media Carrier |
| rdfs:label@de      | Medienträger  |
| skos:definition@de |               |
| skos:example@de    |               |
| rdfs:comment       |               |

### mvdko:Organization

| mvdko:Organization |              |
| ------------------ | ------------ |
| rdf:type           | owl:Class    |
| rdfs:subClassOf    | mvdko:Agent  |
| rdfs:label@en      | Organization |
| rdfs:label@de      | Organisation |
| skos:definition@de |              |
| skos:example@de    |              |
| rdfs:comment       |              |

---

## Object Properties

| mvdko:hasMediumTelevisionStandard |                                             |
| --------------------------------- | ------------------------------------------- |
| rdf:type                          | owl:ObjectProperty; owl:DatatypeProperty    |
| rdfs:label@en                     | has Television Standard                     |
| rdfs:label@de                     | hat TV-Standard                             |
| owl:inverseOf                     | mvdko:isMediumTelevisionStandardOf          |
| rdfs:domain                       |                                             |
| rdfs:range                        |                                             |
| skos:definition@de                |                                             |
| skos:example@de                   |                                             |
| rdfs:comment                      | hasTelevisionStandard hier ausreichend?, MW |

| mvdko:hasLocationOfPublication |                                          |
| ------------------------------ | ---------------------------------------- |
| rdf:type                       | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en                  | has Location of Publication              |
| rdfs:label@de                  | hat Veröffentlichungsort                 |
| owl:inverseOf                  | mvdko:isLocationOfPublicationOf          |
| rdfs:domain                    |                                          |
| rdfs:range                     |                                          |
| skos:definition@de             |                                          |
| skos:example@de                |                                          |
| rdfs:comment                   |                                          |

| mvdko:isMediumChannelOf |                            |
| ----------------------- | -------------------------- |
| rdf:type                | owl:ObjectProperty         |
| rdfs:label@en           | is broadcast channel of    |
| rdfs:label@de           | ist Ausstrahlungskanal von |
| owl:inverseOf           |                            |
| rdfs:domain             |                            |
| rdfs:range              |                            |
| skos:definition@de      |                            |
| skos:example@de         |                            |
| rdfs:comment            |                            |

| mvdko:isMediumEncodingOf |                                   |
| ------------------------ | --------------------------------- |
| rdf:type                 | owl:ObjectProperty                |
| rdfs:label@en            | is medium encoding of             |
| rdfs:label@de            | ist Art der Medienencodierung von |
| owl:inverseOf            |                                   |
| rdfs:domain              |                                   |
| rdfs:range               |                                   |
| skos:definition@de       |                                   |
| skos:example@de          |                                   |
| rdfs:comment             |                                   |

| mvdko:hasMediumEncoding |                                          |
| ----------------------- | ---------------------------------------- |
| rdf:type                | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en           | has Encoding Format                      |
| rdfs:label@de           | hat Encodierungsformat                   |
| owl:inverseOf           | mvdko:isMediumEncodingOf                 |
| rdfs:domain             |                                          |
| rdfs:range              |                                          |
| skos:definition@de      |                                          |
| skos:example@de         |                                          |
| rdfs:comment            | hasEncoding hier ausreichend?, MW        |

| mvdko:hasLocation  |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Location                             |
| rdfs:label@de      | hat Ort                                  |
| owl:inverseOf      | mvdko:isLocationOf                       |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isMediumOf   |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is medium of       |
| rdfs:label@de      | ist Medium von     |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isMediumTelevisionStandardOf |                           |
| ---------------------------------- | ------------------------- |
| rdf:type                           | owl:ObjectProperty        |
| rdfs:label@en                      | is television standard of |
| rdfs:label@de                      | ist Fernsehnorm von       |
| owl:inverseOf                      |                           |
| rdfs:domain                        |                           |
| rdfs:range                         |                           |
| skos:definition@de                 |                           |
| skos:example@de                    |                           |
| rdfs:comment                       |                           |

| mvdko:isVersionOf  |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is version of      |
| rdfs:label@de      | ist Version von    |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasLanguage  |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Language                             |
| rdfs:label@de      | hat Sprache                              |
| owl:inverseOf      | mvdko:isLanguageOf                       |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isIdentifierOf |                    |
| -------------------- | ------------------ |
| rdf:type             | owl:ObjectProperty |
| rdfs:label@en        | is identifier of   |
| rdfs:label@de        | ist Identifier von |
| owl:inverseOf        |                    |
| rdfs:domain          |                    |
| rdfs:range           |                    |
| skos:definition@de   |                    |
| skos:example@de      |                    |
| rdfs:comment         |                    |

| mvdko:hasMediumRegionalCode |                                          |
| --------------------------- | ---------------------------------------- |
| rdf:type                    | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en               | has Regional Code (DVD)                  |
| rdfs:label@de               | hat Regionalcode (DVD)                   |
| owl:inverseOf               | mvdko:isMediumRegionalCodeOf             |
| rdfs:domain                 |                                          |
| rdfs:range                  |                                          |
| skos:definition@de          |                                          |
| skos:example@de             |                                          |
| rdfs:comment                | hasRegionalCode hier ausreichend?, MW    |

| mvdko:hasRole      |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | has Role           |
| rdfs:label@de      | hat Rolle          |
| owl:inverseOf      | mvdko:isRoleOf     |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasSubject   |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Subject                              |
| rdfs:label@de      | hat Thema/Gegenstand                     |
| owl:inverseOf      | mvdko:isSubjectOf                        |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isMediumRegionalCodeOf |                      |
| ---------------------------- | -------------------- |
| rdf:type                     | owl:ObjectProperty   |
| rdfs:label@en                | is regional code of  |
| rdfs:label@de                | ist Regionalcode von |
| owl:inverseOf                |                      |
| rdfs:domain                  |                      |
| rdfs:range                   |                      |
| skos:definition@de           |                      |
| skos:example@de              |                      |
| rdfs:comment                 |                      |

| mvdko:isLanguageOf |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is language of     |
| rdfs:label@de      | ist Sprache von    |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasSource    |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en      | has Source                               |
| rdfs:label@de      | hat Quelle                               |
| owl:inverseOf      | mvdko:isSourceOf                         |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasKeyword   |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Keyword                              |
| rdfs:label@de      | hat Schlagwort                           |
| owl:inverseOf      | mvdko:hasKeyword                         |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasCreator   |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Creator                              |
| rdfs:label@de      | hat Schöpfer*in                          |
| owl:inverseOf      | mvdko:isCreatorOf                        |
| rdfs:domain        | mvdko:CreativeConcept                    |
| rdfs:range         | mvdko:Agent                              |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isCreatorOf  |                     |
| ------------------ | ------------------- |
| rdf:type           | owl:ObjectProperty  |
| rdfs:label@en      | is creator of       |
| rdfs:label@de      | ist Schöpfer*in von |
| owl:inverseOf      |                     |
| rdfs:domain        |                     |
| rdfs:range         |                     |
| skos:definition@de |                     |
| skos:example@de    |                     |
| rdfs:comment       |                     |

| mvdko:hasMediaCarrier |                                          |
| --------------------- | ---------------------------------------- |
| rdf:type              | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en         | has Media Carrier                        |
| rdfs:label@de         | hat Medienträger                         |
| owl:inverseOf         | mvdko:isMediaCarrierOf                   |
| rdfs:domain           |                                          |
| rdfs:range            |                                          |
| skos:definition@de    |                                          |
| skos:example@de       |                                          |
| rdfs:comment          |                                          |

| mvdko:hasRightsHolder |                                          |
| --------------------- | ---------------------------------------- |
| rdf:type              | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en         | has rights holder                        |
| rdfs:label@de         | hat Rechteinhaber*in                     |
| owl:inverseOf         | mvdko:isRightsHolderOf                   |
| rdfs:domain           |                                          |
| rdfs:range            |                                          |
| skos:definition@de    |                                          |
| skos:example@de       |                                          |
| rdfs:comment          |                                          |

| mvdko:isBaseOf     |                                      |
| ------------------ | ------------------------------------ |
| rdf:type           | owl:ObjectProperty                   |
| rdfs:label@en      | is base of                           |
| rdfs:label@de      | ist Vorlage/Inspiration/Einfluss von |
| owl:inverseOf      | mvdko:isBasedOn                      |
| rdfs:domain        |                                      |
| rdfs:range         |                                      |
| skos:definition@de |                                      |
| skos:example@de    |                                      |
| rdfs:comment       |                                      |

| mvdko:isPartOf     |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is part of         |
| rdfs:label@de      | ist Teil von       |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isRightsOf   |                                    |
| ------------------ | ---------------------------------- |
| rdf:type           | owl:ObjectProperty                 |
| rdfs:label@en      | is rights statement/information of |
| rdfs:label@de      | ist Rechteinformation von          |
| owl:inverseOf      |                                    |
| rdfs:domain        |                                    |
| rdfs:range         |                                    |
| skos:definition@de |                                    |
| skos:example@de    |                                    |
| rdfs:comment       |                                    |

| mvdko:isRoleOf     |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is role of         |
| rdfs:label@de      | ist Rolle von      |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasIdentifier |                                          |
| ------------------- | ---------------------------------------- |
| rdf:type            | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en       | has Identifier                           |
| rdfs:label@de       | hat Identifier                           |
| owl:inverseOf       | mvdko:isIdentifierOf                     |
| rdfs:domain         |                                          |
| rdfs:range          |                                          |
| skos:definition@de  |                                          |
| skos:example@de     |                                          |
| rdfs:comment        |                                          |

| mvdko:hasMediumChannel |                                                                                                                                                                                                                                                      |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| rdf:type               | owl:ObjectProperty; owl:DatatypeProperty                                                                                                                                                                                                             |
| rdfs:label@en          | has Publication Channel                                                                                                                                                                                                                              |
| rdfs:label@de          | hat Ausstrahlungskanal/Sender                                                                                                                                                                                                                        |
| owl:inverseOf          | mvdko:isMediumChannelOf                                                                                                                                                                                                                              |
| rdfs:domain            |                                                                                                                                                                                                                                                      |
| rdfs:range             |                                                                                                                                                                                                                                                      |
| skos:definition@de     |                                                                                                                                                                                                                                                      |
| skos:example@de        |                                                                                                                                                                                                                                                      |
| rdfs:comment           | vllt. besser hasDistributionChannel (hasChannel könnte sich auch auf Audioinformationen beziehen), MW hasAudioChannels/hasAudioChannelLayout und hasAudioTrack wären möglicherweise auch zu bedenken (wenn auch bisher nicht in Daten zu finden), MW |

| mvdko:hasRelatedPlace |                        |
| --------------------- | ---------------------- |
| rdf:type              | owl:ObjectProperty     |
| rdfs:label@en         | has related Place      |
| rdfs:label@de         | hat zugehörigen Ort    |
| owl:inverseOf         | mvdko:isRelatedPlaceOf |
| rdfs:domain           |                        |
| rdfs:range            |                        |
| skos:definition@de    |                        |
| skos:example@de       |                        |
| rdfs:comment          |                        |

| mvdko:hasMedium    |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en      | has Medium                               |
| rdfs:label@de      | hat Medium                               |
| owl:inverseOf      | mvdko:isMediumOf                         |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasPlaceOfOccurrence |                                          |
| -------------------------- | ---------------------------------------- |
| rdf:type                   | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en              | has Place of Occurrence                  |
| rdfs:label@de              | hat Ereignisort                          |
| owl:inverseOf              | mvdko:isPlaceOfOccurrenceOf              |
| rdfs:domain                |                                          |
| rdfs:range                 |                                          |
| skos:definition@de         |                                          |
| skos:example@de            |                                          |
| rdfs:comment               |                                          |

| mvdko:isTypeOf     |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is type of         |
| rdfs:label@de      | ist Art von        |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasPart      |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Part                                 |
| rdfs:label@de      | hat Teil                                 |
| owl:inverseOf      | mvdko:isPartOf                           |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isRecordedIn |                      |
| ------------------ | -------------------- |
| rdf:type           | owl:ObjectProperty   |
| rdfs:label@en      | is recorded in       |
| rdfs:label@de      | ist aufgezeichnet in |
| owl:inverseOf      |                      |
| rdfs:domain        |                      |
| rdfs:range         |                      |
| skos:definition@de |                      |
| skos:example@de    |                      |
| rdfs:comment       |                      |

| mvdko:hasTemporalExtent |                                          |
| ----------------------- | ---------------------------------------- |
| rdf:type                | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en           | has temporal Extent                      |
| rdfs:label@de           | hat zeitlichen Umfang                    |
| owl:inverseOf           | mvdko:isTemporalExtentOf                 |
| rdfs:domain             |                                          |
| rdfs:range              |                                          |
| skos:definition@de      |                                          |
| skos:example@de         |                                          |
| rdfs:comment            |                                          |

| mvdko:hasRecordingOf |                                          |
| -------------------- | ---------------------------------------- |
| rdf:type             | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en        | has a Recording of                       |
| rdfs:label@de        | hat Aufzeichnung von                     |
| owl:inverseOf        | mvdko:isRecordedIn                       |
| rdfs:domain          |                                          |
| rdfs:range           |                                          |
| skos:definition@de   |                                          |
| skos:example@de      |                                          |
| rdfs:comment         |                                          |

| mvdko:isSourceOf   |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is source of       |
| rdfs:label@de      | is Quelle von      |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isDateOf     |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is date of         |
| rdfs:label@de      | ist Datum von      |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isMediaCarrierOf |                      |
| ---------------------- | -------------------- |
| rdf:type               | owl:ObjectProperty   |
| rdfs:label@en          | is media carrier of  |
| rdfs:label@de          | ist Medienträger von |
| owl:inverseOf          |                      |
| rdfs:domain            |                      |
| rdfs:range             |                      |
| skos:definition@de     |                      |
| skos:example@de        |                      |
| rdfs:comment           |                      |

| mvdko:isRightsHolderOf |                          |
| ---------------------- | ------------------------ |
| rdf:type               | owl:ObjectProperty       |
| rdfs:label@en          | is rights holder of      |
| rdfs:label@de          | ist Rechteinhaber*in von |
| owl:inverseOf          |                          |
| rdfs:domain            |                          |
| rdfs:range             |                          |
| skos:definition@de     |                          |
| skos:example@de        |                          |
| rdfs:comment           |                          |

| mvdko:isContributorOf |                       |
| --------------------- | --------------------- |
| rdf:type              | owl:ObjectProperty    |
| rdfs:label@en         | is contributor of     |
| rdfs:label@de         | ist Mitwirkende*r von |
| owl:inverseOf         |                       |
| rdfs:domain           |                       |
| rdfs:range            |                       |
| skos:definition@de    |                       |
| skos:example@de       |                       |
| rdfs:comment          |                       |

| mvdko:hasDate      |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has Date Information                     |
| rdfs:label@de      | hat Datumsangabe                         |
| owl:inverseOf      | mvdko:isDateOf                           |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasType      |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en      | has Type                                 |
| rdfs:label@de      | hat Typ                                  |
| owl:inverseOf      | mvdko:isTypeOf                           |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasVersion   |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en      | has Version                              |
| rdfs:label@de      | hat Version                              |
| owl:inverseOf      | mvdko:isVersionOf                        |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isSubjectOf  |                          |
| ------------------ | ------------------------ |
| rdf:type           | owl:ObjectProperty       |
| rdfs:label@en      | is subject of            |
| rdfs:label@de      | ist Thema/Gegenstand von |
| owl:inverseOf      |                          |
| rdfs:domain        |                          |
| rdfs:range         |                          |
| skos:definition@de |                          |
| skos:example@de    |                          |
| rdfs:comment       |                          |

| mvdko:isTemporalExtentOf |                               |
| ------------------------ | ----------------------------- |
| rdf:type                 | owl:ObjectProperty            |
| rdfs:label@en            | is tempral extent/duration of |
| rdfs:label@de            | ist Dauer von                 |
| owl:inverseOf            |                               |
| rdfs:domain              |                               |
| rdfs:range               |                               |
| skos:definition@de       |                               |
| skos:example@de          |                               |
| rdfs:comment             |                               |

| mvdko:hasFunction  |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | has Function       |
| rdfs:label@de      | hat Funktion       |
| owl:inverseOf      | mvdko:isFunctionOf |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isKeywordOf  |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is keyword of      |
| rdfs:label@de      | ist Schlagwort von |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isPlaceOfOccurrenceOf |                           |
| --------------------------- | ------------------------- |
| rdf:type                    | owl:ObjectProperty        |
| rdfs:label@en               | is place of occurrence of |
| rdfs:label@de               | ist Veranstaltungsort von |
| owl:inverseOf               |                           |
| rdfs:domain                 |                           |
| rdfs:range                  |                           |
| skos:definition@de          |                           |
| skos:example@de             |                           |
| rdfs:comment                |                           |

| mvdko:isLocationOf |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is location of     |
| rdfs:label@de      | ist Ort von        |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasPlaceOfResidence |                                          |
| ------------------------- | ---------------------------------------- |
| rdf:type                  | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en             | has Place of Residence                   |
| rdfs:label@de             | hat Residenzort                          |
| owl:inverseOf             | mvdko:isPlaceOfResidenceOf               |
| rdfs:domain               |                                          |
| rdfs:range                |                                          |
| skos:definition@de        |                                          |
| skos:example@de           |                                          |
| rdfs:comment              |                                          |

| mvdko:isFunctionOf |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is function of     |
| rdfs:label@de      | ist Funktion von   |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:isBasedOn    |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:ObjectProperty; owl:DatatypeProperty |
| rdfs:label@en      | is Based on                              |
| rdfs:label@de      | ist basiert auf                          |
| owl:inverseOf      |                                          |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasMediumDate |                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| rdf:type            | owl:DatatypeProperty; owl:ObjectProperty                                                         |
| rdfs:label@en       |                                                                                                  |
| rdfs:label@de       |                                                                                                  |
| owl:inverseOf       | mvdko:isMediumDateOf                                                                             |
| rdfs:domain         |                                                                                                  |
| rdfs:range          |                                                                                                  |
| skos:definition@de  |                                                                                                  |
| skos:example@de     |                                                                                                  |
| rdfs:comment        | Könnte diese Proeprty durch hasDate ersetzt werden?, MW; Als Subproperty von hasDate denkbar. MW |

| mvdko:isPlaceOfResidenceOf |                          |
| -------------------------- | ------------------------ |
| rdf:type                   | owl:ObjectProperty       |
| rdfs:label@en              | is place of residence of |
| rdfs:label@de              | ist Residentort von      |
| owl:inverseOf              |                          |
| rdfs:domain                |                          |
| rdfs:range                 |                          |
| skos:definition@de         |                          |
| skos:example@de            |                          |
| rdfs:comment               |                          |

| mvdko:isLocationOfPublicationOf |                               |
| ------------------------------- | ----------------------------- |
| rdf:type                        | owl:ObjectProperty            |
| rdfs:label@en                   | is location of publication of |
| rdfs:label@de                   | ist Veröffentlichungsort von  |
| owl:inverseOf                   |                               |
| rdfs:domain                     |                               |
| rdfs:range                      |                               |
| skos:definition@de              |                               |
| skos:example@de                 |                               |
| rdfs:comment                    |                               |

| mvdko:isMediumDateOf |                      |
| -------------------- | -------------------- |
| rdf:type             | owl:ObjectProperty   |
| rdfs:label@en        | is medium date of    |
| rdfs:label@de        | ist Datumsangabe von |
| owl:inverseOf        |                      |
| rdfs:domain          |                      |
| rdfs:range           |                      |
| skos:definition@de   |                      |
| skos:example@de      |                      |
| rdfs:comment         |                      |

| mvdko:hasEvent     |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has corresponding Event                  |
| rdfs:label@de      | hat zugehöriges Ereignis                 |
| owl:inverseOf      | mvdko:isEventOf                          |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:hasContributor |                                          |
| -------------------- | ---------------------------------------- |
| rdf:type             | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en        | has Contributor                          |
| rdfs:label@de        | hat Mitwirkende*n                        |
| owl:inverseOf        | mvdko:isContributorOf                    |
| rdfs:domain          |                                          |
| rdfs:range           |                                          |
| skos:definition@de   |                                          |
| skos:example@de      |                                          |
| rdfs:comment         |                                          |

| mvdko:isEventOf    |                    |
| ------------------ | ------------------ |
| rdf:type           | owl:ObjectProperty |
| rdfs:label@en      | is event of        |
| rdfs:label@de      | ist Ereignis von   |
| owl:inverseOf      |                    |
| rdfs:domain        |                    |
| rdfs:range         |                    |
| skos:definition@de |                    |
| skos:example@de    |                    |
| rdfs:comment       |                    |

| mvdko:hasRights    |                                          |
| ------------------ | ---------------------------------------- |
| rdf:type           | owl:DatatypeProperty; owl:ObjectProperty |
| rdfs:label@en      | has rights information                   |
| rdfs:label@de      | hat Rechteangabe                         |
| owl:inverseOf      | mvdko:isRightsOf                         |
| rdfs:domain        |                                          |
| rdfs:range         |                                          |
| skos:definition@de |                                          |
| skos:example@de    |                                          |
| rdfs:comment       |                                          |

| mvdko:isRelatedPlaceOf |                                    |
| ---------------------- | ---------------------------------- |
| rdf:type               | owl:ObjectProperty                 |
| rdfs:label@en          | is related place of                |
| rdfs:label@de          | ist zugehöriger/relevanter Ort von |
| owl:inverseOf          |                                    |
| rdfs:domain            |                                    |
| rdfs:range             |                                    |
| skos:definition@de     |                                    |
| skos:example@de        |                                    |
| rdfs:comment           |                                    |
