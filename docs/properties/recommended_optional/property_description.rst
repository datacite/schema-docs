.. _17:

17. Description
====================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** All additional information that does not fit in any of the other categories. May be used for technical information or detailed information associated with a scientific instrument.

**Allowed values, examples, other constraints:**

Free text.

It is a best practice to supply a description.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none
    
.. rubric:: Example XML

.. code:: xml

  <descriptions>
      <description xml:lang="en" descriptionType="Abstract">Example abstract</description>
  </descriptions>


.. _17.a:

17.a descriptionType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of the Description.

**Allowed values, examples, other constraints:**

If Description is used, descriptionType is mandatory.

*Controlled List Values:*


* :ref:`Abstract`
* :ref:`Methods`
* :ref:`SeriesInformation`
* :ref:`TableOfContents`
* :ref:`TechnicalInfo`
* :ref:`descriptionType_Other`

Note: :ref:`SeriesInformation` as a container for series title, volume, issue, page number, and related fields, is now superseded by the new :ref:`20` property with relationType "IsPublishedIn" selected.

See :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix_1/descriptionType>` for definitions.
