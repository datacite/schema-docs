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
    
.. rubric:: Example

.. tabs::

   .. code-tab:: xml

      <descriptions>
          <description xml:lang="en" descriptionType="Abstract">Example abstract</description>
      </descriptions>
   
   .. code-tab:: json

      "descriptions": [
        {
          "lang": "en",
          "description": "Example abstract",
          "descriptionType": "Abstract"
        }
      ]

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

See :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix-1/descriptionType>` for definitions.


.. _17.lang:

17.lang xml:lang
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The language of the description.

**Allowed values, examples, other constraints:**

`xml:lang` values must follow the pattern defined by the `XML schema language type <https://www.w3.org/TR/xmlschema-2/#language>`_, e.g.: fr, cmn, nys, swh.  See the W3C’s `Choosing a Language Tag <https://www.w3.org/International/questions/qa-choosing-language-tags>`_ for guidance on recommended values.