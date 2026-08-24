relationType
=====================================

Description of the relationship of the resource being registered (A) and the related resource (B).

*Used by:*

* :ref:`12.b`
* :ref:`20.b`

Note: Some relationTypes are processed as citations and references. Read more about `Contributing Citations and References <https://support.datacite.org/docs/contributing-citations-and-references>`_ on the DataCite support site.

*Options:*

.. contents:: :local:
    :backlinks: none


.. _IsCitedBy:

IsCitedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that B includes A in a citation

**Inverse relationType:** :ref:`Cites`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI"relationType="IsCited By">10.4232/10.ASEAS-5.2-1</relatedIdentifier>


.. _Cites:

Cites
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A includes B in a citation

**Inverse relationType:** :ref:`IsCitedBy`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISBN" relationType="Cites">0761964312</relatedIdentifier>


.. _IsSupplementTo:

IsSupplementTo
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A is a supplement to B

**Inverse relationType:** :ref:`IsSupplementedBy`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="IsSupplementTo">urn:nbn:de:0168-ssoar-13172</relatedIdentifier>


.. _IsSupplementedBy:

IsSupplementedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that B is a supplement to A

**Inverse relationType:** :ref:`IsSupplementTo`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="PMID" relationType="IsSupplementedBy">16911322</relatedIdentifier>


.. _IsContinuedBy:

IsContinuedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is continued by the work B

**Inverse relationType:** :ref:`Continues`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="IsContinuedBy">urn:nbn:de:bsz:21-opus-4967</relatedIdentifier>


.. _Continues:

Continues
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a continuation of the work B

**Inverse relationType:** :ref:`IsContinuedBy`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="Continues">urn:nbn:de:bsz:21-opus-4966</relatedIdentifier>


.. _Describes:

Describes
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A describes B

**Inverse relationType:** :ref:`IsDescribedBy`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Describes">10.6084/m9.figshare.c.3288407</relatedIdentifier>


.. _IsDescribedBy:

IsDescribedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is described by B

**Inverse relationType:** :ref:`Describes`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsDescribedBy">10.1038/sdata.2016.123</relatedIdentifier>


.. _HasMetadata:

HasMetadata
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates resource A has additional metadata B

**Inverse relationType:** :ref:`IsMetadataFor`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasMetadata" relatedMetadataScheme="DDI-L" schemeURI="http://www.ddialliance.org/Specification/DDI-Lifecycle/3.1/XMLSchema/instance.xsd">10.1234/567890</relatedIdentifier>


.. _IsMetadataFor:

IsMetadataFor
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates additional metadata A for a resource B

**Inverse relationType:** :ref:`HasMetadata`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsMetadataFor" relatedMetadataScheme="DDI-L" schemeURI="http://www.ddialliance.org/Specification/DDI-Lifecycle/3.1/XMLSchema/instance.xsd">10.1234/567891</relatedIdentifier>


.. _HasVersion:

HasVersion
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A has a version B

**Inverse relationType:** :ref:`IsVersionOf`

**Example and Usage Notes:**

The registered resource such as a software package or code repository has a versioned instance (indicates A has the instance B). It may be used, e.g., to relate an un-versioned code repository to one of its specific software versions.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasVersion">10.5281/ZENODO.832053</relatedIdentifier>


.. _IsVersionOf:

IsVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a version of B

**Inverse relationType:** :ref:`HasVersion`

**Example and Usage Notes:**

The registered resource is an instance of a target resource (indicates that A is an instance of B). It may be used, e.g., to relate a specific version of a software package to its software code repository.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsVersionOf">10.5281/ZENODO.832054</relatedIdentifier>


.. _IsNewVersionOf:

IsNewVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a new edition of B, where the new edition has been modified or updated

**Inverse relationType:** :ref:`IsPreviousVersionOf`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsNewVersionOf">10.5438/0005</relatedIdentifier>


.. _IsPreviousVersionOf:

IsPreviousVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a previous edition of B

**Inverse relationType:** :ref:`IsNewVersionOf`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsPreviousVersionOf">10.5438/0007</relatedIdentifier>


.. _IsPartOf:

IsPartOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a portion of B; may be used for elements of a series

