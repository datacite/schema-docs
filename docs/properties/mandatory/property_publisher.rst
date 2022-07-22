4. Publisher
====================

**Occurrences:** 1

**Definition:** The name of the entity that holds, archives, publishes, prints, distributes, releases, issues, or produces the resource. This property will be used to formulate the citation, so consider the prominence of the role.

For software, use Publisher for the code repository. If there is an entity other than a code repository, that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the property Contributor with contributorType "hostingInstitution" for the code repository.

**Allowed values, examples, other constraints:**

Examples: World Data Center for Climate (WDCC); GeoForschungsZentrum Potsdam (GFZ); Geological Institute, University of Tokyo, GitHub

4.a publisherIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Uniquely identifies the publisher, according to various schemes.

**Allowed values, examples, other constraints:**

Examples:

* http://doi.org/10.17616/R3P88S
* https://ror.org/01k4yrm29
* https://viaf.org/viaf/151411898/
* https://www.wikidata.org/wiki/Q34433


4.b publisherIdentifierScheme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The name of the publisher identifier scheme

**Allowed values, examples, other constraints:**

If publisherIdentifier is used, publisherIdentifierScheme is mandatory.

Examples:

* ROR
* Crossref Funder ID
* VIAF
* Re3data
* Wikidata
* ISNI
* OpenDOAR
* FAIRsharing
* Ringgold
* ISSN

4.c schemeURI
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The URI of the publisher identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* https://ror.org/
* https://www.re3data.org/
* https://fairsharing.org/
* https://www.wikidata.org
