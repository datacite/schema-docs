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

* Addition of :ref:`Instrument <Instrument>` to the :doc:`resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>` controlled list values.

 * This value may used in :ref:`10.a resourceTypeGeneral <10.a>` and other places where resourceTypeGeneral is used (:ref:`12.f <12.f>`, :ref:`20.a <20.a>`).

* Addition of new relationType pair: :ref:`IsUsedBy <IsUsedBy>` and :ref:`Uses <Uses>`

Support for publisher identifiers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Addition of new subproperties for :doc:`Publisher </properties/mandatory/property_publisher>`:

   * :ref:`publisherIdentifier <4.a>`
   * :ref:`publisherIdentifierScheme <4.b>`
   * :ref:`schemeURI <4.c>`

Distribution property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 * Addition of a new :doc:`Distribution </properties/recommended_optional/property_distribution>` property. Subproperties:

   * :ref:`mediaType <21.1>`
   * :ref:`contentUrl <21.2>`
   * :ref:`lastUpdated <21.2.a>`
   * :ref:`byteSize <21.2.b>`
   * :ref:`checkSum <21.3>`
   * :ref:`algorithm <21.3.a>`
   * :ref:`accessRights <21.4>`
   * :ref:`accessRightsUri <21.4.a>`


Documentation changes
-----------------------------

Support for instruments
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Changes and additions to these definitions, in support of instruments:

 * :doc:`Title </properties/mandatory/property_title>`
 * :doc:`Creator </properties/mandatory/property_creator>`
 * :doc:`Contributor </properties/recommended_optional/property_contributor>`
 * :doc:`AlternateIdentifier </properties/recommended_optional/property_alternateidentifier>`
 * :doc:`Description </properties/recommended_optional/property_description>`
 * :ref:`descriptionType: TechnicalInfo <TechnicalInfo>`

* To enhance support for instruments, addition of new mapping: :doc:`/mappings/pidinst`

Distribution property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* To enhance support for the Distribution property, addition of a new guidance document: :doc:`/guidance/distribution`

Other changes and corrections
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Correction of the cardinality for ``affiliationIdentifier`` (properties :ref:`2.5.a <2.5.a>` and :ref:`7.5.a <7.5.a>`).
* Correction of the capitalization of ``schemeURI`` (properties :ref:`2.5.c <2.5.c>`, :ref:`7.5.c <7.5.c>`, and :ref:`19.2.b <19.2.b>`).
* Addition of a note to :ref:`funderIdentifierType <19.2.a>` to indicate when it is mandatory.
* Updated examples for ``nameIdentifier`` and its attributes (properties :ref:`2.4 <2.4>` and :ref:`7.4 <7.4>`).
* Updated examples for ``affiliationIdentifier`` and its attributes (properties :ref:`2.5 <2.5>` and :ref:`7.5 <7.5>`).
* Other minor corrections to definitions and examples.


New documentation structure
-----------------------------

We have relocated some content to two new sections:

- :doc:`Guidance </guidance/index>`
- :doc:`Mappings </mappings/index>`

These sections may be updated more frequently than the metadata schema itself.
