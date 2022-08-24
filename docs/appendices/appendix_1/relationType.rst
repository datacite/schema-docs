relationType
=====================================

Description of the relationship of the resource being registered (A) and the related resource (B).

*Used by:*

* :ref:`12.b`
* :ref:`20.b`

*Options:*

.. contents:: :local:


IsCitedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that B includes A in a citation

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI"relationType="IsCited By">10.4232/10.ASEAS-5.2-1</relatedIdentifier>


Cites
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that A includes B in a citation

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISBN" relationType="Cites">0761964312</relatedIdentifier>


IsSupplementTo
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that A is a supplement to B

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="IsSupplementTo">urn:nbn:de:0168-ssoar-13172</relatedIdentifier>


IsSupplementedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that B is a supplement to A

**Example and Usage Notes:**

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="PMID" relationType="IsSupplementedBy">16911322/</relatedIdentifier>


IsContinuedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is continued by the work B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="IsContinuedBy">urn:nbn:de:bsz:21-opus-4967</relatedIdentifier>

Continues
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a continuation of the work B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="Continues">urn:nbn:de:bsz:21-opus-4966</relatedIdentifier>


Describes
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A describes B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Describes">10.6084/m9.figshare.c.3288407</relatedIdentifier>

IsDescribedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is described by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsDescribedBy">10.1038/sdata.2016.123</relatedIdentifier>


.. _HasMetadata:

HasMetadata
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates resource A has additional metadata B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasMetadata" relatedMetadataScheme="DDI-L" schemeURI="http://www.ddialliance.org/Specification/DDI-Lifecycle/3.1/XMLSchema/instance.xsd">10.1234/567890</relatedIdentifier>


IsMetadataFor
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates additional metadata A for a resource B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsMetadataFor" relatedMetadataScheme="DDI-L" schemeURI="http://www.ddialliance.org/Specification/DDI-Lifecycle/3.1/XMLSchema/instance.xsd">10.1234/567891</relatedIdentifier>


HasVersion
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A has a version (B)

**Example and Usage Notes:**

The registered resource such as a software package or code repository has a versioned instance (indicates A has the instance B). It may be used, e.g., to relate an un-versioned code repository to one of its specific software versions.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="HasVersion">10.5281/ZENODO.832053</relatedIdentifier>


IsVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a version of B

**Example and Usage Notes:**

The registered resource is an instance of a target resource (indicates that A is an instance of B). It may be used, e.g., to relate a specific version of a software package to its software code repository.

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsVersionOf">10.5281/ZENODO.832054</relatedIdentifier>


IsNewVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a new edition of B, where the new edition has been modified or updated

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsNewVersionOf">10.5438/0005</relatedIdentifier>


IsPreviousVersionOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a previous edition of B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsPreviousVersionOf">10.5438/0007</relatedIdentifier>


IsPartOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a portion of B; may be used for elements of a series

**Example and Usage Notes:**

*Recommended for discovery.*

Primarily this relation is applied to container-contained type relationships.

May be used for individual software modules; note that code repository-to-version relationships should be modeled using IsVersionOf and HasVersion

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsPartOf">10.5281/zenodo.754312</relatedIdentifier>


HasPart
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A includes the part B

**Example and Usage Notes:**

*Recommended for discovery.*

Primarily this relation is applied to container-contained type relationships.

May be used for individual software modules; note that code repository-to-version relationships should be modeled using IsVersionOf and HasVersion

*Recommended for discovery.*

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="HasPart">https://zenodo.org/record/16564/files/dune-stuff-LSSC_15.zip</relatedIdentifier>


IsPublishedIn
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is published inside B, but is independent of other things published inside of B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISSN" relationType="IsPublishedIn">2213-1337</relatedIdentifier>


IsReferencedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is used as a source of information by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsReferencedBy">http://www.testpubl.de</relatedIdentifier>


References
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates B is used as a source of information for A

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="References">urn:nbn:de:bsz:21-opus-963</relatedIdentifier>


IsDocumentedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates B is documentation about/explaining A

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsDocumentedBy">http://tobias-lib.uni-tuebingen.de/volltexte/2000/96/</relatedIdentifier>

May be used for software documentation.

Documents
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is documentation about/explaining B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Documents">10.1234/7836</relatedIdentifier>

May be used for software documentation.

IsCompiledBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates B is used to compile or create A

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="isCompiledBy">http://d-nb.info/gnd/4513749-3</relatedIdentifier>

May be used to indicate either a traditional text compilation, or the compiler program used to generate executable software.


Compiles
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates B is the result of a compile or creation event using A

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="Compiles">urn:nbn:de:bsz:21-opus-963</relatedIdentifier>

May be used for software and text, as a compiler can be a computer program or a person.


IsVariantFormOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a variant or different form of B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsVariantFormOf">10.1234/8675</relatedIdentifier>

Use for a different form of one thing.

May be used for different software operating systems or compiler formats, for example.


IsOriginalFormOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is the original form of B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsOriginalFormOf">10.1234/9035</relatedIdentifier>

May be used for different software operating systems or compiler formats, for example.


IsIdenticalTo
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that A is identical to B, for use when there is a need to register two separate instances of the same resource

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsIdenticalTo">http://oac.cdlib.org/findaid/ark:/13030/c8r78fzq</relatedIdentifier>

IsIdenticalTo should be used for a resource that is the same as the registered resource but is saved on another location, maybe another institution.


IsReviewedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that A is reviewed by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsReviewedBy">10.5256/F1000RESEARCH.4288.R4745</relatedIdentifier>


Reviews
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates that A is a review of B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Reviews">10.12688/f1000research.4001.1</relatedIdentifier>


IsDerivedFrom
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates B is a source upon which A is based

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsDerivedFrom">10.6078/M7DZ067C</relatedIdentifier>

IsDerivedFrom should be used for a resource that is a derivative of an original resource.

In this example, the dataset is derived from a larger dataset and data values have been manipulated from their original state.


IsSourceOf
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** indicates A is a source upon which B is based

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsSourceOf"> http://opencontext.org/projects/81204AF8-127C-4686-E9B0-1202C3A47959</relatedIdentifier>

IsSourceOf is the original resource from which a derivative resource was created.

In this example, this is the original dataset without value manipulation.


IsRequiredBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is required by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsRequiredBy">10.1234/8675</relatedIdentifier>

May be used to indicate software dependencies.


Requires
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A requires B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Requires">10.1234/867</relatedIdentifier>

May be used to indicate software dependencies.


Obsoletes
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A replaces B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="Obsoletes">10.5438/0007</relatedIdentifier>


IsObsoletedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is replaced by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsObsoletedBy">10.5438/0005</relatedIdentifier>

.. _IsUsedBy:

IsUsedBy
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A is used by B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsUsedBy">10.5072/dataset</relatedIdentifier>

May be used to indicate the relationship between an instrument and where it has been used (as in, instrument A is IsUsedBy research output B).

.. _Uses:

Uses
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Indicates A uses B

**Example and Usage Notes:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI"relationType="Uses">10.5072/instrument</relatedIdentifier>

May be used to indicate the relationship between an instrument and where it has been used (as in, research output A uses instrument B).
