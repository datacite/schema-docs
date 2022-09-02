.. _21:

21. Distribution
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Represents an accessible form of a resource such as downloadable files.

**Allowed values, examples, other constraints:**

The use of this property indicates directly downloadable distributions. Every distribution should represent the same resource in its entirety. It should NOT be used to describe collections.

Collections of files should be either using an archive format or a BagIt folder structure. See :doc:`/guidance/distribution` for recommendations.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <distributions>
     <distribution mediaType="application/gzip">
       <contentURL lastUpdated="2022-05-05" byteSize="1236546456">https://example.org/bagit.gzip</contentURL>
       <checksum algorithm="MD5">d41d8cd98f00b204e9800998ecf8427e</checksum>
       <accessRights accessRightsUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
     </distribution>
   </distributions>

.. _21.a:

21.a mediaType
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Media type expressed using a MIME format.

**Allowed values, examples, other constraints:**

If Distribution is used, mediaType is mandatory.

Only MIME formats are allowed: see `IANA site <http://www.iana.org/assignments/media-types/media-types.xhtml>`_ and `MDN reference <https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types>`_.

Examples:

- application/zip
- audio/mpeg

.. _21.1:

21.1 contentURL
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The URL leading to content provided by a repository using a valid protocol.

**Allowed values, examples, other constraints:**

If Distribution is used, contentURL is mandatory.

URLs should use schemes that are registered with IANA (e.g., https, ftp): https://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml

Examples:

- https://example.org/data.csv
- ftp://example.org/data.txt
- https://example.org/bagit.zip
- https://example.org/files.gzip

See :doc:`/guidance/distribution` for recommendations on archive file formats.

.. _21.1.a:

21.1.a lastUpdated
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Date when the content URL value was last updated. [#f1]_

**Allowed values, examples, other constraints:**

YYYY, YYYY-MM-DD, YYYYMM-DDThh:mm:ssTZD or any other format or level of granularity described in W3CDTF [#f2]_.

.. _21.1.b:

21.1.b byteSize
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The size of a distribution in bytes. The value is related to the object in :ref:`21.1`.

**Allowed values, examples, other constraints:**

The size in bytes can be approximated (as a decimal) when the precise size is not known.

Examples:

- 1048576 for 1 Megabyte

.. _21.2:

21.2 checkSum
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A value that allows the integrity of a file to be verified. The value is related to the object in :ref:`21.1`.

**Allowed values, examples, other constraints:**

This attribute allows the results of a variety of checksum and cryptographic message digest algorithms to be represented.

.. _21.2.a:

21.2.a algorithm
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Identifies the algorithm used to produce the checksum.

**Allowed values, examples, other constraints:**

If checkSum is used, algorithm is mandatory.

Recommended values should follow Version 2.3 of SPDX: https://spdx.org/rdf/terms/#d4e1968

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

.. _21.3:

21.3 accessRights
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A rights statement that describes how the distribution is accessed.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/

To provide copyright or licensing information, use the :ref:`16` property.

Examples:

- embargoed access
- metadata only access
- open access


.. _21.3.a:

21.3.a accessRightsUri
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI used to define the access rights.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary for to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/

Examples:

- http://purl.org/coar/access_right/c_abf2 for “open access”
- http://purl.org/coar/access_right/c_14cb for “metadata only”

.. rubric:: Footnotes
.. [#f1] To determine when the file contents were last updated, compare :ref:`21.2` values.
.. [#f2] https://www.w3.org/TR/NOTE-datetime
