Appendix 2: Earlier Version Update Notes
==========================================

Appendix 2 provides the update contents of earlier versions of the schema.

Version 4.3 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.3 of the schema includes these changes:

* Addition of new subproperties for Affiliation in the ``Creator`` and ``Contributor`` properties:

  * affiliationIdentifier
  * affiliationIdentifierScheme
  * schemeURI
* Addition of a new subproperty “schemeURI” for funderIdentifier of the ``FundingReference`` property.
* Addition of “ROR” to the controlled list values of funderIdentifierType of the ``FundingReference`` property.

Version 4.3 of the documentation includes these changes:

* Addition of “ROR” and “GRID” as examples of nameIdentifierScheme and schemeURI of the properties ``Creator`` and ``Contributor``.
* Addition of a usage note to the “affiliation” subproperty of ``Creator`` and ``Contributor``.
* Addition of a note to the Date property and “dateInformation” subproperty on the use of dates in ancient history.
* Broadening of the description of dateType “Created” with dates in ancient history (see Appendix 1, Table 6)
* Amendment of the hierarchical numbering of the metadata properties to align with the schema XSD.
* Removal of brackets in the guidance regarding unknown values.

Version 4.2 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.2 of the schema includes these changes:

* Addition of new dateType “Withdrawn”
* Addition of new relationType pair: IsObsoletedBy and Obsoletes
* Addition of new relatedIdentifierType “w3id”
* Addition of new subproperties for Rights:

  * rightsIdentifier
  * rightsIdentifierScheme
  * schemeURI

* Addition of the XML language attribute to the properties ``Creator``, ``Contributor`` and ``Publisher`` for organizational names.

Version 4.2 of the documentation includes these changes:

* Addition of “data management plan” and “conference paper” as examples to the description of resourceTypeGeneral “Text” (see Appendix 1, Table 7).
* Addition of a usage note to the relationType pair “Compiles/IsCompiledBy” (see Appendix 1, Table 9).
* Addition of a reference to the DataCite Event Data service to the description of the relatedIdentifier property.
* Addition of subproperty “resourceTypeGeneral” to relatedIdentifier.
* Notes on the coverage and scope of the metadata schema, and the preferred language in which the metadata should be provided.

Version 4.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.1 of the schema includes these changes:

* Allowing multiple polygons per GeoLocation
* Addition of new optional subproperties for polygon

  * inPolygonPoint
* Addition of new dateType “Other”
* Addition of new subproperty for Date

  * dateInformation
* Addition of a new resourceType "DataPaper"
* Addition of three new relationType pairs:

  * IsDescribedBy and Describes
  * HasVersion and IsVersionOf
  * IsRequiredBy and Requires
* Addition of a new optional attribute for creatorName and ContributorName:

  * nameType. Controlled list: personal, organizational
* Addition of a new optional attribute for relatedIdentifier

  * resourceTypeGeneral. Controlled list is identical to existing resourceTypeGeneral attribute
* Addition of optional lang attribute to Rights property
* Change to the definition of Collection to encompass collections of one resourceType as well as those of mixed types.
* Inclusion of a reference to the Research Data Alliance (RDA)-recommended dynamic data citation approach in documentation in section 2.2, Citation.
* Change to the definition and examples of Size property to include duration as well as extent.
* Correction of the hierarchy of elements for Creator and Contributor.
* To enhance support for software citation, addition of 2 new appendices: one with a list of all the changes and explanatory notes; and one with Force11 mappings
* Changes and additions to these definitions, in support of software citation:

  * Identifier
  * Title
  * Publisher
  * Contributor
  * PublicationYear
  * resourceTypeGeneral (Service, Software)
  * relationType pairs (IsPartOf, HasPart, IsDocumentedBy, Documents, IsVariantFormOf, IsOriginalFormOf)
  * Version
  * Rights
  * Description (TechnicalInfo)

Version 4.0 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.0 of the schema includes these changes:

* Allowing more than one nameIdentifier per creator or contributor
* Addition of new optional subproperties for creatorName and contributorName

  * givenName
  * familyName
* Addition of new titleType “Other”
* Addition of new subproperty for subjectScheme

  * subjectScheme

     * valueURI
* Changing resourceTypeGeneral from optional to mandatory
* Addition of a new relatedIdentifierType option “IGSN”
* Addition of a new descriptionType "TechnicalInfo"
* Addition of a new subproperty for GeoLocation “geoLocationPolygon”
* Changing the definition of the existing GeoLocation sub properties (geoLocationPoint, and geoLocationBox)
* Addition of a new property: FundingReference, with subproperties

  * funderName
  * funderIdentifier

     * funderIdentifierType

  * awardNumber
  * awardURI
  * awardTitle
* Deprecation of contributorType “funder” (as a result of adding the new property “FundingReference”)

Version 4.0 of the documentation includes these changes:

* Provision of a link to guidelines for how to write the ORCID ID (See properties 2.2.1 and 7.3.1 nameIdentifierScheme)
* Adjustment of the instructions for resourceTypeGeneral option “collection” (See Appendix 1, Table 7)

Note that, while the property resourceType has been relocated in the documentation to the mandatory property section, it retains its original numbering (10).

Version 3.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 3.1 of the schema includes these changes:

