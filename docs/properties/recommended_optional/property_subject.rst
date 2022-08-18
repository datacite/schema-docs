6. Subject
====================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** Subject, keyword, classification code, or key phrase describing the resource

**Allowed values, examples, other constraints:**

Free text

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <subjects>
    <subject xml:lang="en" subjectScheme="Library of Congress Subject Headings (LCSH)" schemeURI="https://id.loc.gov/authorities/subjects.html" valueURI="https://id.loc.gov/authorities/subjects/sh2009009655.html">Climate change mitigation</subject>
    <subject xml:lang="en" subjectScheme="ANZSRC Fields of Research" schemeURI="https://www.abs.gov.au/statistics/classifications/australian-and-new-zealand-standard-research-classification-anzsrc" classificationCode="370201">Climate change processes</subject>
  </subject>

6.a subjectScheme
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the subject scheme or classification code or authority if one is used

**Allowed values, examples, other constraints:**

Free text

Examples:

* Library of Congress Subject Headings (LCSH)
* ANZSRC Fields of Research

6.b schemeURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the subject identifier scheme

**Allowed values, examples, other constraints:**

Example: https://id.loc.gov/authorities/subjects.html

6.c valueURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the subject term

**Allowed values, examples, other constraints:**

Example:
https://id.loc.gov/authorities/ subjects/sh85118622.html

6.d classificationCode
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The classification code used for the subject term in the subject scheme

**Allowed values, examples, other constraints:**

Example:
310607
(where 310607 is the classification code associated with the subject term “Nanobiotechnology” in the ANZSRC Fields of Research subject scheme)

The classificationCode sub-property may be used for subject schemes, like ANZSRC, which do not have valueURIs for each subject term.
