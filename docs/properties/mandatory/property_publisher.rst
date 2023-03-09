.. _4:

4. Publisher
====================

**Obligation:** Mandatory

**Occurrences:** 1

**Definition:** The name of the entity that holds, archives, publishes, prints, distributes, releases, issues, or produces the resource. This property will be used to formulate the citation, so consider the prominence of the role.

For software, use Publisher for the code repository. If there is an entity other than a code repository, that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the property :ref:`7` with contributorType "hostingInstitution" for the code repository.

**Allowed values, examples, other constraints:**

Examples:

* World Data Center for Climate (WDCC)
* GeoForschungsZentrum Potsdam (GFZ)
* Consejo Superior de Investigaciones Científicas
* University of Tokyo
* GitHub

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

 <publisher xml:lang="en" publisherIdentifier="https://ror.org/04z8jg394" publisherIdentifierScheme="ROR" schemeURI="https://ror.org/">Helmholtz Centre Potsdam - GFZ German Research Centre for Geosciences</publisher>

.. _4.a:

4.a publisherIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Uniquely identifies the publisher, according to various schemes.

**Allowed values, examples, other constraints:**

Examples:

* https://doi.org/10.17616/R3989R
* https://ror.org/04z8jg394
* https://viaf.org/viaf/151411898/
* https://www.wikidata.org/wiki/Q7842

.. _4.b:

4.b publisherIdentifierScheme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The name of the publisher identifier scheme.

**Allowed values, examples, other constraints:**

If publisherIdentifier is used, publisherIdentifierScheme is mandatory.

Examples:

* re3data
* ROR
* VIAF
* Wikidata
* Crossref Funder ID
* ISNI
* OpenDOAR
* FAIRsharing
* ISSN

.. _4.c:

4.c schemeURI
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the publisher identifier scheme.

**Allowed values, examples, other constraints:**

Examples:

* https://www.re3data.org/
* https://ror.org/
* https://viaf.org/
* https://www.wikidata.org
