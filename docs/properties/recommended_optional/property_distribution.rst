.. _21:

21. Distribution
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Represents an accessible form of a resource such as downloadable files. This property can be repeated if different variations are available.

**Allowed values, examples, other constraints:**

The use of this property indicates directly downloadable distributions. Every distribution should represent the same resource in its entirety.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <distributions>
    <distribution>
      <file mediaType="application/gzip">
        <contentURL byteSize="1236546456">https://example.org/archive.zip</contentURL>
        <checksums>
              <checksum algorithm="MD5">d41d8cd98f00b204e9800998ecf8427e</checksum>
        </checksums>
        <accessLevel xml:lang="en" accessLevelURI="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
      </file>
    </distribution>
  </distributions>


.. _21.1:

21.1 file
~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1-n

**Definition:** A container in a computer system for storing information.

**Allowed values, examples, other constraints:**

If Distribution is used, at least one file is mandatory.

A file can either represent the entirety of the distribution, or a part of it. Collections of files can be described either using a single file (e.g., an archive format or a BagIt folder structure) or as multiple files. See :doc:`/guidance/distribution` for recommendations.


.. _21.1.a:

21.1.a mediaType
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Media type expressed using a MIME format.

**Allowed values, examples, other constraints:**

If file is used, mediaType is mandatory.

MIME formats are strongly recommended: see `IANA site <http://www.iana.org/assignments/media-types/media-types.xhtml>`_ and `MDN reference <https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types>`_.

Examples:

- application/zip
- audio/mpeg

.. _21.1.1:

21.1.1 contentURL
^^^^^^^^^^^^^^^^^^^^^

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

.. _21.1.1.a:

21.1.1.a byteSize
##########################

**Occurrences:** 0-1

**Definition:** The size of a distribution in bytes. The value is related to the object in :ref:`21.1.1`.

**Allowed values, examples, other constraints:**

The size in bytes can be approximated (as an integer) when the precise size is not known.

Examples:

- 1048576 for 1 Megabyte

.. _21.1.2:

21.1.2 checkSum
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-n

**Definition:** A value that allows the integrity of a file to be verified. The value is related to the object in :ref:`21.1.1`.

**Allowed values, examples, other constraints:**

This attribute allows the results of a variety of checksum and cryptographic message digest algorithms to be represented.

.. _21.1.2.a:

21.1.2.a algorithm
##########################

**Occurrences:** 1

**Definition:** Identifies the algorithm used to produce the checksum.

**Allowed values, examples, other constraints:**

If checkSum is used, algorithm is mandatory.

Recommended values should follow Version 2.3 of SPDX: https://spdx.org/rdf/terms/#d4e1968

Examples:

- MD5
- SHA-1
- SHA-256
- SHA-512

.. _21.1.3:

21.1.3 accessLevel
^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** A statement that describes how the distribution is accessed.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/

To provide copyright or licensing information, use the :ref:`16` property. To provide an embargo date, use the :ref:`8` property with :ref:`8.a` :ref:`Available`.

Examples:

- embargoed access
- metadata only access
- open access


.. _21.1.3.a:

21.1.3.a accessLevelURI
##########################

**Occurrences:** 0-1

**Definition:** The URI used to define the access level.

**Allowed values, examples, other constraints:**

Recommended values should follow the COAR vocabulary for to declare the access status of a resource: https://vocabularies.coar-repositories.org/access_rights/

Examples:

- http://purl.org/coar/access_right/c_abf2 for “open access”
- http://purl.org/coar/access_right/c_14cb for “metadata only access”
