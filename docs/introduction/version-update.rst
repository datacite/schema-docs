Version 4.8 Update
====================

.. note::

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.8/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.8/epub/

These changes are in response to requests from DataCite community members—people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

If you have ideas for the DataCite Metadata Schema, we invite you to contribute on `DataCite Suggestions <https://github.com/datacite/datacite-suggestions/discussions/categories/metadata-schema-suggestions>`_

.. contents:: :local:
    :backlinks: none

Schema changes
-----------------------------
* Addition of a new :ref:`21` property, with sub-properties:

  * :ref:`21.1`
  * :ref:`21.1.a`
  * :ref:`21.1.b`
  * :ref:`21.1.c`
  * :ref:`21.1.d`
* Addition of a new :ref:`22` property, with sub-property:

  * :ref:`22.a`
* Addition of :ref:`BlogPost` to the :doc:`/appendices/appendix-1/resourceTypeGeneral` controlled list values.

  * This value may be used in :ref:`10.a` and other places where resourceTypeGeneral is used (:ref:`12.f`, :ref:`20.a`).
* Addition of :ref:`PatentNumber` to the :doc:`/appendices/appendix-1/relatedIdentifierType` controlled list values.

  * This value may be used in :ref:`12.a` and other places where relatedIdentifierType is used (:ref:`20.1.a`).
* Addition of new :doc:`/appendices/appendix-1/contributorType`: :ref:`Reviewer`

  * This value may be used in :ref:`7.a` and other places where contributorType is used (:ref:`20.12.a`).

Documentation changes
-----------------------------
* Addition of :doc:`Appendix 1: Controlled List Definitions - accessType </appendices/appendix-1/accessType>` to accompany :ref:`22.a` and :ref:`21.1.c`.