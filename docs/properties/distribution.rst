.. _21:

21. Distribution
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Represents a form of a resource that can be accessed or retrieved, such as downloadable files. This property can be repeated if different variations are available.

**Allowed values, examples, other constraints:**

The use of this property indicates directly downloadable distributions. There is no expectation that different downloadable distributions must contain exactly equivalent information. Different distributions might include or exclude different subsets of the entire resource.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none

.. rubric:: Example

.. tabs::

   .. code-tab:: xml

        <distributions>
            <distribution>
                <contentURL byteSize="838861" mediaType="text/plain" accessType="Public" contentName="readme.txt">https://example.org/readme.txt</contentURL>
                <contentURL byteSize="524288" mediaType="application/json" accessType="Restricted" contentName="data.json">https://example.org/data.json"</contentURL>
            </distribution>
            <distribution>
                <contentURL byteSize="6081741" mediaType="application/zip" accessType="Public" contentName="package.zip">https://example.org/package.zip</contentURL>
            </distribution>
        </distributions>
   
   .. code-tab:: json
    
        "distributions": [
          [
            {
              "contentUrl": "https://example.org/readme.txt",
              "byteSize": 838861,
              "mediaType": "text/plain",
              "accessType": "Public",
              "contentName": "readme.txt"
            },
            {
              "contentUrl": "https://example.org/data.json",
              "byteSize": 5242880,
              "mediaType": "application/json",
              "accessType": "Restricted",
              "contentName": "data.json"
            }
            ],
          [
            {
              "contentUrl": "https://example.org/package.zip",
              "byteSize": 6081741,
              "mediaType": "application/zip",
              "accessType": "Public",
              "contentName": "package.json"
            }
          ]
        ]

.. _21.1:

21.1 contentURL
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1-n

**Definition:** The URL leading to content provided by a repository using a valid protocol.

**Allowed values, examples, other constraints:** 

If Distribution is used, at least one contentURL is mandatory. URLs should use schemes that are registered with IANA (e.g., https, ftp). [#f1]_

A contentURL can either represent an entire distribution, or a part of it. Collections of files can be represented either using a single contentURL (e.g., an archive format or a BagIt package) or as multiple contentURLs.

Examples:

* ``https://example.org/files/2023-06_ocean-temperature_pacific.csv``
* ``ftp://example.org/files/survey-responses_2022_deidentified.txt``
* ``https://example.org/files/census-microdata_2016.tar.gz``
* ``https://example.org/api/download?id=550e8400-e29b-41d4-a716-446644550000``
* ``https://data.example.org/records/98765/export``

.. _21.1.a:

21.1.a byteSize
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The size of the object retrievable via the contentURL in bytes.

**Allowed values, examples, other constraints:**

The size in bytes can be approximated (as an integer) when the precise size is not known.

Example:

* 1048576 (for 1 Megabyte)

.. _21.1.b:

21.1.b mediaType
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** Media type of the object retrievable via the contentURL.

**Allowed values, examples, other constraints:**

Media types (formerly known as MIME types) from the list maintained by IANA are strongly recommended. [#f2]_ Where no suitable IANA-registered media type exists, an appropriate community-accepted media type may be used.

Examples:

* application/zip
* audio/mpeg

.. _21.1.c:

21.1.c accessType
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of access for which the object at the contentURL is available.

**Allowed values, examples, other constraints:**

To describe access conditions for the overall resource, use the :ref:`22` property.

To provide copyright or licensing information, use the :ref:`16` property. To provide an embargo date, use the :ref:`8` property with dateType :ref:`Available`.

*Controlled List Values:*

 * :ref:`public`
 * :ref:`restricted`

See :doc:`Appendix 1: Controlled List Definitions - accessType </appendices/appendix-1/accessType>` for definitions.

.. _21.1.d:

21.1.d contentName
^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** A name or label assigned to the object represented by the contentURL. This may be the file name, a human-readable title, or other descriptive label.

**Allowed values, examples, other constraints:**

Example:

* ``2023-06_ocean-temperature_pacific.csv``
* ``survey-responses_2022_deidentified.txt``
* ``census-microdata_2016.tar.gz``
* ``Dmelanogaster_assembly_r6.48.fasta.gz``
* ``Sentinel2_AmazonBasin_20230615.tif``


.. rubric:: Footnotes
.. [#f1] See the IANA's list of `Uniform Resource Identifier (URI) Schemes <https://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml>`_.
.. [#f2] See the IANA's list of `Media Types <http://www.iana.org/assignments/media-types/media-types.xhtml>`_ and the MDN's documentation on `Media types (MIME types) <https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/MIME_types>`_ for guidance.