17. Description
====================

**Occurrences:** 0-n

**Definition:** All additional information that does not fit in any of the other categories. May be used for technical information.

**Allowed values, examples, other constraints:**

Free text

It is a best practice to supply a description.

*Sub-properties:*

.. contents:: :local:


17.a descriptionType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of the Description

**Allowed values, examples, other constraints:**

If Description is used, descriptionType is mandatory.

*Controlled List Values:*


* Abstract
* Methods
* SeriesInformation
* TableOfContents
* TechnicalInfo
* Other

Note: SeriesInformation as a container for series title, volume, issue, page number, and related fields, is now superseded by the new :doc:`RelatedItem </properties/recommended_optional/property_relateditem>` property.

See :doc:`Appendix 1: Controlled List Definitions - descriptionType </appendices/appendix_1/descriptionType>` for definitions.
