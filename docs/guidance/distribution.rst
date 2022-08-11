Using Distribution for a collection of files
=================================================================

If a repository wishes to provide a direct download link for a Direct Object of multiple files, it is recommended that the content be packaged in an archive file format (e.g., .TAR or .ZIP file), to which the contentUrl would resolve. In cases where there are multiple files that cannot be packaged in an archive format (for instance, due to the large size of individual files), it is recommended that the repository employ the BagIt file packaging specification (IETF RFC 8493, https://www.rfc-editor.org/rfc/rfc8493.html).

BagIt defines “a set of hierarchical file layout conventions for storage and transfer of arbitrary digital content.” A “bag” is a structured file system directory that MUST include the following required elements:

- A bag declaration file, named “bagit.txt”, that details the version of the BagIt specification as well as the character encoding for metadata files (e.g., UTF-8).
- A subdirectory named “data/”, which is intended to hold the bag’s content payload but will be empty in the current use case.
- A manifest file that includes a checksum value and relative path for each file; the checksum algorithm will be indicated in the filename (e.g., “manifest-md5.txt” if the md5 algorithm is employed).
- A TSV file named “fetch.txt.” Each line of this file refers to a single content file and should include the following columns, in this order:

   - An absolute and fully-resolvable URL for the file’s download location
   - The length of the file, expressed as a number of octets (or “-” if unspecified)
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
