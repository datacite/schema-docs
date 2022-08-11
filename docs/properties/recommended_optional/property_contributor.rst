7. Contributor
====================

**Occurrences:** 0-n

**Definition:** The institution or person responsible for collecting, managing, distributing, or otherwise contributing to the development of the resource. To supply multiple contributors, repeat this property.

For software, if there is an alternate entity that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the contributorType "hostingInstitution" for the code repository.

For instruments, if there is an institution responsible for the management of the instrument (for example, the legal owner, the operator, or an institute providing access to the instrument), use the contributorType “hostingInstitution” for the owner of the instrument.

**Allowed values, examples, other constraints:**

Note: DataCite infrastructure supports up to 10,000 names. For name lists above that size, consider attribution via linking to the related metadata.

Examples: Charpy, Antoine; Foo Data Center

*Sub-properties:*

.. contents:: :local:

.. _7.a:

7.a contributorType
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of contributor of the resource

**Allowed values, examples, other constraints:**

If Contributor is used, then contributorType is mandatory.

*Controlled List Values:*

* ContactPerson
* DataCollector
* DataCurator
* DataManager
* Distributor
* Editor
* HostingInstitution
* Producer
* ProjectLeader
* ProjectManager
* ProjectMember
* RegistrationAgency
* RegistrationAuthority
* RelatedPerson
* Researcher
* ResearchGroup
* RightsHolder
* Sponsor
* Supervisor
* WorkPackageLeader
* Other

See :doc:`Appendix 1: Controlled List Definitions - contributorType </appendices/appendix_1/contributorType>` for definitions.


.. _7.1:

7.1 contributorName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The full name of the contributor

**Allowed values, examples, other constraints:**

If Contributor is used, then contributorName is mandatory.

Examples: Patel, Emily; ABC Foundation

The personal name format should be: family, given. Non- roman names should be transliterated according to the `ALA-LC schemas <http://www.loc.gov/catdir/cpso/roman.html>`_.

7.1.a nameType
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of name

**Allowed values, examples, other constraints:**

*Controlled List Values:*

 * Organizational
 * Personal (default)


7.2 givenName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The personal or first name of the contributor

**Allowed values, examples, other constraints:**

Examples based on the `7.1`_ names: Emily


7.3 familyName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The surname or last name of the contributor

**Allowed values, examples, other constraints:**

Examples based on the `7.1`_ names: Patel


7.4 nameIdentifier
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** Uniquely identifies an individual or legal entity, according to various schemes

**Allowed values, examples, other constraints:**

The format is dependent upon scheme.


7.4.a nameIdentifierScheme
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The name of the name identifier scheme

**Allowed values, examples, other constraints:**

If nameIdentifier is used, nameIdentifierScheme is mandatory.

Examples: ORCID [#f1]_, ISNI, ROR, GRID.


7.4.b schemeURI
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the name identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* http://orcid.org
* http://www.isni.org
* https://ror.org/
* https://www.grid.ac/


7.5 affiliation
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** The organizational or institutional affiliation of the contributor

**Allowed values, examples, other constraints**

Free text.

The contributor's nameType may be *Organizational* or *Personal*. In the case of an organizational contributor, e.g., a research group,
this will often be the name of the institution to which that organization belongs.

7.5.a affiliationIdentifier
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-n

**Definition:** Uniquely identifies the organizational affiliation of the contributor.

**Allowed values, examples, other constraints:**

The format is dependent upon scheme. Examples:

* https://ror.org/04aj4c181
* grid.461819.3

7.5.b affiliationIdentifierScheme
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The name of the affiliation identifier scheme

**Allowed values, examples, other constraints:**

If affiliationIdentifier is used, affiliationIdentifierScheme is mandatory.

Examples: ROR, GRID

7.5.c SchemeURI
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** URI of the affiliation identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* https://isni.org
* https://ror.org/
* https://www.grid.ac/

.. rubric:: Footnotes
.. [#f1] When entering an ORCID, follow these style guidelines: https://orcid.org/content/journal- article-display-guidelines
