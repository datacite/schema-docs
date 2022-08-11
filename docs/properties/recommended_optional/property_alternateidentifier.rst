11. AlternateIdentifier
========================

**Occurrences:** 0-n

**Definition:** An identifier other than the primary Identifier applied to the resource being registered. This may be any alphanumeric string which is unique within its domain of issue. May be used for local identifiers,  a serial number of an instrument or an inventory number. The AlternateIdentifier should be an additional identifier for the same instance of the resource (i.e., same location, same file).

**Allowed values, examples, other constraints:**

Free text

Example: E-GEOD-34814

*Sub-properties:*

.. contents:: :local:

11.a alternateIdentifierType
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of the AlternateIdentifier

**Allowed values, examples, other constraints:**

Free text

If alternateIdentifier is used, alternateIdentifierType is mandatory. For the above example, the alternateIdentifierType would be “A local accession number”
