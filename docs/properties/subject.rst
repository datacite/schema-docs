.. _6:

6. Subject
====================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** Subject, keyword, classification code, or key phrase describing the resource.

**Allowed values, examples, other constraints:**

Free text.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none
    
.. rubric:: Example

.. tabs::

   .. code-tab:: xml

      <subjects>
        <subject xml:lang="en" subjectScheme="Library of Congress Subject Headings (LCSH)" schemeURI="https://id.loc.gov/authorities/subjects.html" valueURI="https://id.loc.gov/authorities/subjects/sh2009009655.html">Climate change mitigation</subject>
        <subject xml:lang="en" subjectScheme="ANZSRC Fields of Research" schemeURI="https://www.abs.gov.au/statistics/classifications/australian-and-new-zealand-standard-research-classification-anzsrc" classificationCode="370201">Climate change processes</subject>
      </subject>
   
   .. code-tab:: json

      "subjects": [
        {
          "subject": "Climate change mitigation",
          "schemeUri": "https://id.loc.gov/authorities/subjects.html",
          "valueUri": "https://id.loc.gov/authorities/subjects/sh2009009655.html",
          "subjectScheme": "Library of Congress Subject Headings (LCSH)",
          "lang": "en"
        },
        {
          "subject": "Climate change processes",
          "schemeUri": "https://www.abs.gov.au/statistics/classifications/australian-and-new-zealand-standard-research-classification-anzsrc",
          "valueUri": "https://id.loc.gov/authorities/subjects/sh2009009655.html",
          "subjectScheme": "ANZSRC Fields of Research",
          "classificationCode": "370201",
          "lang": "en"
        }
      ]

.. _6.a:

6.a subjectScheme
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The name of the subject scheme or classification code or authority if one is used.

**Allowed values, examples, other constraints:**

Free text.

Examples:

* Library of Congress Subject Headings (LCSH)
* ANZSRC Fields of Research

.. _6.b:

6.b schemeURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the subject identifier scheme.

**Allowed values, examples, other constraints:**

Example: https://id.loc.gov/authorities/subjects.html

.. _6.c:

6.c valueURI
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the subject term.

**Allowed values, examples, other constraints:**

Example:
https://id.loc.gov/authorities/subjects/sh85118622.html


.. _6.d:

6.d classificationCode
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The classification code used for the subject term in the subject scheme.

**Allowed values, examples, other constraints:**

Example:
310607
(where 310607 is the classification code associated with the subject term “Nanobiotechnology” in the ANZSRC Fields of Research subject scheme)

The classificationCode sub-property may be used for subject schemes, like ANZSRC, which do not have valueURIs for each subject term.


.. _6.x:

6.x xml:lang
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The language of the subject.

**Allowed values, examples, other constraints:**

`xml:lang` values must follow the pattern defined by the `XML schema language type <https://www.w3.org/TR/xmlschema-2/#language>`_, e.g.: fr, cmn, nys, swh.  See the W3C’s `Choosing a Language Tag <https://www.w3.org/International/questions/qa-choosing-language-tags>`_ for guidance on recommended values.