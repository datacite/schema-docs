relatedIdentifierType
=====================================

*Used by:*

* :ref:`12.a`
* :ref:`20.1.a`

*Options:*

.. contents:: :local:


.. _ARK:

ARK
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Archival Resource Key

**Description:** A URI designed to support long-term access to information objects. In general, ARK syntax is of the form (brackets, []. indicate optional elements):

``[http://NMA/]ark:/NAAN/Name [Qualifier]``.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ARK" relationType="IsCitedBy">ark:/13030/tqb3kh97gh8w</relatedIdentifier>


.. _arXiv:

arXiv
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** arXiv identifier

**Description:** arXiv.org is a repository of preprints of scientific papers in the fields of mathematics, physics, astronomy, computer science, quantitative biology, statistics, and quantitative finance.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="arXiv" relationType="IsCitedBy">arXiv:0706.0001</relatedIdentifier>


.. _bibcode:

bibcode
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Astrophysics Data System bibliographic codes

**Description:** A standardized 19-character identifier according to the syntax ``yyyyjjjjjvvvvmppppa``. See http://info-uri.info/registry/OAIHandler?verb=GetRecord&metadataPrefix=reg&identifier=info:bibcode/.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="bibcode" relationType="IsCitedBy">2018AGUFM.A24K..07S</relatedIdentifier>

Note: bibcodes can be searched via https://ui.adsabs.harvard.edu/ or resolved using ``https://ui.adsabs.harvard.edu/abs/<bibcode>``.


.. _DOI:

DOI
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Digital Object Identifier

**Description:** A character string used to uniquely identify an object. A DOI name is divided into two parts, a prefix and a suffix, separated by a slash.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="DOI" relationType="IsSupplementTo">10.1016/j.epsl.2011.11.037</relatedIdentifier>


.. _EAN13:

EAN13
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** European Article Number (now renamed International Article Number, but retaining the original acronym)

**Description:** A 13-digit barcoding standard that is a superset of the original 12-digit Universal Product Code (UPC) system.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="EAN13" relationType="Cites">9783468111242</relatedIdentifier>


.. _EISSN:

EISSN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Electronic International Standard Serial Number

**Description:** ISSN used to identify periodicals in electronic form (eISSN or e-ISSN).

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="eISSN" relationType="Cites">1562-6865</relatedIdentifier>


.. _Handle:

Handle
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Handle

**Description:** This refers specifically to an ID in the Handle system operated by the Corporation for National Research Initiatives (CNRI).

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="Handle" relationType="References">10013/epic.10033</relatedIdentifier>


.. _IGSN:

IGSN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** International Geo Sample Number

**Description:** A 9-digit alphanumeric code that uniquely identifies samples from our natural environment and related sampling features.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="IGSN" relationType="References">IECUR0097 </relatedIdentifier>


.. _ISBN:

ISBN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** International Standard Book Number

**Description:** A unique numeric book identifier. There are 2 formats: a 10-digit ISBN format and a 13-digit ISBN.

**Example:**

.. code:: xml

  <relatedIdentifier><relatedIdentifier relatedIdentifierType="ISBN" relationType="IsPartOf">978-3-905673-82-1 </relatedIdentifier>


.. _ISSN:

ISSN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** International Standard Serial Number

**Description:** A unique 8-digit number used to identify a print or electronic periodical publication.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISSN" relationType="IsPartOf">0077-5606 </relatedIdentifier>


.. _ISTC:

ISTC
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** International Standard Text Code

**Description:** A unique “number" assigned to a textual work. An ISTC consists of 16 numbers and/or letters.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="ISTC" relationType="Cites">0A9 2002 12B4A105 7</relatedIdentifier>


.. _LISSN:

LISSN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Linking ISSN

**Description:** The linking ISSN or ISSN-L enables collocation or linking among different media versions of a continuing resource.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="LISSN" relationType="Cites">1188-1534</relatedIdentifier>


.. _LSID:

LSID
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Life Science Identifiers

**Description:** A unique identifier for data in the Life Science domain. Format: ``urn:lsid:authority:namespace:identifier:revision``.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="LSID" relationType="Cites">urn:lsid:ubio.org:namebank:11815</relatedIdentifier>


.. _PMID:

PMID
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** PubMed identifier

**Description:** A unique number assigned to each PubMed record.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="PMID" relationType="IsReferencedBy">12082125</relatedIdentifier>


.. _PURL:

PURL
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Persistent Uniform Resource Locator

**Description:** A PURL has three parts: (1) a *protocol*, (2) a *resolver address*, and (3) a *name*.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="PURL" relationType="Cites">http://purl.oclc.org/foo/bar</relatedIdentifier>


.. _UPC:

UPC
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Universal Product Code

**Description:** A barcode symbology used for tracking trade items in stores. Its most common form, the UPC-A, consists of 12 numerical digits.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="UPC" relationType="Cites">123456789999</relatedIdentifier>


.. _URL:

URL
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Uniform Resource Locator

**Description:** Also known as web address, a URL is a specific character string that constitutes a reference to a resource. The syntax is: ``scheme://domain:port/path?query_string#fragment_id``.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URL" relationType="IsCitedBy">http://www.heatflow.und.edu/index2.html</relatedIdentifier>


.. _URN:

URN
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Uniform Resource Name

**Description:** A unique and persistent identifier of an electronic document. The syntax is: ``urn:<NID>:<NSS>``. The leading urn: sequence is case-insensitive, <NID> is the namespace identifier, <NSS> is the namespace-specific string.

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="URN" relationType="IsSupplementTo">urn:nbn:de:101:1-201102033592</relatedIdentifier>


.. _w3id:

w3id
~~~~~~~~~~~~~~~~~~~~~~~~~

**Full Name:** Permanent identifier for Web applications

**Description:** Mostly used to publish vocabularies and ontologies. The letters ‘w3’ stand for “World Wide Web".

**Example:**

.. code:: xml

  <relatedIdentifier relatedIdentifierType="w3id" relationType="IsCitedBy">https://w3id.org/games/spec/coil#Coil_Bomb_Die_Of_Age</relatedIdentifier>
