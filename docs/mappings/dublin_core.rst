DataCite to Dublin Core Mapping 4.4
========================================

.. note::

   This mapping will be updated to version 4.5 with the official release.

Citation:
DataCite Metadata Working Group. (2021). DataCite to Dublin Core Mapping 4.4. DataCite e.V. https://doi.org/10.14454/qn00-qx85.

On the occasion of the release of `v4.4 of the DataCite Metadata Schema <https://schema.datacite.org/meta/kernel-4.4/doc/DataCite-MetadataKernel_v4.4.pdf>`_ the Metadata Working Group has updated the mapping to Dublin Core. This replaces the mapping in the Appendix of the `DataCite-MetadataKernel v2.1 <https://schema.datacite.org/archive/kernel-2.1/doc/DataCite-MetadataKernel_v2.1.pdf>`_.

The mapping can be used to convert records described following version 4.4 of the DataCite Metadata Schema into records that comply with the Dublin Core Metadata Initiative Schema.

.. _Table 4:

Table 4: DataCite to Dublin Core Mapping
------------------------------------------------------

.. list-table::
   :header-rows: 1
   :widths: auto
   :class: longtable
   :name: Table 4: DataCite to Dublin Core Mapping

   * - DataCite-Property
     - Dublin Core
   * - :ref:`1`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`1.a`
     - –
   * - :ref:`2`
     - `dcterms:creator <http://purl.org/dc/terms/creator>`_
   * - :ref:`2.1`
     - `dcterms:creator <http://purl.org/dc/terms/creator>`_
   * - :ref:`2.1.a`
     - –
   * - :ref:`2.2`
     - –
   * - :ref:`2.3`
     - –
   * - :ref:`2.4`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`2.4.a`
     - –
   * - :ref:`2.4.b`
     - –
   * - :ref:`2.5`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`2.5.a`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`2.5.b`
     - –
   * - :ref:`2.5.c`
     - –
   * - :ref:`3`
     - `dcterms:title <http://purl.org/dc/terms/title>`_
   * - :ref:`3.a`
     - `dcterms:alternative <http://purl.org/dc/terms/alternative>`_
   * - :ref:`4`
     - `dcterms:publisher <http://purl.org/dc/terms/publisher>`_
   * - :ref:`5`
     - `dcterms:issued <http://purl.org/dc/terms/issued>`_
   * - :ref:`6`
     - `dcterms:subject <http://purl.org/dc/terms/subject>`_
   * - :ref:`6.a`
     - –
   * - :ref:`6.b`
     - –
   * - :ref:`6.c`
     - `dcterms:subject <http://purl.org/dc/terms/subject>`_
   * - :ref:`6.d`
     - `dcterms:subject <http://purl.org/dc/terms/subject>`_
   * - :ref:`7`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`7.a`
     - –
   * - :ref:`7.1`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`7.1.a`
     - –
   * - :ref:`7.2`
     - –
   * - :ref:`7.3`
     - –
   * - :ref:`7.4`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`7.4.a`
     - –
   * - :ref:`7.4.b`
     - –
   * - :ref:`7.5`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`7.5.a`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`7.5.b`
     - –
   * - :ref:`7.5.c`
     - –
   * - :ref:`8`
     - `dcterms:date <http://purl.org/dc/terms/date>`_
   * - :ref:`8.a` [#f1]_
     - –
   * - - :ref:`Accepted`
     - `dcterms:dateAccepted <http://purl.org/dc/terms/dateAccepted>`_
   * - - :ref:`Available`
     - `dcterms:available <http://purl.org/dc/terms/available>`_
   * - - :ref:`Collected`
     - `dcterms:date <http://purl.org/dc/terms/date>`_
   * - - :ref:`Copyrighted`
     - `dcterms:dateCopyrighted <http://purl.org/dc/terms/dateCopyrighted>`_
   * - - :ref:`Created`
     - `dcterms:created <http://purl.org/dc/terms/created>`_
   * - - :ref:`Issued`
     - `dcterms:issued <http://purl.org/dc/terms/issued>`_
   * - - :ref:`Submitted`
     - `dcterms:dateSubmitted <http://purl.org/dc/terms/dateSubmitted>`_
   * - - :ref:`Updated`
     - `dcterms:modified <http://purl.org/dc/terms/modified>`_
   * - :ref:`8.a` (for StartDate/EndDate)
     - `dcterms:temporal <http://purl.org/dc/terms/temporal>`_
   * - :ref:`8.b`
     - –
   * - :ref:`9`
     - `dcterms:language <http://purl.org/dc/terms/language>`_
   * - :ref:`10`
     - `dcterms:type <http://purl.org/dc/terms/type>`_
   * - :ref:`10.a`
     - `dcterms:type <http://purl.org/dc/terms/type>`_
   * - :ref:`11`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`11.a`
     - –
   * - :ref:`12`
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`12.a`
     - –
   * - :ref:`12.b` [#f2]_
     -
   * - - :ref:`IsReferencedBy`
     - `dcterms:isReferencedBy <http://purl.org/dc/terms/isReferencedBy>`_
   * - - :ref:`references`
     - `dcterms:references <http://purl.org/dc/terms/references>`_
   * - - :ref:`IsVersionOf`
     - `dcterms:isVersionOf <http://purl.org/dc/terms/isVersionOf>`_
   * - - :ref:`HasVersion`
     - `dcterms:hasVersion <http://purl.org/dc/terms/hasVersion>`_
   * - - :ref:`IsVariantFormOf`
     - `dcterms:isFormatOf <http://purl.org/dc/terms/isFormatOf>`_
   * - - :ref:`IsPartOf`
     - `dcterms:isPartOf <http://purl.org/dc/terms/isPartOf>`_
   * - - :ref:`HasPart`
     - `dcterms:hasPart <http://purl.org/dc/terms/hasPart>`_
   * - - :ref:`IsObsoletedBy`
     - `dcterms:isReplacedBy <http://purl.org/dc/terms/isReplacedBy>`_
   * - - :ref:`Obsoletes`
     - `dcterms:replaces <http://purl.org/dc/terms/replaces>`_
   * - - :ref:`IsDerivedFrom`
     - `dcterms:source <http://purl.org/dc/terms/source>`_
   * - - *Other relation types*
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`12.c`
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`12.d`
     - –
   * - :ref:`12.e`
     - –
   * - :ref:`12.f`
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`13`
     - `dcterms:extent <http://purl.org/dc/terms/extent>`_
   * - :ref:`14`
     - `dcterms:format <http://purl.org/dc/terms/format>`_
   * - :ref:`15`
     - –
   * - :ref:`16`
     - `dcterms:rights <http://purl.org/dc/terms/rights>`_
   * - :ref:`16.a`
     - `dcterms:rights <http://purl.org/dc/terms/rights>`_
   * - :ref:`16.b`
     - `dcterms:rights <http://purl.org/dc/terms/rights>`_
   * - :ref:`16.c`
     - –
   * - :ref:`16.d`
     - –
   * - :ref:`17`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`17.a`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`Abstract`
     - `dcterms:abstract <http://purl.org/dc/terms/abstract>`_
   * - :ref:`Methods`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`TechnicalInfo`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`TableOfContents`
     - `dcterms:tableOfContents <http://purl.org/dc/terms/tableOfContents>`_
   * - :ref:`descriptionType_Other`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`18`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.1.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.1.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.2.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.2.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.2.3`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.2.4`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.3`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.1.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.1.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.2.1`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4.2.2`
     - `dcterms:spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`19`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`19.1`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`19.2`
     - `dcterms:contributor <http://purl.org/dc/terms/contributor>`_
   * - :ref:`19.2.a`
     - –
   * - :ref:`19.2.b`
     - –
   * - :ref:`19.3`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`19.3.a`
     - `dcterms:identifier <http://purl.org/dc/terms/identifier>`_
   * - :ref:`19.4`
     - `dcterms:description <http://purl.org/dc/terms/description>`_
   * - :ref:`20` [#f3]_
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`20.a`
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`20.b`
     -
   * - - :ref:`IsReferencedBy`
     - `dcterms:isReferencedBy <http://purl.org/dc/terms/isReferencedBy>`_
   * - - :ref:`References`
     - `dcterms:references <http://purl.org/dc/terms/references>`_
   * - - :ref:`IsVersionOf`
     - `dcterms:isVersionOf <http://purl.org/dc/terms/isVersionOf>`_
   * - - :ref:`HasVersion`
     - `dcterms:hasVersion <http://purl.org/dc/terms/hasVersion>`_
   * - - :ref:`IsVariantFormOf`
     - `dcterms:isFormatOf <http://purl.org/dc/terms/isFormatOf>`_
   * - - :ref:`IsPartOf`
     - `dcterms:isPartOf <http://purl.org/dc/terms/isPartOf>`_
   * - - :ref:`HasPart`
     - `dcterms:hasPart <http://purl.org/dc/terms/hasPart>`_
   * - - :ref:`IsObsoletedBy`
     - `dcterms:isReplacedBy <http://purl.org/dc/terms/isReplacedBy>`_
   * - - :ref:`Obsoletes`
     - `dcterms:replaces <http://purl.org/dc/terms/replaces>`_
   * - - :ref:`IsDerivedFrom`
     - `dcterms:source <http://purl.org/dc/terms/source>`_
   * - - *Other relation types*
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`20.1`
     - `dcterms:relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`20.1.a`
     - –
   * - :ref:`20.2`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.2.1`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.3`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.3.a`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.4`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.5`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.6`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.7`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.7.a`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.8`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.9`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.10`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.11`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.12`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.12.a`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_
   * - :ref:`20.12.1`
     - `dcterms:bibliographicCitation <http://purl.org/dc/terms/bibliographicCitation>`_

Future developments
------------------------

The Metadata Working Group are in discussion with ongoing developments by a team at the National Library of Finland who have proposed a draft DC application profile called SRAP (Scholarly Resources Application Profile) “for expressing metadata about scholarly works such as dissertations and academic articles. Describing these documents using current DC Terms is not ideal because many relevant elements are missing”. This is an interesting development because they hope that a future version may focus on research datasets. Examples of proposed SRAP elements which are of value to DataCite include dcterms:affiliation; dcterms:grantNumber and using an id= or pid= for identifier or value URIs for elements such as dcterms:creator or dcterms:contributor.


.. rubric:: Footnotes

.. [#f1] :ref:`8.a` is mandatory in DataCite if :ref:`8` is used. For controlled list values, see: :doc:`Appendix 1: Controlled List Definitions - dateType </appendices/appendix_1/dateType>`.

.. [#f2] :ref:`12.b` is mandatory in DataCite if :ref:`12` is used. For controlled list values, see: :doc:`Appendix 1: Controlled List Definitions - relationType </appendices/appendix_1/relationType>`.

.. [#f3] For the details of the related item i.e. title etc., use dcterms:bibliographicCitation. Concatenate the content according to any preferred Citation format.
