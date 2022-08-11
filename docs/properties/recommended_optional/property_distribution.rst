21. Distribution
====================

**Occurrences:** 0-n

**Definition:** Represents an accessible form of a resource such as downloadable files.

**Allowed values, examples, other constraints:**

The use of this property indicates directly downloadable distributions. Every distribution should represent the same resource in its entirety. It should NOT be used to describe collections.

Collections of files should be either using an archive format or a bagit folder structure. See :doc:`/guidance/distribution` for recommendations.

*Sub-properties:*

.. contents:: :local:

.. _21.a:

21.a mediaType
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Media type typically expressed using a MIME format (see `IANA site <http://www.iana.org/assignments/media-types/media-types.xhtml>`_ and `MDN reference <https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types>`_).

**Allowed values, examples, other constraints:**

If Distribution is used, mediaType is mandatory.

Only MIME formats are allowed: https://www.iana.org/assignments/media-types/media-types.xhtml

Examples:

- application/zip
- audio/mpeg

.. _21.b:

21.b contentUrl
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The URI leading to a content provided by a repository using a valid protocol.

**Allowed values, examples, other constraints:**

If Distribution is used, contentUrl is mandatory.

Only URIs with schemes from IANA-registered schemes are allowed: https://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml

Examples:

- https://zenodo.org/record/6591787/files/frequent_bigrams.csv
- ftp://ds.internic.net/rfc/rfc1436.txt
- https://zenodo.org/record/6591787/files/bagit.zip
- https://zenodo.org/record/6591787/files/files.gzip

See :doc:`/guidance/distribution` for recommendations on archive file formats.

.. _21.b.1:

21.b.1 lastUpdated
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Date when the content URL was last updated.

**Allowed values, examples, other constraints:**

YYYY, YYYY-MM-DD, YYYYMM-DDThh:mm:ssTZD or any other format or level of granularity described in W3CDTF [#f1]_.

.. _21.b.2:

21.b.2 byteSize
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The size of a distribution in bytes.

**Allowed values, examples, other constraints:**

The size in bytes can be approximated (as a decimal) when the precise size is not known.

Examples:
- 1048576 for 1 Megabyte

.. _21.c:

21.c checkSum
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A value that allows the contents of a file to be authenticated.

**Allowed values, examples, other constraints:**

This attribute allows the results of a variety of checksum and cryptographic message digest algorithms to be represented.

.. _21.c.1:

21.c.1 algorithm
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Identifies the algorithm used to produce the checksum.

**Allowed values, examples, other constraints:**

If checkSum is used, algorithm is mandatory.

Recommended values should follow Version 2.2 of SPDX: https://spdx.org/rdf/terms/#d4e1968

Examples:

- MD2
- MD4
- MD5
- MD6
- SHA-1
- SHA-224
- SHA-256
- SHA-384
- SHA-512

.. _21.d:

21.d accessRights
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A rights statement that describes how the distribution is accessed.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/access_rights.nt

To provide copyright or licensing information, use the :doc:`Rights </properties/recommended_optional/property_rights>` property.

Examples:

- embargoed access
- metadata only access
- open access


.. _21.d.1:

21.d.1 accessRightsUri
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI used to define the access rights.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary for to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/access_rights.nt

Examples:

- https://vocabularies.coar-repositories.org/access_rights/c_abf2/ for “open access”
- http://purl.org/coar/access_right/c_14cb for “metadata only”

.. rubric:: Footnotes
.. [#f1] https://www.w3.org/TR/NOTE-datetime