**Inverse relationType:** :ref:`HasPart`

**Example and Usage Notes:**

*Recommended for discovery.*

Primarily this relation is applied to container-contained type relationships.

May be used for individual software modules; note that code repository-to-version relationships should be modeled using IsVersionOf and HasVersion

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsPartOf">10.5281/zenodo.754312</relatedIdentifier>


.. _HasPart:

HasPart
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A includes the part B

**Inverse relationType:** :ref:`IsPartOf`

**Example and Usage Notes:**

*Recommended for discovery.*

Primarily this relation is applied to container-contained type relationships.

May be used for individual software modules; note that code repository-to-version relationships should be modeled using IsVersionOf and HasVersion

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="HasPart">https://zenodo.org/record/16564/files/dune-stuff-LSSC_15.zip</relatedIdentifier>


.. _IsPublishedIn:

IsPublishedIn
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is published inside B, but is independent of other things published inside of B

**Inverse relationType:** N/A

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISSN" relationType="IsPublishedIn">2213-1337</relatedIdentifier>


.. _IsReferencedBy:

IsReferencedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is used as a source of information by B

**Inverse relationType:** :ref:`References`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsReferencedBy">http://www.testpubl.de</relatedIdentifier>


.. _References:

References
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates B is used as a source of information for A

**Inverse relationType:** :ref:`IsReferencedBy`

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="References">urn:nbn:de:bsz:21-opus-963</relatedIdentifier>


.. _IsDocumentedBy:

IsDocumentedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates B is documentation about/explaining A

**Inverse relationType:** :ref:`Documents`

**Example and Usage Notes:**

May be used for software documentation.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsDocumentedBy">http://tobias-lib.uni-tuebingen.de/volltexte/2000/96/</relatedIdentifier>


.. _Documents:

Documents
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is documentation about/explaining B

**Inverse relationType:** :ref:`IsDocumentedBy`

**Example and Usage Notes:**

May be used for software documentation.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Documents">10.1234/7836</relatedIdentifier>


.. _IsCompiledBy:

IsCompiledBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates B is used to compile or create A

**Inverse relationType:** :ref:`Compiles`

**Example and Usage Notes:**

May be used to indicate either a traditional text compilation, or the compiler program used to generate executable software.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsCompiledBy">http://d-nb.info/gnd/4513749-3</relatedIdentifier>


.. _Compiles:

Compiles
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates B is the result of a compile or creation event using A

**Inverse relationType:** :ref:`IsCompiledBy`

**Example and Usage Notes:**

May be used for software and text, as a compiler can be a computer program or a person.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="Compiles">urn:nbn:de:bsz:21-opus-963</relatedIdentifier>


.. _IsVariantFormOf:

IsVariantFormOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a variant or different form of B

**Inverse relationType:** :ref:`IsOriginalFormOf`

**Example and Usage Notes:**

Use for a different form of one thing.

May be used for different software operating systems or compiler formats, for example.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsVariantFormOf">10.1234/8675</relatedIdentifier>


.. _IsOriginalFormOf:

IsOriginalFormOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is the original form of B

**Inverse relationType:** :ref:`IsVariantFormOf`

**Example and Usage Notes:**

May be used for different software operating systems or compiler formats, for example.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsOriginalFormOf">10.1234/9035</relatedIdentifier>


.. _IsIdenticalTo:

IsIdenticalTo
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A is identical to B, for use when there is a need to register two separate instances of the same resource

**Inverse relationType:** N/A

**Example and Usage Notes:**

IsIdenticalTo should be used for a resource that is the same as the registered resource but is saved on another location, maybe another institution.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsIdenticalTo">http://oac.cdlib.org/findaid/ark:/13030/c8r78fzq</relatedIdentifier>


.. _IsReviewedBy:

IsReviewedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A is reviewed by B

**Inverse relationType:** :ref:`Reviews`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsReviewedBy">10.5256/F1000RESEARCH.4288.R4745</relatedIdentifier>


.. _Reviews:

Reviews
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A is a review of B

**Inverse relationType:** :ref:`IsReviewedBy`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Reviews">10.12688/f1000research.4001.1</relatedIdentifier>


.. _IsDerivedFrom:

