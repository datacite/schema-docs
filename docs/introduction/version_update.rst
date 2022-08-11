Version 4.5 Update
====================

.. note::

   For the first time, the DataCite Metadata Working Group is releasing the DataCite Metadata Schema documentation as web documentation.

   To access the documentation in PDF or Epub format, access the menu in the bottom left corner or the links below:

   - PDF: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/pdf/
   - Epub: https://datacite-metadata-schema.readthedocs.io/_/downloads/en/4.5_draft/epub/

   To make the DataCite Metadata Schema more easily usable on the web, we have updated the documentation structure. As a result, numbering for footnotes, tables, and selected appendices has changed from Version 4.4.

.. note::

   *To do: Summarize updates.*

Schema changes
-----------------------------

This release of the Metadata Schema contains...

The remainder of the Version 4.5 changes are in response to requests from DataCite community members, people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.


Documentation changes
-----------------------------

* Following community feedback and suggestions, this version includes changes and additions to clarify the :doc:`RelatedItem </properties/recommended_optional/property_relateditem>` property:

 * Changes and additions to subproperty definitions:

     * Addition of a note in :ref:`relatedItemIdentifier <20.1>` to strongly recommend the use of an identical :doc:`RelatedIdentifier </properties/recommended_optional/property_relatedidentifier>` for indexing.
     * Addition of a note in :ref:`volume <20.5>`, :ref:`issue <20.6>`, :ref:`number <20.7>`, :ref:`numberType <20.7.a>`, :ref:`firstPage <20.8>`, :ref:`lastPage <20.9>`, and :ref:`edition <20.11>` to indicate that these subproperties should only be used with the relationType “IsPublishedIn”.
     * Change to :ref:`firstPage <20.8>` and :ref:`lastPage <20.9>` to specify that the pages refer to the resource *within* the related item (for which the DOI is being registered), not the entire related item.
     * Minor changes to other RelatedItem subproperty definitions to improve consistency.
 * Updated definition of descriptionType :ref:`SeriesInformation` in :ref:`17.a descriptionType <17.a>` and :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix_1/descriptionType>` and  to clarify that it is superceded by RelatedItem *with the "relationType IsPublishedIn" selected*.

* Addition of a note to :ref:`3.a titleType <3.a>` (subproperty of :doc:`/properties/mandatory/property_title`) to match the corresponding note in :ref:`20.3.a titleType <20.3.a>` (subproperty of :ref:`20.3 Title <20.3>` in :doc:`/properties/recommended_optional/property_relateditem`).

New documentation structure
-----------------------------

We have relocated some content to two new sections:

- :doc:`Guidance </guidance/index>`
- :doc:`Mappings </mappings/index>`

These sections may be updated more frequently than the metadata schema itself.
