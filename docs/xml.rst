XML Schema and Examples
=====================================

.. note::
   This page contains links to version 4.4 and will be updated after the official release of version 4.5.

XML Schema
--------------------------------

The XML Schema is available here:
https://schema.datacite.org/meta/kernel-4.4/metadata.xsd

XML Examples
------------------------
Examples for various resource types and special cases can be found at https://schema.datacite.org/meta/kernel-4.4/index.html.

..
  New XML Examples

  .. code:: xml

    <distributions>
       <distribution mediaType="image/png">
         <contentURL lastUpdated="2022-05-05" byteSize="1236546456">http://example.org/data.png</contentURL>
         <checksum algorithm="MD5">d41d8cd98f00b204e9800998ecf8427e</checksum>
         <accessRights accessRightsSchema="https://vocabularies.coar-repositories.org/access_rights/access_rights.nt">embargoedaccess</accessRights>
       </distribution>
       <distribution mediaType="text/csv">
         <contentURL>http://example.org/data.csv</contentURL>
       </distribution>
     </distributions>

  .. code:: xml

    <resource xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://datacite.org/schema/kernel-4" xsi:schemaLocation="http://datacite.org/schema/kernel-4 https://schema.datacite.org/meta/kernel-4.4/metadata.xsd">
      <identifier identifierType="DOI">10.5072/example-instrument</identifier>
      <creators>
        <creator>
        <creatorName nameType="Organizational">DECTRIS</creatorName>
        <nameIdentifier schemeURI="https://www.wikidata.org/" nameIdentifierScheme="Wikidata">Q107529885</nameIdentifier>
        </creator>
      </creators>
      <titles>
        <title xml:lang="en-US">FPilatus detector at MX station 14.1</title>
      </titles>
      <publisher xml:lang="en">Helmholtz-Zentrum Berlin für Materialien und Energie</publisher>
      <publicationYear>2021</publicationYear>
      <contributors>
        <contributor contributorType="HostingInstitution">
        <contributorName nameType="Organizational">Helmholtz-Zentrum Berlin für Materialien und Energie</contributorName>
        <nameIdentifier schemeURI="https://ror.org/" nameIdentifierScheme="ROR">https://ror.org/02aj13c28</nameIdentifier>
        </contributor>
      </contributors>
      <resourceType resourceTypeGeneral="Instrument">Raster image pixel detector</resourceType>
      <alternateIdentifiers>
        <alternateIdentifier alternateIdentifierType="SerialNumber">1234567</alternateIdentifier>
      </alternateIdentifiers>
      <relatedIdentifiers>
        <relatedIdentifier relatedIdentifierType="Handle" relationType="IsPartOf" resourceTypeGeneral="Instrument">1234.1675</relatedIdentifier>
        <relatedIdentifier relatedIdentifierType="URL" relationType="References" resourceTypeGeneral="Text">https://www.dectris.com/products/pilatus3/pilatus3-s-for-synchrotron/details/pilatus3-s-6m</relatedIdentifier>
      </relatedIdentifiers>
      <descriptions>
        <description xml:lang="en-US" descriptionType="Abstract">The Pilatus 6M pixel-detector at the MX station 14.1</description>
        <description xml:lang="en-US" descriptionType="TechnicalInfo">Model Name: PILATUS3 S 6M. Instrument type: Raster image pixel detector. Measured variables: X-ray.</description>
      </descriptions>
    </resource>
