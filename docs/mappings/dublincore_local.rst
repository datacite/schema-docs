DataCite - Dublin Core local extension
=================================================================

An example local extension to Dublin Core for DataCite metadata properties.

.. _Table 5:

Table 5: DataCite - Dublin Core local extension
------------------------------------------------------

.. list-table::
   :header-rows: 1
   :widths: auto
   :class: longtable
   :name: DataCite - Dublin Core local extension

   * - DataCite-Property
     - DataCite - Dublin Core local extension
   * - :ref:`1`
     - `dc.identifier <http://purl.org/dc/terms/identifier>`_.doi
   * - :ref:`1.a`
     - –
   * - :ref:`2`
     - `dc.creator <http://purl.org/dc/terms/creator>`_
   * - :ref:`2.1`
     - `dc.creator <http://purl.org/dc/terms/creator>`_
   * - :ref:`2.1.a`
     - –
   * - :ref:`2.2`
     - –
   * - :ref:`2.3`
     - –
   * - :ref:`2.4`
     - `dc.creator <http://purl.org/dc/terms/creator>`_.pid
   * - :ref:`2.4.a`
     - –
   * - :ref:`2.4.b`
     - –
   * - :ref:`2.5`
     - `dc.creator <http://purl.org/dc/terms/creator>`_.affiliation
   * - :ref:`2.5.a`
     - `dc.creator <http://purl.org/dc/terms/creator>`_.affiliation.pid
   * - :ref:`2.5.b`
     - –
   * - :ref:`2.5.c`
     - –
   * - | :ref:`3`
       | Mapped by :ref:`3.a`:
     - `dc.title <http://purl.org/dc/terms/title>`_
   * - - AlternativeTitle
     - `dc.title.alternative <http://purl.org/dc/terms/alternative>`_
   * - - Subtitle
     - `dc.title <http://purl.org/dc/terms/title>`_.subtitle
   * - - TranslatedTitle
     - `dc.title <http://purl.org/dc/terms/title>`_.translatedTitle
   * - - Other
     - `dc.title <http://purl.org/dc/terms/title>`_.other
   * - :ref:`3.a`
     - –
   * - :ref:`4`
     - `dc.publisher <http://purl.org/dc/terms/publisher>`_
   * - :ref:`4.a`
     - `dc.publisher <http://purl.org/dc/terms/publisher>`_.pid
   * - :ref:`4.b`
     - –
   * - :ref:`4.c`
     - –
   * - :ref:`5`
     - `dc.date.issued <http://purl.org/dc/terms/issued>`_
   * - :ref:`6`
     - `dc.subject <http://purl.org/dc/terms/subject>`_
   * - :ref:`6.a`
     - –
   * - :ref:`6.b`
     - –
   * - :ref:`6.c`
     - `dc.subject <http://purl.org/dc/terms/subject>`_.pid
   * - :ref:`6.d`
     - `dc.subject <http://purl.org/dc/terms/subject>`_.classification
   * - :ref:`7`
     - `dc.contributor <http://purl.org/dc/terms/contributor>`_.{contributorType}
   * - :ref:`7.a`
     - –
   * - :ref:`7.1`
     - `dc.contributor <http://purl.org/dc/terms/contributor>`_.{contributorType}
   * - :ref:`7.1.a`
     - –
   * - :ref:`7.2`
     - –
   * - :ref:`7.3`
     - –
   * - :ref:`7.4`
     - `dc.contributor <http://purl.org/dc/terms/contributor>`_.{contributorType}.pid
   * - :ref:`7.4.a`
     - –
   * - :ref:`7.4.b`
     - –
   * - :ref:`7.5`
     - `dc.contributor <http://purl.org/dc/terms/contributor>`_.{contributorType}.affiliation
   * - :ref:`7.5.a`
     - `dc.contributor <http://purl.org/dc/terms/contributor>`_.{contributorType}.affiliation.pid
   * - :ref:`7.5.b`
     - –
   * - :ref:`7.5.c`
     - –
   * - | :ref:`8`
       | Mapped by :ref:`8.a`:
     - `dc.date <http://purl.org/dc/terms/date>`_
   * - - :ref:`Accepted`
     - `dc.date.accepted <http://purl.org/dc/terms/dateAccepted>`_
   * - - :ref:`Available`
     - `dc.date.available <http://purl.org/dc/terms/available>`_
   * - - :ref:`Copyrighted`
     - `dc.date.copyrighted <http://purl.org/dc/terms/dateCopyrighted>`_
   * - - :ref:`Collected`
     - `dc.date <http://purl.org/dc/terms/date>`_.collected
   * - - :ref:`Created`
     - `dc.date.created <http://purl.org/dc/terms/created>`_
   * - - :ref:`Issued`
     - `dc.date.issued <http://purl.org/dc/terms/issued>`_
   * - - :ref:`Submitted`
     - `dc.date.submitted <http://purl.org/dc/terms/dateSubmitted>`_
   * - - :ref:`Updated`
     - `dc.date.modified <http://purl.org/dc/terms/modified>`_
   * - - :ref:`Valid`
     - `dc.date.valid <http://purl.org/dc/terms/valid>`_
   * - - :ref:`Withdrawn`
     - `dc.date <http://purl.org/dc/terms/date>`_.withdrawn
   * - - :ref:`dateType_Other`
     - `dc.date <http://purl.org/dc/terms/date>`_.other
   * - :ref:`8.a`
     - –
   * - :ref:`8.b`
     - `dc.description <http://purl.org/dc/terms/description>`_
   * - :ref:`9`
     - `dc.language <http://purl.org/dc/terms/language>`_
   * - :ref:`10`
     - `dc.type <http://purl.org/dc/terms/type>`_
   * - :ref:`10.a`
     - `dc.type <http://purl.org/dc/terms/type>`_
   * - :ref:`11`
     - `dc.identifier <http://purl.org/dc/terms/identifier>`_.{alternateIdentifierType}
   * - :ref:`11.a`
     - –
   * - | :ref:`12`
       | Mapped by :ref:`12.b`:
     - `dc.relation <http://purl.org/dc/terms/relation>`_
   * - - :ref:`IsReferencedBy`
     - `dc.relation.isReferencedBy <http://purl.org/dc/terms/isReferencedBy>`_
   * - - :ref:`references`
     - `dc.relation.references <http://purl.org/dc/terms/references>`_
   * - - :ref:`IsVersionOf`
     - `dc.relation.isVersionOf <http://purl.org/dc/terms/isVersionOf>`_
   * - - :ref:`HasVersion`
     - `dc.relation.hasVersion <http://purl.org/dc/terms/hasVersion>`_
   * - - :ref:`IsVariantFormOf`
     - `dc.relation.isFormatOf <http://purl.org/dc/terms/isFormatOf>`_
   * - - :ref:`IsPartOf`
     - `dc.relation.isPartOf <http://purl.org/dc/terms/isPartOf>`_
   * - - :ref:`HasPart`
     - `dc.relation.hasPart <http://purl.org/dc/terms/hasPart>`_
   * - - :ref:`IsObsoletedBy`
     - `dc.relation.isReplacedBy <http://purl.org/dc/terms/isReplacedBy>`_
   * - - :ref:`Obsoletes`
     - `dc.relation.replaces <http://purl.org/dc/terms/replaces>`_
   * - - :ref:`IsDerivedFrom`
     - `dc.source <http://purl.org/dc/terms/source>`_ or `dc.relation.source <http://purl.org/dc/terms/source>`_
   * - - *Other relationTypes*
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}
   * - :ref:`12.a`
     - –
   * - :ref:`12.b` 
     - –
   * - :ref:`12.c`
     - –
   * - :ref:`12.d`
     - –
   * - :ref:`12.e`
     - –
   * - :ref:`12.f`
     - –
   * - :ref:`13`
     - `dc.format.extent <http://purl.org/dc/terms/extent>`_
   * - :ref:`14`
     - `dc.format <http://purl.org/dc/terms/format>`_
   * - :ref:`15` 
     - `dc.description <http://purl.org/dc/terms/description>`_.version
   * - :ref:`16`
     - `dc.rights <http://purl.org/dc/terms/rights>`_
   * - :ref:`16.a`
     - `dc.rights.license <http://purl.org/dc/terms/license>`_
   * - :ref:`16.b`
     - `dc.rights <http://purl.org/dc/terms/rights>`_
   * - :ref:`16.c`
     - –
   * - :ref:`16.d`
     - –
   * - | :ref:`17`
       | Mapped by :ref:`17.a`:
     - `dc.description <http://purl.org/dc/terms/description>`_
   * - - :ref:`Abstract`
     - `dc.description.abstract <http://purl.org/dc/terms/abstract>`_
   * - - :ref:`Methods`
     - `dc.description <http://purl.org/dc/terms/description>`_.methods
   * - - :ref:`SeriesInformation`
     - `dc.description <http://purl.org/dc/terms/description>`_.seriesInformation
   * - - :ref:`TechnicalInfo`
     - `dc.description <http://purl.org/dc/terms/description>`_.technicalINfo
   * - - :ref:`TableOfContents`
     - `dc.description.tableOfContents <http://purl.org/dc/terms/tableOfContents>`_
   * - - :ref:`descriptionType_Other`
     - `dc.description <http://purl.org/dc/terms/description>`_.other
   * - :ref:`17.a`
     - –
   * - :ref:`18`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.point
   * - :ref:`18.1.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.point.longitude
   * - :ref:`18.1.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.point.latitude
   * - :ref:`18.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.box
   * - :ref:`18.2.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.box.west
   * - :ref:`18.2.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.box.east
   * - :ref:`18.2.3`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.box.south
   * - :ref:`18.2.4`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.box.north
   * - :ref:`18.3`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_
   * - :ref:`18.4`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon
   * - :ref:`18.4.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.polygonPoint
   * - :ref:`18.4.1.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.polygonPoint.longitude
   * - :ref:`18.4.1.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.polygonPoint.latitude
   * - :ref:`18.4.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.inPolygonPoint
   * - :ref:`18.4.2.1`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.inPolygonPoint.longitude
   * - :ref:`18.4.2.2`
     - `dc.coverage.spatial <http://purl.org/dc/terms/spatial>`_.polygon.inPolygonPoint.latitude
   * - :ref:`19`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.fundingReference
   * - :ref:`19.1`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.fundingReference.funderName
   * - :ref:`19.2`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.fundingReference.pid
   * - :ref:`19.2.a`
     - –
   * - :ref:`19.2.b`
     - –
   * - :ref:`19.3`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.fundingReference.awardNumber
   * - :ref:`19.3.a`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.awardNumber.pid
   * - :ref:`19.4`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.awardTitle
   * - | :ref:`20` 
       | Mapped by :ref:`20.b` as above for :ref:`12`.
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}
   * - :ref:`20.a`
     - –
   * - :ref:`20.b`
     - –
   * - :ref:`20.1`
     - `dc.relation <http://purl.org/dc/terms/relation>`_
   * - :ref:`20.1.a`
     - –
   * - :ref:`20.2`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.creator
   * - :ref:`20.2.1`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.creator
   * - :ref:`20.3`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.title
   * - :ref:`20.3.a`
     - –
   * - :ref:`20.4`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.publicationYear
   * - :ref:`20.5`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.volume
   * - :ref:`20.6`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.issue
   * - :ref:`20.7`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.number
   * - :ref:`20.7.a`
     - –
   * - :ref:`20.8`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.firstPage
   * - :ref:`20.9`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.lastPage
   * - :ref:`20.10`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.publisher
   * - :ref:`20.11`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.edition
   * - :ref:`20.12`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.contributor.{contributorType}
   * - :ref:`20.12.a`
     - –
   * - :ref:`20.12.1`
     - `dc.relation <http://purl.org/dc/terms/relation>`_.{relationType}.contributor.{contributorType}