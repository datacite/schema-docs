Overview
===========

The properties of the DataCite Metadata Schema are presented in this section.

.. contents:: :local:
    :backlinks: none


Conventions
-------------------

Levels of obligation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are three different levels of obligation for the metadata properties:

* **Mandatory (M)** properties *must* be provided;
* **Recommended (R)** properties are optional, but strongly recommended for interoperability; and
* **Optional (O)** (but not specifically recommended) properties provide richer description.

Repositories who wish to enhance the prospects that their metadata will be found, cited, and linked
to original research are strongly encouraged to submit both the Recommended and Mandatory sets of
properties. Together, the Mandatory and Recommended sets of properties and their sub-properties are
especially valuable to information seekers and added-service providers, such as indexers. The Metadata
Working Group members strongly urge the inclusion of metadata identified as Recommended for the
purpose of achieving greater exposure for the resource’s metadata record and, therefore, the underlying
research itself.

The prospect that a resource's metadata will be found, cited, and linked is enhanced by using the
combined Mandatory and Recommended "super set" of properties and sub-properties. These are bolded in :ref:`Table 1 <Table_1>` (Mandatory Properties) and :ref:`Table 2 <Table_2>` (Recommended and Optional Properties).


Naming and numbering
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Properties and sub-properties have naming and numbering conventions as follows:

- properties begin with a capital letter (e.g., ``Creator``)
- sub-properties begin with a lower case letter, with subsequent words using capital letters (e.g., ``creatorName``, ``nameType``) [#f1]_

Each property is numbered. The major properties are numbered 1-22.

Occurrences
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

“Occurrences" indicates cardinality/quantity constraints for the properties as follows:

* 0-n = optional and repeatable
* 0-1 = optional, but not repeatable
* 1-n = required and repeatable
* 1 = required, but not repeatable


XML schema
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the XML schema:

- Properties are always represented as *elements*.
- Sub-properties can be either *sub-elements* or *attributes*.

The numbering convention distinguishes *elements* and *sub-elements* from *attributes*:

- *Elements* and *sub-elements* are numbered (e.g., 2. Creator, 2.1 creatorName).
- *Attributes* are represented with letters (e.g., 2.1.a nameType)

Because XML attributes are not repeatable, sub-properties represented as attributes will always have an occurrence of either 0-1 (optional) or 1 (required).

.. list-table::
   :header-rows: 1
   :widths: auto

   * - XML representation
     - Property or sub-property
     - Example
   * - Element
     - Property
     - :ref:`2`
   * - Sub-element
     - Sub-property
     - :ref:`2.1`
   * - Attribute
     - Sub-property
     - :ref:`2.1.a`


.. _xmllang:

xml:lang
^^^^^^^^^^^^

XML provides an `xml:lang` attribute [#f2]_ that can be used on the following properties and sub-properties:

* :ref:`2.1`
* :ref:`3`
* :ref:`4`
* :ref:`6`
* :ref:`7.1`
* :ref:`16`
* :ref:`17`
* :ref:`20.2.1`
* :ref:`20.3`
* :ref:`20.12.1` 

This provides a way to describe the language used for the *content of the specified properties*. [#f3]_


The schema provides the :ref:`9` property to be used to describe the language of the resource.



Mandatory Properties
-------------------------------------------------

The mandatory properties must be supplied with any initial metadata submission to DataCite, together with their relevant sub-properties. If one of the required
properties is unavailable, please use one of the standard (machine-recognizable) codes listed in
:doc:`/appendices/appendix-3`.

.. _Table_1:

Table 1: DataCite Mandatory Properties
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 1  | :ref:`Identifier <1>`                                                                   | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 2  | :ref:`Creator <2>`                                                                      | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 3  | :ref:`Title <3>`                                                                        | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 4  | :ref:`Publisher <4>`                                                                    | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 5  | :ref:`PublicationYear <5>`                                                              | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 10 | :ref:`ResourceType <10>`                                                                | M          |
+----+-----------------------------------------------------------------------------------------+------------+

.. _Guidance_missing_values: 

Guidance for handling missing mandatory property values
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If providing values for any of the mandatory properties presents a difficulty, use of standard machine-recognizable codes is strongly advised. A set of the codes is provided in :doc:`/appendices/appendix-3`. However, we recommend that you consider the resulting effect on the citation created from the metadata provided. [#f4]_

Recommended and Optional Properties
-------------------------------------------------

Of the Recommended set of properties, the most important to use is the ``Description`` property, together with the Recommended sub-property ``descriptionType="Abstract"`` (see :ref:`17`). :doc:`Appendix 1 </appendices/appendix-1/index>` includes detailed descriptions of controlled list values, using bold text to indicate those values that are especially important for information seekers and added service providers. It cannot be emphasized enough how valuable an Abstract is to other scholars in finding the resource and then determining whether or not the resource, once found, is worth investigating further, re-using, or validating.

.. _Table_2:

Table 2: DataCite Recommended and Optional Properties
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 6  | :ref:`Subject <6>`                                                                      | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 7  | :ref:`Contributor <7>`                                                                  | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 8  | :ref:`Date <8>`                                                                         | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 9  | :ref:`Language <9>`                                                                     | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 11 | :ref:`AlternateIdentifier <11>`                                                         | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 12 | :ref:`RelatedIdentifier <12>`                                                           | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 13 | :ref:`Size <13>`                                                                        | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 14 | :ref:`Format <14>`                                                                      | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 15 | :ref:`Version <15>`                                                                     | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 16 | :ref:`Rights <16>`                                                                      | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 17 | :ref:`Description <17>`                                                                 | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 18 | :ref:`GeoLocation <18>`                                                                 | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 19 | :ref:`FundingReference <19>`                                                            | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 20 | :ref:`RelatedItem <20>`                                                                 | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 21 | :ref:`Distribution <21>`                                                                | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 22 | :ref:`Access <22>`                                                                      | O          |
+----+-----------------------------------------------------------------------------------------+------------+


.. rubric:: Footnotes
.. [#f1] This convention is known as “camelCase.” https://en.wikipedia.org/wiki/CamelCase
.. [#f2] `xml:lang` values must follow the pattern defined by the `XML schema language type <https://www.w3.org/TR/xmlschema-2/#language>`_, e.g.: fr, cmn, nys, swh.  See the W3C’s `Choosing a Language Tag <https://www.w3.org/International/questions/qa-choosing-language-tags>`_ for guidance on recommended values.
.. [#f3] For creator and contributor names, `xml:lang` is recommended only when nameType is "Organizational".
.. [#f4] The standard values will be represented as provided in the citation string. For example, here is an example of a citation that uses machine-readable substitutions for all but one of the required metadata properties. The less metadata that is supplied, the less information is conveyed: ``:unkn (2020). :none. :null. https://doi.org/10.5072/FK2JW8C992``