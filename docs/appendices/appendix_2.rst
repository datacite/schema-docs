Appendix 2: Earlier Version Update Notes
==========================================

Appendix 2 provides the update contents of earlier versions of the schema.

Version 4.4 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Addition of the new subproperty :ref:`6.d` in the :ref:`6` property.
* Addition of new values to the :ref:`10.a` property:

 * :ref:`Book`
 * :ref:`BookChapter`
 * :ref:`ComputationalNotebook`
 * :ref:`ConferencePaper`
 * :ref:`ConferenceProceeding`
 * :ref:`Dissertation`
 * :ref:`Journal`
 * :ref:`JournalArticle`
 * :ref:`OutputManagementPlan`
 * :ref:`PeerReview`
 * :ref:`Preprint`
 * :ref:`Report`
 * :ref:`Standard`

* Addition of a new relationType: :ref:`IsPublishedIn` (indicates that A is published in B)
* Addition of a new :ref:`20` property, with subproperties to contain specific details for containing publication information previously encoded in a :ref:`17` field with ``descriptionType=”SeriesInformation”`` (for example, to define the journal name, volume, and page number for an article resource). Subproperties:

 * :ref:`20.b`
 * :ref:`20.a`
 * :ref:`20.1`
 * :ref:`20.1.a`
 * :ref:`20.2`
 * :ref:`20.3`
 * :ref:`20.4`
 * :ref:`20.5`
 * :ref:`20.6`
 * :ref:`20.7`
 * :ref:`20.8`
 * :ref:`20.9`
 * :ref:`20.10`
 * :ref:`20.11`
 * :ref:`20.12`

Major Documentation changes:

* The title of this document has changed to: *DataCite Metadata Schema Documentation for the Publication and Citation for Research Data and Other Research Outputs*.
* Following community feedback and suggestions, this version includes further clarification as regards the following contributorTypes: :ref:`DataManager`, :ref:`DataCurator`, :ref:`ResearchGroup`, and :ref:`HostingInstitution`.


Version 4.3 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.3 of the schema includes these changes:

* Addition of new subproperties for affiliation (:ref:`2.5 <2.5>`, :ref:`7.5 <7.5>`) in the :ref:`2` and :ref:`7` properties:

  * affiliationIdentifier (:ref:`2.5.a <2.5.a>`, :ref:`7.5.a <7.5.a>`)
  * affiliationIdentifierScheme (:ref:`2.5.b <2.5.b>`, :ref:`7.5.b <7.5.b>`)
  * schemeURI (:ref:`2.5.c <2.5.c>`, :ref:`7.5.c <7.5.c>`)
* Addition of a new subproperty :ref:`19.2.b` for :ref:`19.2` of the :ref:`19` property.
* Addition of “ROR” to the controlled list values of :ref:`19.2.a` of the :ref:`19` property.

Version 4.3 of the documentation includes these changes:

* Addition of “ROR” and “GRID” as examples of nameIdentifierScheme (:ref:`2.4.a <2.4.a>`, :ref:`7.4.a <7.4.a>`) and schemeURI (:ref:`2.4.b <2.4.b>`, :ref:`7.4.b <7.4.b>`) of the properties :ref:`2` and :ref:`7`.
* Addition of a usage note to the affiliation (:ref:`2.5 <2.5>`, :ref:`7.5 <7.5>`) subproperty of :ref:`2` and :ref:`7`.
* Addition of a note to the :ref:`8` property and :ref:`8.b` subproperty on the use of dates in ancient history.
* Broadening of the description of dateType :ref:`Created` with dates in ancient history (see :doc:`Appendix 1: Controlled List Definitions - dateType </appendices/appendix_1/dateType>`)
* Amendment of the hierarchical numbering of the metadata properties to align with the schema XSD.
* Removal of brackets in the guidance regarding unknown values.

Version 4.2 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.2 of the schema includes these changes:

* Addition of new dateType :ref:`Withdrawn`
* Addition of new relationType pair: :ref:`IsObsoletedBy` and :ref:`Obsoletes`
* Addition of new relatedIdentifierType :ref:`w3id`
* Addition of new subproperties for :ref:`16`:

  * :ref:`16.b`
  * :ref:`16.c`
  * :ref:`16.d`

* Addition of the XML language attribute to the properties :ref:`2`, :ref:`7` and :ref:`4` for organizational names.

Version 4.2 of the documentation includes these changes:

