.. _1:

1. Identifier
====================

**Obligation:** Mandatory

**Occurrences:** 1

**Definition:** The Identifier is a unique string that identifies a resource.

For software, determine whether the identifier is for a specific version of a piece of software, (per the Force11 Software Citation Principles [#f1]_), or for all versions.

**Allowed values, examples, other constraints:**

A DOI (Digital Object Identifier) registered by a DataCite Member. The format should be ``10.21384/foo``.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none

.. rubric:: Example XML

.. code:: xml

 <identifier identifierType="DOI">10.21384/foo</identifier>

.. _1.a:

1.a identifierType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of Identifier.

**Allowed values, examples, other constraints:**

*Controlled List Value:*

* DOI



.. rubric:: Footnotes
.. [#f1] Smith AM, Katz DS, Niemeyer KE, FORCE11 Software Citation Working Group. (2016) Software citation principles. PeerJ Computer Science 2:e86 https://doi.org/10.7717/peerj-cs.86
