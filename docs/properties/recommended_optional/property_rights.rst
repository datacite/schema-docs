16. Rights
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Any rights information for this resource.

The property may be repeated to record complex rights characteristics.

**Allowed values, examples, other constraints:**

Free text.

Provide a rights management statement for the resource or reference a service providing such information. Include embargo information if applicable.

Use the complete title of a license and include version information if applicable.

May be used for software licenses.

Examples:

* Creative Commons Attribution 4.0 International
* Apache License, Version 2.0

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <rightsList>
    <rights xml:lang="en" schemeURI="https://spdx.org/licenses/" rightsIdentifierScheme="SPDX" rightsIdentifier="CC-BY-4.0" rightsURI="https://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International</rights>
  </rightsList>

.. _16.a:

16.a rightsURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the license

**Allowed values, examples, other constraints:**

Example: https://creativecommons.org/licenses/by/3.0/de/

.. _16.b:

16.b rightsIdentifier
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A short, standardized version of the license name

**Allowed values, examples, other constraints:**

Example: CC-BY-3.0

A list of identifiers for commonly-used licenses may be found here: (https://spdx.org/licenses/).

.. _16.c:

16.c rightsIdentifierScheme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the scheme

**Allowed values, examples, other constraints:**

Example: SPDX

.. _16.d:

16.d schemeURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the rightsIdentifierScheme

**Allowed values, examples, other constraints:**

Example: https://spdx.org/licenses/
