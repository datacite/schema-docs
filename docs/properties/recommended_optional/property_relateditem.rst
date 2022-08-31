.. _20:

20. RelatedItem
====================

**Occurrences:** 0-n

**Definition:** Information about a resource related to the one being registered.

**Allowed values, examples, other constraints:**

Can be used to provide series information or a text citation where the related resource does not have an identifier. However, it is also optional to provide an identifier here.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. note::

   See :doc:`/guidance/related_item_guide` for guidance.

.. _20.a:

20.a relatedItemType
~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The general type of the related item.

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
* :ref:`Text`
* :ref:`Workflow`
* :ref:`resourceTypeGeneral_Other`

See :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>` for definitions, examples, and usage notes.

.. _20.b:

20.b relationType
~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Description of the relationship of the resource being registered (A) and the related item (B).

**Allowed values, examples, other constraints:**

Use the controlled list values as stated in :ref:`12.b`:

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
* :ref:`IsUsedBy`
* :ref:`Uses`

relationType :ref:`IsPublishedIn` can be used to include series information, like title, volume, issue, page, etc.

See :doc:`Appendix 1: Controlled List Definitions - relationType </appendices/appendix_1/relationType>` for definitions, examples, and usage notes.

.. _20.1:

20.1 relatedItemIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The identifier for the related item.

**Allowed values, examples, other constraints:**

Example: 10.1021/jacs.9b01862

If relatedItemIdentifier is provided, an identical :ref:`12` is strongly recommended for indexing.

.. _20.1.a:

20.1.a relatedItemIdentifierType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of the Identifier for the related item.

**Allowed values, examples, other constraints:**

Use the controlled list values as stated in :ref:`12.a`:

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

See :doc:`Appendix 1: Controlled List Definitions - relatedIdentifierType </appendices/appendix_1/relatedIdentifierType>` for definitions, examples, and usage notes.


20.1.b relatedMetadataScheme
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The name of the scheme.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.


20.1.c schemeURI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the relatedMetadataScheme.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.


20.1.d schemeType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of the relatedMetadataScheme, linked with the schemeURI.

**Allowed values, examples, other constraints:**

Use only with this relation pair: (:ref:`HasMetadata`/ :ref:`IsMetadataFor`)

Examples: XSD, DDT, Turtle

.. _20.2:

20.2 Creator
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** The institution or person responsible for creating the related resource.

To supply multiple creators, repeat this property.


.. _20.2.1:

20.2.1 creatorName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The full name of the related item creator.

**Allowed values, examples, other constraints:**

Examples: Charpy, Antoine; Jemison, Mae; Foo Data Center

Note: The personal name, format should be: family, given. Non-roman names may be transliterated according to the `ALA-LC tables <https://www.loc.gov/catdir/cpso/roman.html>`_.


20.2.1.a nameType
###################

**Occurrences:** 0-1

**Definition:** The type of name.

**Allowed values, examples, other constraints:**

*Controlled List Values:*

 * Organizational
 * Personal (default)


20.2.2 givenName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The personal or first name of the creator.

**Allowed values, examples, other constraints:**

Examples based on the `20.2.1`_ names: Antoine; Mae


20.2.3 familyName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The surname or last name of the creator.

**Allowed values, examples, other constraints:**

Examples based on the `20.2.1`_ names: Charpy; Jemison

.. _20.3:

20.3 Title
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1-n

**Definition:** Title of the related item.

**Allowed values, examples, other constraints:**

Example: Journal of the American Chemical Society

.. _20.3.a:

20.3.a titleType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Type of the related item title. Use this sub-property to add a subtitle, translation, or alternate title to the main title. The primary title of the related item should not have a titleType sub-property.

**Allowed values, examples, other constraints:**

The titleType sub-property is used when more than a single title is provided. Unless otherwise indicated by titleType, a title is considered to be the main title.

.. _20.4:

20.4 PublicationYear
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The year when the item was or will be made publicly available.

**Allowed values, examples, other constraints:**

YYYY

.. _20.5:

20.5 volume
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Volume of the related item.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.6:

20.6 issue
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Issue number or name of the related item.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.7:

20.7 number
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Number of the related item, e.g., report number of article number.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.7.a:

20.7.a numberType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Type of the related item’s number, e.g., report number or article number.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

*Controlled List Values:*

* Article
* Chapter
* Report
* Other

.. _20.8:

20.8 firstPage
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** First page of the resource within the related item, e.g., of the chapter, article, or conference paper in proceedings.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.9:

20.9 lastPage
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Last page of the resource within the related item, e.g., of the chapter, article, or conference paper in proceedings.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.10:

20.10 Publisher
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the entity that holds, archives, publishes prints, distributes, releases, issues, or produces the resource.

**Allowed values, examples, other constraints:**

Examples: World Data Center for Climate (WDCC); GeoForschungsZentrum Potsdam (GFZ); Geological Institute, University of Tokyo, GitHub

.. _20.11:

20.11 edition
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Edition or version of the related item.

**Allowed values, examples, other constraints:**

Use only with relationType :ref:`IsPublishedIn`.

Free text.

.. _20.12:

20.12 Contributor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** An institution or person identified as contributing to the development of the resource. If multiple contributors are identified, this sub-property may be repeated for each contributor.

**Allowed values, examples, other constraints:**

Examples: Charpy, Antoine; Foo Data Center

.. _20.12.a:

20.12.a contributorType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The type of contributor of the resource.

**Allowed values, examples, other constraints:**

Use the controlled list values as stated in :ref:`7.a`.

See :doc:`Appendix 1: Controlled List Definitions - contributorType </appendices/appendix_1/contributorType>` for definitions, examples and usage notes.

.. _20.12.1:

20.12.1 contributorName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The full name of the related item contributor.

**Allowed values, examples, other constraints:**

If Contributor is used, then contributorName is mandatory.

Examples: Charpy, Antoine; Jemison, Mae; Foo Data Center

Note: The personal name, format should be: family, given. Non-roman names may be transliterated according to the `ALA-LC tables <https://www.loc.gov/catdir/cpso/roman.html>`_.

20.12.1.a nameType
###################

**Occurrences:** 0-1

**Definition:** The type of name.

**Allowed values, examples, other constraints:**

*Controlled List Values:*

 * Organizational
 * Personal (default)


20.12.2 givenName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The personal or first name of the contributor.

**Allowed values, examples, other constraints:**

Examples based on the `20.12.1`_ names: Antoine; Mae


20.12.3 familyName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The surname or last name of the contributor.

**Allowed values, examples, other constraints:**

Examples based on the `20.12.1`_ names: Charpy; Jemison
