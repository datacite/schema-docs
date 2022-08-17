Overview
===========

The properties of the DataCite Metadata Schema are presented in this section.

.. contents:: :local:

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
combined Mandatory and Recommended "super set" of properties and sub-properties. These are bolded in Tables 1 and 2.


Mandatory Properties
-------------------------------------------------

:doc:`mandatory/index` provides a detailed description of the mandatory properties, which must be supplied with any
initial metadata submission to DataCite, together with their sub-properties. **If one of the required
properties is unavailable**, please use one of the standard (machine-recognizable) codes listed in
:doc:`/appendices/appendix_3`.

.. _Table 1:

Table 1: DataCite Mandatory Properties
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 1  | **Identifier**                                                                          | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 2  | **Creator**                                                                             | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 3  | **Title**                                                                               | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 4  | **Publisher**                                                                           | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 5  | **PublicationYear**                                                                     | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 10 | **ResourceType**                                                                        | M          |
+----+-----------------------------------------------------------------------------------------+------------+


Recommended and Optional Properties
-------------------------------------------------

In :doc:`recommended_optional/index`, the Recommended and Optional properties are described in detail. For
an example of how to make a submission in XML format, please see the `XML Examples <https://schema.datacite.org/meta/kernel-4.0/>`_ provided on the
`DataCite Metadata Schema website <https://schema.datacite.org/>`_.


Of the Recommended set of properties, the most important to use is the ``Description`` property,
together with the Recommended attribute ``descriptionType="Abstract"`` (see :doc:`17. Description </properties/recommended_optional/property_description>`). :doc:`Appendix 1 </appendices/appendix_1/index>` includes detailed descriptions of controlled list values, using bold text to indicate those values that are especially important for information seekers and added service providers. It cannot be emphasized enough how valuable an Abstract is to other scholars in
finding the resource and then determining whether or not the resource, once found, is worth
investigating further, re-using, or validating.

.. _Table 2:

Table 2: DataCite Recommended and Optional Properties
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 6  | **Subject**                                                                             | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 7  | **Contributor**                                                                         | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 8  | **Date**                                                                                | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 9  | Language                                                                                | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 11 | AlternateIdentifier                                                                     | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 12 | **RelatedIdentifier**                                                                   | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 13 | Size                                                                                    | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 14 | Format                                                                                  | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 15 | Version                                                                                 | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 16 | Rights                                                                                  | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 17 | **Description**                                                                         | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 18 | **GeoLocation**                                                                         | R          |
+----+-----------------------------------------------------------------------------------------+------------+
| 19 | FundingReference                                                                        | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 20 | RelatedItem                                                                             | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 21 | Distribution                                                                            | O          |
+----+-----------------------------------------------------------------------------------------+------------+


Conventions
-------------------

Throughout this document, a naming convention has been used for all properties and sub-properties as
follows:

- properties begin with a capital letter (e.g., ``Creator``)
- sub-properties begin with a lower case letter (e.g., ``creatorName``)
- attributes begin with a lower case letter (e.g., ``nameType``)

If the name is a compound of more than one word, subsequent words begin with capital letters (e.g., ``creatorName``, ``nameType``). [#f1]_

Each property is numbered. The major properties are numbered 1-21.

In the XML schema, properties are represented as elements and can have sub-properties (sub-elements). Both properties and sub-properties can have attributes. Elements, sub-elements, and attributes are indicated using numbers and letters:

* numbers indicate *elements* and *sub-elements* (e.g., 2. Creator, 2.1 creatorName)
* letters indicate *attributes* (e.g., 2.1.a nameType)

“Occurrences" indicates cardinality/quantity constraints for the properties as follows:

* 0-n = optional and repeatable
* 0-1 = optional, but not repeatable
* 1-n = required and repeatable
* 1 = required, but not repeatable

XML provides an xml:lang attribute [#f2]_ that can be used on the properties ``Title``, ``Subject``, ``Rights``,
``Description``, and ``RelatedItem Title``, as well as on the properties ``Creator``,
``Contributor`` and ``Publisher`` for organizational names. This provides a way to describe the
language used for the content of the specified properties. The schema provides a ``Language`` property
to be used to describe the language of the resource.

.. rubric:: Footnotes
.. [#f1] This convention is known as “camelCase.” https://en.wikipedia.org/wiki/CamelCase
.. [#f2] Allowed values IETF BCP 47, ISO 639-1 language codes, e.g. en, de, fr
