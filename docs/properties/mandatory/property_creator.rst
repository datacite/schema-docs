2. Creator
====================

**Occurrences:** 1-n

**Definition:** The main researchers involved in producing the data, or the authors of the publication, in priority order. For instruments this is the manufacturer or developer of the instrument. To supply multiple creators, repeat this property.

**Allowed values, examples, other constraints:**

May be a corporate/institutional or personal name. Note: DataCite infrastructure supports up to 10,000 names. For name lists above that size, consider attribution via linking to the related metadata.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

::

  <creators>
      <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
          <nameIdentifier schemeURI="https://orcid.org/" nameIdentifierScheme="ORCID">0000-0001-5727-2427</nameIdentifier>
          <affiliation affiliationIdentifier="https://ror.org/03efmqc40" affiiationIdentifierScheme="ROR" SchemeURI="https://ror.org">Arizona State University</affiliation>
      </creator>
      <creator>
          <creatorName xml:lang="en" nameType="Organizational">California Digital Library</creatorName>
          <nameIdentifier schemeURI="https://ror.org/" nameIdentifierScheme="ROR">https://ror.org/03yrm5c26</nameIdentifier>
      </creator>
  </creators>

2.1 creatorName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The full name of the creator.

**Allowed values, examples, other constraints:**

Examples: Charpy, Antoine; Jemison, Mae; Foo Data Center

Note that the personal name, format should be: family, given. Names in non-roman scripts may be transliterated according to the `ALA-LC tables <https://www.loc.gov/catdir/cpso/roman.html>`_.


2.1.a nameType
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of name

**Allowed values, examples, other constraints:**

*Controlled List Values:*

 * Organizational
 * Personal (default)


2.2 givenName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The personal or first name of the creator

**Allowed values, examples, other constraints:**

Examples based on the 2.1 names: Antoine; Mae


2.3 familyName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The surname or last name of the creator

**Allowed values, examples, other constraints:**

Examples based on the 2.1 names: Charpy; Jemison


.. _2.4:

2.4 nameIdentifier
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** Uniquely identifies an individual or legal entity, according to various schemes.

**Allowed values, examples, other constraints:**

The format is dependent upon scheme.

Examples:

* https://orcid.org/0000-0001-5727-2427
* https://isni.org/isni/0000000492299539
* https://ror.org/04aj4c181


2.4.a nameIdentifierScheme
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The name of the name identifier scheme

**Allowed values, examples, other constraints:**

If nameIdentifier is used, nameIdentifierScheme is mandatory.

Examples:

* ORCID
* ISNI
* ROR


2.4.b schemeURI
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the name identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* https://orcid.org/
* https://isni.org/
* https://ror.org/


.. _2.5:

2.5 affiliation
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** The organizational or institutional affiliation of the creator

**Allowed values, examples, other constraints**

Free text.

The creator’s nameType may be *Organizational* or *Personal*. In the case of an organizational creator, e.g., a research group,
this will often be the name of the institution to which that organization belongs.

Examples:

* German National Library of Science and Technology
* DataCite


.. _2.5.a:

2.5.a affiliationIdentifier
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Uniquely identifies the organizational affiliation of the creator.

**Allowed values, examples, other constraints:**

The format is dependent upon scheme.

Examples:

* https://ror.org/04aj4c181
* https://isni.org/isni/0000000492299539


2.5.b affiliationIdentifierScheme
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The name of the affiliation identifier scheme

**Allowed values, examples, other constraints:**

If affiliationIdentifier is used, affiliationIdentifierScheme is mandatory.

Examples:

* ROR
* ISNI


.. _2.5.c:

2.5.c schemeURI
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the affiliation identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* https://ror.org/
* https://isni.org/
