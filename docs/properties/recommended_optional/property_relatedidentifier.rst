.. _12:

12. RelatedIdentifier
=======================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** Identifiers of related resources. These must be globally unique identifiers.

**Allowed values, examples, other constraints:**

Free text.

Note: `DataCite Event Data <https://support.datacite.org/docs/eventdata-guide>`_ collects all references to related resources based on the relatedIdentifier property.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <relatedIdentifiers>
      <relatedIdentifier relatedIdentifierType="DOI" relationType="IsCitedBy" resourceTypeGeneral="JournalArticle">10.21384/bar</relatedIdentifier>
      <relatedIdentifier relatedIdentifierType="URL" relationType="HasMetadata" relatedMetadataScheme="DDI-L" schemeType="XSD" schemeURI="http://www.ddialliance.org/Specification/DDI-Lifecycle/3.1/XMLSchema/instance.xsd">https://example.com/</relatedIdentifier>
  </relatedIdentifiers>

.. _12.a:

12.a relatedIdentifierType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of the RelatedIdentifier.

**Allowed values, examples, other constraints:**

If relatedIdentifier is used, relatedIdentifierType is mandatory.

*Controlled List Values:*

* :ref:`ARK`
* :ref:`arXiv`
* :ref:`bibcode`
* :ref:`DOI`
* :ref:`EAN13`
* :ref:`EISSN`
* :ref:`Handle`
* :ref:`IGSN`
* :ref:`ISBN`
* :ref:`ISSN`
* :ref:`ISTC`
* :ref:`LISSN`
* :ref:`LSID`
* :ref:`PMID`
* :ref:`PURL`
* :ref:`UPC`
* :ref:`URL`
* :ref:`URN`
* :ref:`w3id`

See :doc:`Appendix 1: Controlled List Definitions - relatedIdentifierType </appendices/appendix_1/relatedIdentifierType>` for full names and examples.

.. _12.b:

12.b relationType
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Description of the relationship of the resource being registered (A) and the related resource (B).

**Allowed values, examples, other constraints:**

If RelatedIdentifier is used, relationType is mandatory.

*Controlled List Values:*

* :ref:`IsCitedBy`
* :ref:`Cites`
* :ref:`IsSupplementTo`
* :ref:`IsSupplementedBy`
* :ref:`IsContinuedBy`
* :ref:`Continues`
* :ref:`IsDescribedBy`
* :ref:`Describes`
* :ref:`HasMetadata`
* :ref:`IsMetadataFor`
* :ref:`HasVersion`
* :ref:`IsVersionOf`
* :ref:`IsNewVersionOf`
* :ref:`IsPreviousVersionOf`
* :ref:`IsPartOf`
* :ref:`HasPart`
* :ref:`IsPublishedIn`
* :ref:`IsReferencedBy`
* :ref:`References`
* :ref:`IsDocumentedBy`
* :ref:`Documents`
* :ref:`IsCompiledBy`
* :ref:`Compiles`
* :ref:`IsVariantFormOf`
* :ref:`IsOriginalFormOf`
* :ref:`IsIdenticalTo`
* :ref:`IsReviewedBy`
* :ref:`Reviews`
* :ref:`IsDerivedFrom`
* :ref:`IsSourceOf`
* :ref:`IsRequiredBy`
* :ref:`Requires`
* :ref:`IsObsoletedBy`
* :ref:`Obsoletes`
* :ref:`IsMeasuredBy`
* :ref:`Measures`

See :doc:`Appendix 1: Controlled List Definitions - relationType </appendices/appendix_1/relationType>` for definitions, examples and usage notes.

.. _12.c:

12.c relatedMetadataScheme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the scheme.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.

.. _12.d:

12.d schemeURI
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the relatedMetadataScheme.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.

.. _12.e:

12.e schemeType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The type of the relatedMetadataScheme, linked with the schemeURI.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

Examples: XSD, DDT, Turtle

.. _12.f:

12.f resourceTypeGeneral
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The general type of the related resource.

**Allowed values, examples, other constraints:**

Use the controlled list values as stated in :ref:`10.a`:

* :ref:`Audiovisual`
* :ref:`Book`
* :ref:`BookChapter`
* :ref:`Collection`
* :ref:`ComputationalNotebook`
* :ref:`ConferencePaper`
* :ref:`ConferenceProceeding`
* :ref:`DataPaper`
* :ref:`Dataset`
* :ref:`Dissertation`
* :ref:`Event`
* :ref:`Image`
* :ref:`InteractiveResource`
* :ref:`Instrument`
* :ref:`Journal`
* :ref:`JournalArticle`
* :ref:`Model`
* :ref:`OutputManagementPlan`
* :ref:`PeerReview`
* :ref:`PhysicalObject`
* :ref:`Preprint`
* :ref:`Report`
* :ref:`Service`
* :ref:`Software`
* :ref:`Sound`
* :ref:`Standard`
* :ref:`StudyRegistration`
* :ref:`Text`
* :ref:`Workflow`
* :ref:`resourceTypeGeneral_Other`

See :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>` for definitions, examples and usage notes.
