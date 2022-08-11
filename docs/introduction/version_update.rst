Version 4.5 Update
====================

.. note::

   For the first time, the DataCite Metadata Working Group is releasing the DataCite Metadata Schema documentation as web documentation.

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/epub/

   To make the DataCite Metadata Schema more easily usable on the web, we have updated the documentation structure. As a result, numbering for footnotes, tables, and selected appendices has changed from Version 4.4.

These changes are in response to requests from DataCite community members, people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

Schema changes
-----------------------------

* Addition of new values to the :ref:`resourceTypeGeneral <10.a>` property:

 * :ref:`Instrument <Instrument>`

* Addition of new relationType pair: :ref:`IsUsedBy <IsUsedBy>` and :ref:`Uses <Uses>`

Documentation changes
-----------------------------

* Changes and additions to these definitions, in support of instruments:

 * :doc:`Title </properties/mandatory/property_title>`
 * :doc:`Creator </properties/mandatory/property_creator>`
 * :doc:`Contributor </properties/recommended_optional/property_contributor>`
 * :doc:`AlternateIdentifier </properties/recommended_optional/property_alternateidentifier>`
 * :doc:`Description </properties/recommended_optional/property_description>`
 * :ref:`Description (TechnicalInfo) <TechnicalInfo>`

* To enhance support for instruments, addition of new mapping: :doc:`/mappings/pidinst`

New documentation structure
-----------------------------

We have relocated some content to two new sections:

- :doc:`Guidance </guidance/index>`
- :doc:`Mappings </mappings/index>`

These sections may be updated more frequently than the metadata schema itself.