* Addition of “data management plan” and “conference paper” as examples to the description of resourceTypeGeneral :ref:`Text` (see :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>`).
* Addition of a usage note to the relationType pair :ref:`Compiles`/:ref:`IsCompiledBy` (see :doc:`Appendix 1: Controlled List Definitions - relatedIdentifierType </appendices/appendix_1/relatedIdentifierType>`).
* Addition of a reference to the DataCite Event Data service to the description of the :ref:`12` property.
* Addition of subproperty :ref:`12.f` to :ref:`12`.
* Notes on the coverage and scope of the metadata schema, and the preferred language in which the metadata should be provided.

Version 4.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.1 of the schema includes these changes:

* Allowing multiple polygons per :ref:`18`
* Addition of new optional subproperties for polygon

  * :ref:`18.4.2`
* Addition of new dateType “Other”
* Addition of new subproperty for :ref:`8`

  * :ref:`8.b`
* Addition of a new resourceType :ref:`DataPaper`
* Addition of three new relationType pairs:

  * :ref:`IsDescribedBy` and :ref:`Describes`
  * :ref:`HasVersion` and :ref:`IsVersionOf`
  * :ref:`IsRequiredBy` and :ref:`Requires`
* Addition of a new optional attribute for :ref:`2.1` and :ref:`7.1`:

  * nameType (:ref:`2.1.a <2.1.a>`, :ref:`7.1.a <7.1.a>`). Controlled list: personal, organizational
* Addition of a new optional attribute for :ref:`12`

  * :ref:`12.f`. Controlled list is identical to existing :ref:`10.a` attribute
* Addition of optional lang attribute to :ref:`16` property
* Change to the definition of :ref:`Collection` to encompass collections of one resourceType as well as those of mixed types.
* Inclusion of a reference to the Research Data Alliance (RDA)-recommended dynamic data citation approach in documentation in :doc:`section 2.2, Citation </guidance/dynamic_datasets>`.
* Change to the definition and examples of :ref:`13` property to include duration as well as extent.
* Correction of the hierarchy of elements for :ref:`2` and :ref:`7`.
* To enhance support for software citation, addition of 2 new appendices: one with a list of all the changes and explanatory notes (:doc:`/guidance/software_citation`); and one with Force11 mappings (:doc:`/mappings/force11_software_citation`)
* Changes and additions to these definitions, in support of software citation:

  * :ref:`1`
  * :ref:`3`
  * :ref:`4`
  * :ref:`7`
  * :ref:`5`
  * :ref:`10.a` (:ref:`Service`, :ref:`Software`)
  * relationType pairs (:ref:`IsPartOf`, :ref:`HasPart`, :ref:`IsDocumentedBy`, :ref:`Documents`, :ref:`IsVariantFormOf`, :ref:`IsOriginalFormOf`)
  * :ref:`15`
  * :ref:`16`
  * :ref:`17` (:ref:`TechnicalInfo`)

Version 4.0 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 4.0 of the schema includes these changes:

* Allowing more than one nameIdentifier (:ref:`2.4 <2.4>`, :ref:`7.4 <7.4>`) per :ref:`2` or :ref:`7`
* Addition of new optional subproperties for :ref:`2.1` and :ref:`7.1`:

  * givenName (:ref:`2.2 <2.2>`, :ref:`7.2 <7.2>`)
  * familyName (:ref:`2.3 <2.3>`, :ref:`7.3 <7.3>`)
* Addition of new :ref:`3.a` “Other”
* Addition of new subproperty for :ref:`6.a`:

  * :ref:`6.a`:

     * :ref:`6.c`
* Changing :ref:`10.a` from optional to mandatory
* Addition of a new relatedIdentifierType option :ref:`IGSN`
* Addition of a new descriptionType :ref:`TechnicalInfo`
* Addition of a new subproperty for :ref:`18`: :ref:`18.4`
* Changing the definition of the existing :ref:`18` sub properties (:ref:`18.1`, and :ref:`18.2`)
* Addition of a new property: :ref:`19`, with subproperties

  * :ref:`19.1`
  * :ref:`19.2`

     * :ref:`19.2.a`

  * :ref:`19.3`
  * :ref:`19.3.a`
  * :ref:`19.4`
* Deprecation of contributorType “funder” (as a result of adding the new property :ref:`19`)

Version 4.0 of the documentation includes these changes:

* Provision of a link to guidelines for how to write the ORCID ID (See properties 2.2.1 and 7.3.1 nameIdentifierScheme)
* Adjustment of the instructions for resourceTypeGeneral option :ref:`Collection` (See :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>`)

Note that, while the property :ref:`10` has been relocated in the documentation to the mandatory property section, it retains its original numbering (10).

Version 3.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 3.1 of the schema includes these changes:

* New affiliation attribute (:ref:`2.4 <2.4>`, :ref:`7.4 <7.4>`) for :ref:`2` and :ref:`7`
* New relationType pairs

  * :ref:`IsReviewedBy` and :ref:`Reviews`
  * :ref:`IsDerivedFrom` and :ref:`IsSourceOf`
* New contributorType: :ref:`DataCurator`
* New relatedIdentifierTypes:

  * :ref:`arXiv`
  * :ref:`bibcode`

Version 3.1 of the documentation includes these changes:

* Documentation for the new affiliation attributes (:ref:`2.4 <2.4>`, :ref:`7.4 <7.4>`) for :ref:`2` and :ref:`7`
* Special notes about support for long lists of names (:ref:`2` and :ref:`7`)
* Additional guidance for:

  * Recording :ref:`5`
  * Handling the digitised version of physical object
  * Handling missing mandatory property values, including standard values table (:doc:`/appendices/appendix_3`)
