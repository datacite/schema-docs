Version 4.5 Update
====================

.. note::

   For the first time, the DataCite Metadata Working Group is releasing the DataCite Metadata Schema documentation as web documentation.

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/epub/

   To make the DataCite Metadata Schema more easily usable on the web, we have updated the documentation structure. As a result, numbering for footnotes, tables, and selected appendices has changed from Version 4.4.

These changes are in response to requests from DataCite community members, people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

.. contents:: :local:

Schema changes
-----------------------------

Support for instruments
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Addition of :ref:`Instrument` to the :doc:`/appendices/appendix_1/resourceTypeGeneral` controlled list values.

 * This value may used in :ref:`10.a` and other places where resourceTypeGeneral is used (:ref:`12.f`, :ref:`20.a`).

* Addition of new :doc:`/appendices/appendix_1/relationType` pair: :ref:`IsUsedBy` and :ref:`Uses`

Support for publisher identifiers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Addition of new sub-properties for :ref:`4`:

   * :ref:`4.a`
   * :ref:`4.b`
   * :ref:`4.c`

Distribution property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 * Addition of a new :ref:`21` property. Sub-properties:

   * :ref:`21.a`
   * :ref:`21.1`
   * :ref:`21.1.a`
   * :ref:`21.1.b`
   * :ref:`21.2`
   * :ref:`21.2.a`
   * :ref:`21.3`
   * :ref:`21.3.a`


Documentation changes
-----------------------------

Support for instruments
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Changes and additions to these definitions, in support of instruments:

 * :ref:`3`
 * :ref:`2`
 * :ref:`7`
 * :ref:`11`
 * :ref:`17`
 * :ref:`descriptionType: TechnicalInfo <TechnicalInfo>`

* To enhance support for instruments, addition of new mapping: :doc:`/mappings/pidinst`

Distribution property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* To enhance support for the :ref:`21` property, addition of a new guidance document: :doc:`/guidance/distribution`

RelatedItem property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Changes and additions to sub-property definitions:

 * Addition of a note in :ref:`20.1` to strongly recommend the use of an identical :ref:`12` for indexing.
 * Addition of a note in :ref:`20.5`, :ref:`20.6`, :ref:`20.7`, :ref:`20.7.a`, :ref:`20.8`, :ref:`20.9`, and :ref:`20.11` to indicate that these subproperties should only be used with the relationType :ref:`IsPublishedIn`.
 * Change to :ref:`20.8` and :ref:`20.9` to specify that the pages refer to the resource *within* the related item (for which the DOI is being registered), not the entire related item.
 * Minor changes to other RelatedItem sub-property definitions to improve consistency.

* Updated definition of descriptionType :ref:`SeriesInformation` in :ref:`17.a` and :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix_1/descriptionType>` and  to clarify that it is superseded by :ref:`20` with the relationType :ref:`IsPublishedIn` selected.
* To enhance support for the :ref:`20` property, addition of a new guidance document: :doc:`/guidance/related_item_guide`

Other changes and corrections
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Correction of the cardinality for properties :ref:`2.5.a` and :ref:`7.5.a`.
* Correction of the capitalization of properties :ref:`2.5.c`, :ref:`7.5.c`, and :ref:`19.2.b`.
* Correction of the cardinality of :ref:`19.2.a` and addition of a note indicate when it is mandatory.
* Addition of a note to :ref:`3.a` (sub-property of :ref:`3`) to match the corresponding note in :ref:`20.3.a` (subproperty of :ref:`20.3` in :ref:`20`).
* Updated examples for nameIdentifier (properties :ref:`2.4 <2.4>` and :ref:`7.4 <7.4>`) and its attributes.
* Updated examples for affiliationIdentifier (properties :ref:`2.5 <2.5>` and :ref:`7.5 <7.5>`) and its attributes.
* Other minor corrections to definitions and examples.


New documentation structure
-----------------------------

We have relocated some content to two new sections:

- :doc:`/guidance/index`
- :doc:`/mappings/index`

These sections may be updated more frequently than the metadata schema itself.
