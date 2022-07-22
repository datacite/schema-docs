Appendix 6:  PIDINST Schema [36]_ Mapping
=================================================================

.. _Table 4:

Table 4: PIDINST to DataCite Mapping
------------------------------------------------------

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Identifier                 | Identifier                                       |
+----------------------------+--------------------------------------------------+
| identifierType             | identifierType ‘DOI’                             |
+----------------------------+--------------------------------------------------+
| Name                       | Title                                            |
+----------------------------+--------------------------------------------------+
| Owner                      | Contributor                                      |
+----------------------------+--------------------------------------------------+
| ownerName                  | ContributorName                                  |
+----------------------------+--------------------------------------------------+
|                            | ContributorType                                  |
+----------------------------+--------------------------------------------------+
| ownerIdentifier            | nameIdentifier                                   |
+----------------------------+--------------------------------------------------+
| ownerIdentifierType        | nameIdentifierScheme                             |
+----------------------------+--------------------------------------------------+
| Manufacturer               | Creator                                          |
+----------------------------+--------------------------------------------------+
| manufacturerName           | creatorName                                      |
+----------------------------+--------------------------------------------------+
| manufacturerIdentifier     | nameIdentifier                                   |
+----------------------------+--------------------------------------------------+
| manufacturerIdentifierType | nameIdentifierScheme                             |
+----------------------------+--------------------------------------------------+
| Model                      | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| modelName                  | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| modelIdentifier            | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| modelIdentifierType        | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| Description                | Description with descriptionType ‘Abstract’      |
+----------------------------+--------------------------------------------------+
| InstrumentType             | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| instrumentTypeName         | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| instrumentTypeIdentifier   | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| MeasuredVariable           | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+
| Date                       | Date                                             |
+----------------------------+--------------------------------------------------+
| dateType                   | dateType                                         |
+----------------------------+--------------------------------------------------+
| RelatedIdentifier          | RelatedIdentifier                                |
+----------------------------+--------------------------------------------------+
| relatedIdentifierType      | relatedIdentifierType                            |
+----------------------------+--------------------------------------------------+
| relationType               | relationType                                     |
+----------------------------+--------------------------------------------------+
|                            | Describes, IsDescribedBy                         |
+----------------------------+--------------------------------------------------+
|                            | IsNewVersionOf, IsPreviousVersionOf              |
+----------------------------+--------------------------------------------------+
|                            | HasPart, IsPartOf                                |
+----------------------------+--------------------------------------------------+
|                            | HasMetadata, IsMetadataFor                       |
+----------------------------+--------------------------------------------------+
|                            | Uses, IsUsedBy                                   |
+----------------------------+--------------------------------------------------+
| AlternateIdentifier        | AlternateIdentifier                              |
+----------------------------+--------------------------------------------------+
| alternateIdentifierType    | alternateIdentifierType                          |
+----------------------------+--------------------------------------------------+

Comments
------------------------------------------------------

Name / Title
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Name                       | Title                                            |
+----------------------------+--------------------------------------------------+

May be the title of a dataset, the name of a piece of software or instrument.

Owner / Contributor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Owner                      | Contributor                                      |
+----------------------------+--------------------------------------------------+

Can be used for the owner of an instrument, i.e. the institution responsible for the management of the instrument. This may include the legal owner, the operator, or an institute providing access to the instrument. Use the contributorType “hostingInstitution”.


Manufacturer / Creator
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Manufacturer               | Creator                                          |
+----------------------------+--------------------------------------------------+

The instrument’s manufacturer(s) or developer. This may also be the owner for custom-build instruments.

Model / Description with descriptionType ‘TechnicalInfo’
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Model                      | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+

Detailed information associated with an instrument instance, e.g. model (model name and model identifier), instrument type (name and identifier), or measured variable.


Description / Description with descriptionType ‘Abstract’
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Description                | Description with descriptionType ‘Abstract’      |
+----------------------------+--------------------------------------------------+

Technical description of the device and its capabilities.

MeasuredVariable / Description with descriptionType ‘TechnicalInfo’
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| MeasuredVariable           | Description with descriptionType ‘TechnicalInfo’ |
+----------------------------+--------------------------------------------------+

The variable(s) that this instrument measures or observes.

Date / Date
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| Date                       | Date                                             |
+----------------------------+--------------------------------------------------+
| dateType                   | dateType                                         |
+----------------------------+--------------------------------------------------+

Dates relevant to the instrument.

To indicate the date when the instrument started to be in operation (Commissioned), or ceased to be in operation (DeCommissioned), use dateType ‘Other’ and add ‘Commissioned’ resp. ‘Decommissioned’ in dateInformation.


relationType / relationType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| relationType               | relationType                                     |
+----------------------------+--------------------------------------------------+
|                            | Describes, IsDescribedBy                         |
+----------------------------+--------------------------------------------------+
|                            | IsNewVersionOf, IsPreviousVersionOf              |
+----------------------------+--------------------------------------------------+
|                            | HasPart, IsPartOf                                |
+----------------------------+--------------------------------------------------+
|                            | HasMetadata, IsMetadataFor                       |
+----------------------------+--------------------------------------------------+
|                            | Uses, IsUsedBy                                   |
+----------------------------+--------------------------------------------------+

RelationTypes applicable to instruments.

**Describes, IsDescribedBy**: The linked resource is a document describing the instrument.

*sNewVersionOf, IsPreviousVersionOf**: If an instrument is substantially modified, a new DOI may be attributed to the new version. In that case the old and the new DOI should be linked to each other. IsNewVersionOf should be used in the new DOI record to link the old instrument before the modification.

**HasPart, IsPartOf**: In the case of a complex instrument, having multiple components that may be considered as instruments in their own right, with their own DOIs, these DOIs should be linked. HasPart should be used in the DOI record of the compound instrument to link the components. IsPartOf should be used in the DOI records of the components to link the compound instrument.

**HasMetadata, IsMetadataFor**: If there is additional metadata describing the instrument, possibly using a community specific metadata standard, that metadata record may be linked using HasMetadata.

**Uses, IsUsedBy**: If the instrument has been deployed in some research activity, such as a cruise or a research vessel, IsUsedBy may be used to link that activity.


AlternateIdentifier / AlternateIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+--------------------------------------------------+
| PIDINST Property           | DataCite v. 4.5                                  |
+============================+==================================================+
| AlternateIdentifier        | AlternateIdentifier                              |
+----------------------------+--------------------------------------------------+
| alternateIdentifierType    | alternateIdentifierType                          |
+----------------------------+--------------------------------------------------+

May be used for the instrument's serial number. Other possible uses include an owner’s inventory number or an entry in some instrument database.

The type of the AlternateIdentifier.

.. rubric:: Footnotes
.. [36] Krahl, R., Darroch, L., Huber, R., Devaraju, A., Klump, J., Habermann, T., Stocker, M., & The Research Data Alliance Persistent Identification of Instruments Working Group members (2022). Metadata Schema for the Persistent Identification of Instruments (1.0). Research Data Alliance. https://doi.org/10.15497/RDA00070