* New affiliation attribute for Creator and Contributor
* New relationType pairs

  * IsReviewedBy and Reviews
  * IsDerivedFrom and IsSourceOf
* New contributorType: DataCurator
* New relatedIdentifierTypes:

  * arXiv
  * bibcode

Version 3.1 of the documentation includes these changes:

* Documentation for the new affiliation attributes for Creator and Contributor
* Special notes about support for long lists of names (Creator and Contributor)
* Additional guidance for:

  * Recording Publication Year
  * Handling the digitised version of physical object
  * Handling missing mandatory property values, including standard values table
* Documentation for the new contributorType: DataCurator
* Documentation for the two new relatedIdentifierTypes:

  * arXiv
  * bibcode
* Documentation, including examples, for the new relationType pairs:

  * IsReviewedBy and Reviews
  * IsDerivedFrom and IsSourceOf
* Correction of link errors in 3.0 documentation

Version 3.0 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 3.0 of the DataCite Metadata Schema included these changes [32]_.

* Correction of a problem with our way of depicting dates by

  * implementing RKMS-ISO8601 [33]_ standard for depicting date ranges, so that a range is indicated as follows: 2004-03-02/2005-06-02
  * deleting ``startDate`` and ``endDate`` date types, and derogating these from earlier versions

* Addition of a new ``GeoLocation`` property, with the sub-properties ``geoLocationPoint``, ``geoLocationBox``, ``geoLocationPlace`` supporting a simple depiction of geospatial information, as well as a free text description.
* Addition of new values to controlled lists:

  * ``contributorType``: ResearchGroup and Other
  * ``dateType``: Collected
  * ``resourceTypeGeneral`` : Audiovisual, Workflow, and Other and derogation of Film
  * ``relatedIdentifierType``: PMID
  * ``relationType``: IsIdenticalTo (indicates that A is identical to B, for use when there is a need to register two separate instances of the same resource)
  * ``relationType``: HasMetadata, (indicates resource A has additional metadata B and indicates), IsMetadataFor (indicates additional metadata A for resource B)
  * ``descriptionType``: Methods
* Deletion of the derogated ``resourceType``: film
* new sub-properties for ``relationType``: ``relatedMetadataSchema``, ``schemeURI`` and ``schemaType``, to be used only for the new ``relationType`` pair of ``HasMetadata``, ``IsMetadataFor``
* Addition of ``schemeURI`` sub-property to the ``nameIdentifierScheme`` associated with ``CreatorName``, ``ContributorName`` and ``Subject``
* Addition of the ``rightsURI`` sub-property to ``Rights``; ``Rights`` is now repeatable (within wrapper element ``rightsList``).
* Implementation of the xml:lang attribute [34]_ that can be used on the properties ``Title``, ``Subject`` and ``Description``.
* Removal of two system-generated administrative metadata fields: ``LastMetadataUpdate`` and ``MetadataVersionNumber`` because both values are tracked in another way now.


Version 3.0 of the DataCite Metadata Schema documentation included these changes:

* Updates to the introductory information
* Provision of greater detail, explanatory material and definitions for controlled lists
* Indication of recommended metadata, in addition to mandatory and optional
* Addition of more and more varied XML examples on the Metadata Schema website
* Removal from documentation of information about administrative metadata (which cannot be edited by contributors).

Version 2.2 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 2.2 of the DataCite Metadata Schema introduced several changes, as noted below:

* Addition of “URL” to list of allowed values for ``relatedIdentifierType``
* Addition of the following values to list of allowed values for ``contributorType``: Producer, Distributor, RelatedPerson, Supervisor, Sponsor, Funder, RightsHolder
* Addition of “SeriesInformation” to list of allowed values for ``descriptionType``
* Addition of “Model” to list of allowed values for ``resourceTypeGeneral``

Version 2.2 of the DataCite Metadata Schema documentation included these changes:

* Provision of more examples of xml for different types of resources
* Explanation of the ``PublicationYear`` property in consideration of the requirements of citation. A change to the definition of the Publisher property, which now reads, “The name of the entity that holds, archives, publishes, prints, distributes, releases, issues, or produces the resource. This property will be used to formulate the citation, so consider the prominence of the role.”

Version 2.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 2.1 of the DataCite Metadata Schema introduced several changes, as noted below:

* Addition of a namespace (http://schema.datacite.org/namespace) to the schema in order to support OAI PMH compatibility
* Enforcement of content for mandatory properties
* New type for the ``Date`` property to conform with the specification that it handles both YYYY and YYYY-MM-DD values

Version 2.1 of the DataCite Metadata Schema documentation included these changes:

* Addition of a column to the Mandatory and Optional Properties tables providing an indicator of whether the property being described is an attribute or a child of the corresponding property that has preceded it
* Revision of the allowed values description for the attribute 12.2 ``relationType``. These have been reviewed and rewritten for increased clarity. In several cases, corrections to the definitions occurred.


.. rubric:: Footnotes
.. [32] Two additional schema code level changes are the allowance of keeping optional wrapper elements empty and the allowance of arbitrary ordering of elements (by removal of <xs:sequence>).
.. [33] The standard is documented here: http://www.ukoln.ac.uk/metadata/dcmi/collection-RKMS-ISO8601/
.. [34] Allowed values IETF BCP 47, ISO 639-1 language codes, e.g. en, de, fr