IsDerivedFrom
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates B is a source upon which A is based

**Inverse relationType:** :ref:`IsSourceOf`

**Example and Usage Notes:**

IsDerivedFrom should be used for a resource that is a derivative of an original resource.

In this example, the dataset is derived from a larger dataset and data values have been manipulated from their original state.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsDerivedFrom">10.6078/M7DZ067C</relatedIdentifier>


.. _IsSourceOf:

IsSourceOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a source upon which B is based

**Inverse relationType:** :ref:`IsDerivedFrom`

**Example and Usage Notes:**

IsSourceOf is the original resource from which a derivative resource was created.

In this example, this is the original dataset without value manipulation.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsSourceOf">http://opencontext.org/projects/81204AF8-127C-4686-E9B0-1202C3A47959</relatedIdentifier>


.. _IsRequiredBy:

IsRequiredBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is required by B

**Inverse relationType:** :ref:`Requires`

**Example and Usage Notes:**

May be used to indicate software dependencies.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsRequiredBy">10.1234/8675</relatedIdentifier>


.. _Requires:

Requires
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A requires B

**Inverse relationType:** :ref:`IsRequiredBy`

**Example and Usage Notes:**

May be used to indicate software dependencies.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Requires">10.1234/867</relatedIdentifier>


.. _Obsoletes:

Obsoletes
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A replaces B

**Inverse relationType:** :ref:`IsObsoletedBy`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Obsoletes">10.5438/0007</relatedIdentifier>


.. _IsObsoletedBy:

IsObsoletedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is replaced by B

**Inverse relationType:** :ref:`Obsoletes`

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsObsoletedBy">10.5438/0005</relatedIdentifier>


.. _IsCollectedBy:

IsCollectedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is collected by B

**Inverse relationType:** :ref:`Collects`

**Example and Usage Notes:**

May be used to indicate the relationship between a dataset and an instrument that is used to collect, measure, obtain, or observe data (as in, dataset A is IsCollectedBy instrument B).

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsCollectedBy">10.5072/instrument</relatedIdentifier>


.. _Collects:

Collects
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A collects B

**Inverse relationType:** :ref:`IsCollectedBy`

**Example and Usage Notes:**

May be used to indicate the relationship between an instrument and where it has been used to collect, measure, obtain, or observe data (as in, instrument A collects dataset B).

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI"relationType="Collects">10.5072/data</relatedIdentifier>


.. _IsTranslationOf:

IsTranslationOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is a translation of B

**Inverse relationType:** :ref:`HasTranslation`

**Example and Usage Notes:**

When a resource is shared in one language, then later translated to another, use "IsTranslationOf" to link the translation to the original.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsTranslationOf">10.21384/828a-cm38</relatedIdentifier>


.. _HasTranslation:

HasTranslation
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A has a translation B

**Inverse relationType:** :ref:`IsTranslationOf`

**Example and Usage Notes:**

When a resource is shared in one language, then later translated to another, use "HasTranslation" to link the original resource to its translation.

When a resource is released at the same time in multiple languages, use "HasTranslation" to connect the works to each other in both directions.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasTranslation">10.21384/g01j-jm06</relatedIdentifier>


.. _IsOutputOf:

IsOutputOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is an output of B

**Inverse relationType:** :ref:`HasOutput`

**Example and Usage Notes:** May be used to connect the outputs of awards, projects, software, etc. to their sources.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsOutputOf" resourceTypeGeneral="Project">10.21384/g01j-jm06</relatedIdentifier>


.. _HasOutput:

HasOutput
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A has an output B

**Inverse relationType:** :ref:`IsOutputOf`

**Example and Usage Notes:** May be used to connect awards, projects, software, etc. to their associated outputs.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasOutput" resourceTypeGeneral="Dataset">10.21384/828a-cm38</relatedIdentifier>


.. _relationType_Other:

Other
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates that A is related to B and the relationship does not fit into an existing category.

**Inverse relationType:** N/A

**Example and Usage Notes:**

If selected, supply a value for :ref:`12.g` (or :ref:`20.c` for RelatedItem).

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Other" relationTypeInformation="is output of" resourceTypeGeneral="Project">10.21384/p27z-6n52</relatedIdentifier>