12. RelatedIdentifier
=======================

.. note::
   References to 10.1 should reference 10.a.

**Occurrences:** 0-n

**Definition:** Identifiers of related resources. These must be globally unique identifiers.

**Allowed values, examples, other constraints:**

Free text

Note: DataCite Event Data [24]_ collects all references to related resources based on the relatedIdentifier property.

*Sub-properties:*

.. contents:: :local:

.. _12.a:

12.a relatedIdentifierType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of the RelatedIdentifier

**Allowed values, examples, other constraints:**

If relatedIdentifier is used, relatedIdentifierType is mandatory.

*Controlled List Values:*

* ARK
* arXiv
* bibcode
* DOI
* EAN13
* EISSN
* Handle
* IGSN
* ISBN
* ISSN
* ISTC
* LISSN
* LSID
* PMID
* PURL
* UPC
* URL
* URN
* w3id

See :doc:`Appendix 1: Controlled List Definitions - relatedIdentifierType </appendices/appendix_1/relatedIdentifierType>` for full names and examples.

.. _12.b:

12.b relationType
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Description of the relationship of the resource being registered (A) and the related resource (B)

**Allowed values, examples, other constraints:**

If RelatedIdentifier is used, relationType is mandatory.

*Controlled List Values:*

* IsCitedBy
* Cites
* IsSupplementTo
* IsSupplementedBy
* IsContinuedBy
* Continues
* IsDescribedBy
* Describes
* HasMetadata
* IsMetadataFor
* HasVersion
* IsVersionOf
* IsNewVersionOf
* IsPreviousVersionOf
* IsPartOf
* HasPart
* IsPublishedIn
* IsReferencedBy
* References
* IsDocumentedBy
* Documents
* IsCompiledBy
* Compiles
* IsVariantFormOf
* IsOriginalFormOf
* IsIdenticalTo
* IsReviewedBy
* Reviews
* IsDerivedFrom
* IsSourceOf
* IsRequiredBy
* Requires
* IsObsoletedBy
* Obsoletes

See :doc:`Appendix 1: Controlled List Definitions - relationType </appendices/appendix_1/relationType>` for definitions, examples and usage notes.


12.c relatedMetadataScheme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the scheme

**Allowed values, examples, other constraints:**

Use only with this relation pair:
(HasMetadata/ IsMetadataFor)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.

12.d schemeURI
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the relatedMetadataScheme

**Allowed values, examples, other constraints:**

Use only with this relation pair:
(HasMetadata/ IsMetadataFor)

See :ref:`Appendix 1: Controlled List Definitions - relationType  - HasMetadata <HasMetadata>` for example.

12.e schemeType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The type of the relatedMetadataScheme, linked with the schemeURI

**Allowed values, examples, other constraints:**

Use only with this relation pair:
(HasMetadata/ IsMetadataFor)

Examples: XSD, DDT, Turtle

12.f resourceTypeGeneral
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The general type of the related resource

**Allowed values, examples, other constraints:**

Use the controlled list values as stated in :ref:`10.1 <10.a>`.

See Appendix for definitions, examples and usage notes.

.. rubric:: Footnotes
.. [24] https://support.datacite.org/docs/eventdata-guide
