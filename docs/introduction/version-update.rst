Version 4.7 Update
====================

.. note::

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.7/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.7/epub/

These changes are in response to requests from DataCite community members—people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

.. contents:: :local:
    :backlinks: none

Schema changes
-----------------------------

* Addition of :ref:`Poster` and :ref:`Presentation` to the :doc:`/appendices/appendix-1/resourceTypeGeneral` controlled list values.

  * These values may be used in :ref:`10.a` and other places where resourceTypeGeneral is used (:ref:`12.f`, :ref:`20.a`).
* Addition of :ref:`RAiD` and :ref:`SWHID` to the :doc:`/appendices/appendix-1/relatedIdentifierType` controlled list values.

  * These values may be used in :ref:`12.a` and other places where relatedIdentifierType is used (:ref:`20.1.a`).
* Addition of new :doc:`/appendices/appendix-1/relationType`: :ref:`relationType_Other`
* Addition of new sub-properties:

  * :ref:`12.g` for :ref:`12`
  * :ref:`20.c` for :ref:`20`

Documentation changes
-----------------------------

* Documentation of existing `xml:lang` sub-properties on their property pages:

  * :ref:`2.1.lang` for :ref:`2.1`
  * :ref:`3.lang` for :ref:`3`
  * :ref:`4.lang` for :ref:`4`
  * :ref:`6.lang` for :ref:`6`
  * :ref:`7.1.lang` for :ref:`7.1`
  * :ref:`16.lang` for :ref:`16`
  * :ref:`17.lang` for :ref:`17`
  * :ref:`20.2.1.lang` for :ref:`20.2.1`
  * :ref:`20.3.lang` for :ref:`20.3`
  * :ref:`20.12.1.lang` for :ref:`20.12.1`

* Updated examples in :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix-1/resourceTypeGeneral>`.
* Updated the :ref:`Guidance_missing_values`.
