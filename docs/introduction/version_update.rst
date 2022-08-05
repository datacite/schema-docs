Version 4.5 Update
====================

.. note::

   To do: Summarize updates.

Major Documentation changes:

* Following community feedback and suggestions, this version includes changes and additions to clarify the :doc:`RelatedItem </properties/recommended_optional/property_relateditem>` property:

 * Changes and additions to subproperty definitions:

     * Addition of a note in :ref:`relatedItemIdentifier <20.1>` to strongly recommend the use of an identical :doc:`RelatedIdentifier </properties/recommended_optional/property_relatedidentifier>` for indexing.
     * Addition of a note in :ref:`volume <20.5>`, :ref:`issue <20.6>`, :ref:`number <20.7>`, :ref:`numberType <20.7.a>`, :ref:`firstPage <20.8>`, :ref:`lastPage <20.9>`, and :ref:`edition <20.11>` to indicate that these subproperties should only be used with the relationType “IsPublishedIn”.
     * Change to :ref:`firstPage <20.8>` and :ref:`lastPage <20.9>` to specify that the pages refer to the resource *within* the related item (for which the DOI is being registered), not the entire related item.
     * Minor changes to other RelatedItem subproperty definitions to improve consistency.
 * Updated definition of descriptionType :ref:`SeriesInformation` in :ref:`17.a descriptionType <17.a>` and :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix_1/descriptionType>` and  to clarify that it is superceded by RelatedItem *with the "relationType IsPublishedIn" selected*.

* Addition of a note to :ref:`3.a titleType <3.a>` (subproperty of :doc:`/properties/mandatory/property_title`) to match the corresponding note in :ref:`20.3.a titleType <20.3.a>` (subproperty of :ref:`20.3 Title <20.3>` in :doc:`/properties/recommended_optional/property_relateditem`).
