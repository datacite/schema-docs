Using Distribution for a collection of files
=================================================================

Option 1: Use an archive file format
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
If a repository wishes to provide a direct download link for a resource containing multiple files, it is recommended that the content be packaged in an archive file format (e.g., .TAR or .ZIP file), to which the :ref:`21.1.1` would resolve. 


.. rubric:: Example for Distribution with an archive file format

.. code:: xml

  <distributions>
   <distribution>
     <file mediaType="application/gzip">
       <contentURL byteSize="1236546456">https://example.org/archive.zip</contentURL>
       <checksums>
             <checksum algorithm="MD5">d41d8cd98f00b204e9800998ecf8427e</checksum>
       </checksums>
       <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
     </file>
   </distribution>
 </distributions>

Option 2: Repeat the :ref:`21.1` sub-property
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
As an alternative to archive file formats, a collection of files within a single Distribution can be represented by repeating :ref:`21.1`.

.. rubric:: Example for Distribution with :ref:`21.1` repeated
 
.. code:: xml

<distributions>
   <distribution>
     <file mediaType="text/csv">
       <contentURL byteSize="1236546456">https://example.org/data.csv</contentURL>
       <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
     </file>
     <file mediaType="text/plain">
       <contentURL byteSize="200">https://example.org/README.txt</contentURL>
       <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
     </file>
   </distribution>
 </distributions>

Option 3: Use conventions to describe multiple files (e.g., BagIt)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
In cases where there are multiple files that cannot be packaged in an archive format (for instance, due to the large size of individual files), it is suggested that the repository employ a standard method for describing multpile files, such as BagIt [#f2]_ or Metalink [#f3]_.

BagIt
^^^^^^^^^^^^^^^^^^^^^

BagIt defines “a set of hierarchical file layout conventions for storage and transfer of arbitrary digital content.” A “bag” is a structured file system directory that MUST include the following required elements:

- A bag declaration file, named “bagit.txt”, that details the version of the BagIt specification as well as the character encoding for metadata files (e.g., UTF-8).
- A subdirectory named “data/”, which is intended to hold the bag’s content payload but will be empty in the current use case.
- A manifest file that includes a checksum value and relative path for each file; the checksum algorithm will be indicated in the filename (e.g., “manifest-md5.txt” if the md5 algorithm is employed).
- A TSV file named “fetch.txt.” Each line of this file refers to a single content file and should include the following columns, in this order:

   - An absolute and fully-resolvable URL for the file’s download location
   - The length of the file, expressed as a number of octets (or “-” if unspecified) [#f1]_
   - A relative filepath that indicates where the file should be positioned (e.g., “path/folder/file.csv”)

  The base directory can have any name, as illustrated by the figure below.

.. parsed-literal::

         bagit.zip
         |
         +-- bagit.txt
         |
         +-- manifest-<algorithm>.txt
         |
         |
         +-- data/
         |     |
         |     +-- [empty]
         |
         +-- fetch.txt

A user may then download the bag and use a script to parse the “fetch.txt”, retrieve files using the provided download URLs, and then saved to the appropriate location within the bag’s “data” directory based upon the provided relative path. Once all the content files have been retrieved, the entire bag MAY be validated to ensure the integrity of all content and the appropriate directory structure. Currently available tools for creating, updating, and validating BagIt bags include Python (https://github.com/LibraryOfCongress/bagit-python) and Java (https://github.com/LibraryOfCongress/bagit-java) libraries developed by the United States Library of Congress as well as the Digital Archivist's Resource Tool (DART), developed by the Academic Preservation Trust consortium (https://github.com/APTrust/dart).

.. rubric:: Example for Distribution with BagIt

.. code:: xml

  <distributions>
   <distribution>
     <file mediaType="application/gzip">
       <contentURL byteSize="1236546456">https://example.org/bagit.gzip</contentURL>
       <checksums>
             <checksum algorithm="MD5">d41d8cd98f00b204e9800998ecf8427e</checksum>
       </checksums>
       <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
     </file>
   </distribution>
 </distributions>

A note on multiple distributions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Every distribution should represent the same resource in its entirety. The property can be repeated to describe different formats of the same resource. Determining about how to describe multiple distributions of the same dataset is the responsibility of the metadata provider, taking into account their understanding of the expectations of users, and practices in the relevant community.

.. rubric:: Example for multiple distributions

.. code:: xml

  <distributions>
    <distribution>
      <file mediaType="text/csv">
        <contentURL byteSize="1236546456">https://example.org/data.csv</contentURL>
        <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
      </file>
    </distribution>
    <distribution>
      <file mediaType="application/vnd.ms-excel">
        <contentURL byteSize="1236546456">https://example.org/data.xls</contentURL>
        <accessLevel xml:lang="en" accessLevelUri="http://purl.org/coar/access_right/c_abf2">open access</accessRights>
      </file>
    </distribution>
  </distributions>

.. rubric:: Footnotes

.. [#f1] An octet is 8 bits, or 1 byte: `https://en.wikipedia.org/wiki/Octet_(computing) <https://en.wikipedia.org/wiki/Octet_(computing)>`_
.. [#f2] BagIt file packaging specification (IETF RFC 8493, https://www.rfc-editor.org/rfc/rfc8493.html)
.. [#f3] Metalink is an extensible metadata file format that describes one or more computer files available for download. https://en.wikipedia.org/wiki/Metalink