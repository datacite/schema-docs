Version 4.6 Update
====================

.. note::

   For the first time, the DataCite Metadata Working Group is releasing the DataCite Metadata Schema documentation as web documentation.

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5/epub/

   To make the DataCite Metadata Schema more easily usable on the web, we have updated the documentation structure. As a result, numbering for footnotes, tables, and selected appendices has changed from Version 4.4.

These changes are in response to requests from DataCite community members, people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

.. contents:: :local:
    :backlinks: none

Schema changes
-----------------------------

* Addition of :ref:`Award` and :ref:`Project` to the :doc:`/appendices/appendix-1/resourceTypeGeneral` controlled list values.

 * These values may be used in :ref:`10.a` and other places where resourceTypeGeneral is used (:ref:`12.f`, :ref:`20.a`).

* Addition of :ref:`CSTR` and :ref:`RRID` to the :doc:`/appendices/appendix-1/relatedIdentifierType` controlled list values.

 * These values may be used in :ref:`12.a` and other places where relatedIdentifierType is used (:ref:`20.1.a`).

* Addition of new :doc:`/appendices/appendix-1/contributorType`: :ref:`Translator`

 * This value may be used in :ref:`7.a` and other places where contributorType is used (:ref:`20.12.a`).

* Addition of new :doc:`/appendices/appendix-1/relationType` pair: :ref:`HasTranslation` and :ref:`IsTranslationOf`

* Addition of new :doc:`/appendices/appendix-1/dateType`: :ref:`Coverage`

Documentation changes
-----------------------------

* Clarification of the allowed values for :ref:`9`.

Other changes and corrections
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* FIXME