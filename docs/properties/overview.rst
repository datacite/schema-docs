Overview
===========

The properties of the DataCite Metadata Schema are presented in this section. More detailed
descriptions of the properties, and their related sub-properties, are provided in the :doc:`datacite_properties` section.

There are three different levels of obligation for the metadata properties:

* **Mandatory (M)** properties *must* be provided;
* **Recommended (R)** properties are optional, but strongly recommended for interoperability; and
* **Optional (O)** (but not specifically recommended) properties provide richer description.

**Those clients who wish to enhance the prospects that their metadata will be found, cited, and linked
to original research are strongly encouraged to submit both the Recommended and Mandatory sets of
properties.** Together, the Mandatory and Recommended sets of properties and their sub-properties are
especially valuable to information seekers and added-service providers, such as indexers. The Metadata
Working Group members strongly urge the inclusion of metadata identified as Recommended for the
purpose of achieving greater exposure for the resource’s metadata record and, therefore, the underlying
research itself.

The properties listed in `Table 1`_ have the obligation level Mandatory, and must be supplied when
submitting DataCite metadata. The properties listed in `Table 2`_  have one of the obligation levels
**Recommended** or **Optional** and may be supplied when submitting DataCite metadata.

The prospect that a resource's metadata will be found, cited, and linked is enhanced by using the
combined Mandatory and Recommended "super set" of properties and sub-properties. These are bolded in Tables 1 and 2.

Of the Recommended set of properties, the most important to use is the ``Description`` property,
together with the Recommended sub-property ``descriptionType="Abstract"`` (see DataCite
Properties and property 17). Appendix 1 includes detailed descriptions of controlled list values, using bold text to indicate those values that are especially important for information seekers and added service providers. It cannot be emphasized enough how valuable an Abstract is to other scholars in
finding the resource and then determining whether or not the resource, once found, is worth
investigating further, re-using, or validating.

.. _Table 1:

Table 1: DataCite Mandatory Properties
-----------------------------------------

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 1  | **Identifier**                                                                          | M          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with mandatory type sub-property)                                                      |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 2  | **Creator**                                                                             | M          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with optional given name, family name, name identifier and affiliation sub-properties) |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 3  | **Title**                                                                               | M          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with optional type sub-properties)                                                     |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 4  | **Publisher**                                                                           | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 5  | **PublicationYear**                                                                     | M          |
+----+-----------------------------------------------------------------------------------------+------------+
| 10 | **ResourceType**                                                                        | M          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with mandatory general type description sub- property)                                 |            |
+----+-----------------------------------------------------------------------------------------+------------+

.. _Table 2:

Table 2: DataCite Recommended and Optional Properties
------------------------------------------------------

+----+-----------------------------------------------------------------------------------------+------------+
| ID | Property                                                                                | Obligation |
|    |                                                                                         |            |
+====+=========================================================================================+============+
| 6  | **Subject**                                                                             | R          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with scheme sub-property)                                                              |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 7  | **Contributor**                                                                         | R          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with optional given name, family name, name identifier and affiliation sub-properties) |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 8  | **Date**                                                                                | R          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with type sub-property)                                                                |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 9  | Language                                                                                | O          |
+----+-----------------------------------------------------------------------------------------+------------+
| 11 | AlternateIdentifier                                                                     | O          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with type sub-property)                                                                |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 12 | **RelatedIdentifier**                                                                   | R          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with type and relation type sub-properties)                                            |            |
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
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with type sub-property)                                                                |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 18 | **GeoLocation**                                                                         | R          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with point, box, place, and polygon sub-properties)                                    |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 19 | FundingReference                                                                        | O          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with name, identifier, and award related sub-properties)                               |            |
+----+-----------------------------------------------------------------------------------------+------------+
| 20 | RelatedItem                                                                             | O          |
|    |                                                                                         |            |
|    |                                                                                         |            |
|    | (with identifier, creator, title, publication year, volume, issue, number, page,        |            |
|    |                                                                                         |            |
|    | publisher, edition, and contributor sub-properties)                                     |            |
+----+-----------------------------------------------------------------------------------------+------------+