* Documentation for the new contributorType: :ref:`DataCurator`
* Documentation for the two new relatedIdentifierTypes:

  * :ref:`arXiv`
  * :ref:`bibcode`
* Documentation, including examples, for the new relationType pairs:

  * :ref:`IsReviewedBy` and :ref:`Reviews`
  * :ref:`IsDerivedFrom` and :ref:`IsSourceOf`
* Correction of link errors in 3.0 documentation

Version 3.0 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 3.0 of the DataCite Metadata Schema included these changes [#f1]_.

* Correction of a problem with our way of depicting dates by

  * implementing RKMS-ISO8601 [#f2]_ standard for depicting date ranges, so that a range is indicated as follows: 2004-03-02/2005-06-02
  * deleting ``startDate`` and ``endDate`` date types, and derogating these from earlier versions

* Addition of a new :ref:`18` property, with the sub-properties :ref:`18.1`, :ref:`18.2`, :ref:`18.3` supporting a simple depiction of geospatial information, as well as a free text description.
* Addition of new values to controlled lists:

  * :doc:`/appendices/appendix_1/contributorType`: :ref:`ResearchGroup` and :ref:`contributorType_Other`
  * :doc:`/appendices/appendix_1/dateType`: :ref:`Collected`
  * :doc:`/appendices/appendix_1/resourceTypeGeneral` : :ref:`Audiovisual`, :ref:`Workflow`, and :ref:`resourceTypeGeneral_Other` and derogation of Film
  * :doc:`/appendices/appendix_1/relatedIdentifierType`: :ref:`PMID`
  * :doc:`/appendices/appendix_1/relationType`: :ref:`IsIdenticalTo` (indicates that A is identical to B, for use when there is a need to register two separate instances of the same resource)
  * :doc:`/appendices/appendix_1/relationType`: :ref:`HasMetadata`, (indicates resource A has additional metadata B and indicates), :ref:`IsMetadataFor` (indicates additional metadata A for resource B)
  * :doc:`/appendices/appendix_1/descriptionType`: :ref:`Methods`
* Deletion of the derogated resourceType: film
* New sub-properties for :ref:`12.b`: :ref:`12.c`, :ref:`12.d` and :ref:`12.e`, to be used only for the new relationType pair of :ref:`HasMetadata`, :ref:`IsMetadataFor`
* Addition of schemeURI (:ref:`2.4.b <2.4.b>`, :ref:`7.4.b <7.4.b>`, :ref:`6.b <6.b>`) sub-property to the nameIdentifierScheme (:ref:`2.4.a <2.4.a>`, :ref:`7.4.a <7.4.a>`, :ref:`6.a <6.a>`) associated with :ref:`2.1`, :ref:`7.1` and :ref:`6`
* Addition of the :ref:`16.a` sub-property to :ref:`16`; :ref:`16` is now repeatable (within wrapper element ``rightsList``).
* Implementation of the xml:lang attribute [#f3]_ that can be used on the properties :ref:`3`, :ref:`6` and :ref:`17`.
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

* Addition of “URL” to list of allowed values for relatedIdentifierType
* Addition of the following values to list of allowed values for contributorType: :ref:`Producer`, :ref:`Distributor`, :ref:`RelatedPerson`, :ref:`Supervisor`, :ref:`Sponsor`, Funder, :ref:`RightsHolder`
* Addition of :ref:`SeriesInformation` to list of allowed values for descriptionType
* Addition of :ref:`Model` to list of allowed values for resourceTypeGeneral

Version 2.2 of the DataCite Metadata Schema documentation included these changes:

* Provision of more examples of xml for different types of resources
* Explanation of the :ref:`5` property in consideration of the requirements of citation. A change to the definition of the :ref:`4` property, which now reads, “The name of the entity that holds, archives, publishes, prints, distributes, releases, issues, or produces the resource. This property will be used to formulate the citation, so consider the prominence of the role.”

Version 2.1 Update
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Version 2.1 of the DataCite Metadata Schema introduced several changes, as noted below:

* Addition of a namespace (http://schema.datacite.org/namespace) to the schema in order to support OAI PMH compatibility
* Enforcement of content for mandatory properties
* New type for the :ref:`8` property to conform with the specification that it handles both YYYY and YYYY-MM-DD values

Version 2.1 of the DataCite Metadata Schema documentation included these changes:

* Addition of a column to the Mandatory and Optional Properties tables providing an indicator of whether the property being described is an attribute or a child of the corresponding property that has preceded it
* Revision of the allowed values description for the attribute 12.2 ``relationType``. These have been reviewed and rewritten for increased clarity. In several cases, corrections to the definitions occurred.


.. rubric:: Footnotes
.. [#f1] Two additional schema code level changes are the allowance of keeping optional wrapper elements empty and the allowance of arbitrary ordering of elements (by removal of <xs:sequence>).
.. [#f2] The standard is documented here: http://www.ukoln.ac.uk/metadata/dcmi/collection-RKMS-ISO8601/
.. [#f3] Allowed values IETF BCP 47, ISO 639-1 language codes, e.g. en, de, fr
