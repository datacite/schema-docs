Using RelatedItem for publication information and related resources
================================================================================

The :ref:`20` property was developed to satisfy two distinct use cases.

The first use case is **providing publication information** for journal articles, book chapters, and other resources that are published within another item. This information about the related item (the container) is needed to formulate a complete citation of the primary resource being described. For example, a book title is necessary to cite a book chapter, and a journal title and volume/issue number are necessary to cite a journal article.

The second use case is **providing information about related resources.**

- When a related resource *does not have an identifier*, the :ref:`20` property should be used to provide information about the related resource.
- When a related resource *has an identifier*, the :ref:`12` property should *always* be used. In addition, the :ref:`20` property may *optionally* be used to provide information about the related resource.

.. rubric:: Contents

.. contents:: :local:

Use case: Providing publication information for journal articles, book chapters, and more
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The RelatedItem property with relationType :ref:`IsPublishedIn` can be used to provide more complete publication for journal articles, book chapters, and other components of larger resources.

With the :ref:`IsPublishedIn` relationType, the following optional sub-properties may be used:

* :ref:`20.5`
* :ref:`20.6`
* :ref:`20.7`
* :ref:`20.8`
* :ref:`20.9`
* :ref:`20.11`

The related item that the resource is published in may have an identifier of this own. When the related item has an identifier, it may be included in the :ref:`20.1` attribute. In addition, the :ref:`12` property should also be supplied.

Example: Journal article in a journal (with an ISSN)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. tab-set-code::
  
  .. code:: xml

    <?xml version="1.0" encoding="UTF-8"?>
    <resource
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns="http://datacite.org/schema/kernel-4" xsi:schemaLocation="http://datacite.org/schema/kernel-4 http://schema.datacite.org/meta/kernel-4.4/metadata.xsd">
      <identifier identifierType="DOI">10.21384/ExampleArticle</identifier>
      <creators>
        <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
          <nameIdentifier schemeURI="https://orcid.org/" nameIdentifierScheme="ORCID">0000-0001-5727-2427</nameIdentifier>
          <affiliation affiliationIdentifier="https://ror.org/03efmqc40" affiiationIdentifierScheme="ROR" SchemeURI="https://ror.org">Arizona State University</affiliation>
        </creator>
      </creators>
      <titles>
        <title xml:lang="en">Example Article Title</title>
      </titles>
      <publisher xml:lang="en">Example Publisher</publisher>
      <publicationYear>2022</publicationYear>
      <resourceType resourceTypeGeneral="JournalArticle"></resourceType>
      <relatedIdentifiers>
        <relatedIdentifier relatedIdentifierType="ISSN" relationType="IsPublishedIn">1234-5678</relatedIdentifier>
      </relatedIdentifiers>
      <relatedItems>
        <relatedItem relationType="IsPublishedIn" relatedItemType="Journal">
          <relatedItemIdentifier relatedItemIdentifierType="ISSN">1234-5678</relatedItemIdentifier>
          <titles>
            <title>Journal of Metadata Examples</title>
          </titles>
          <publicationYear>2022</publicationYear>
          <volume>3</volume>
          <issue>4</issue>
          <number numberType="Article">2</number>
          <firstPage>20</firstPage>
          <lastPage>35</lastPage>
          <publisher>Example Publisher</publisher>
        </relatedItem>
      </relatedItems>
    </resource>

  .. code:: json

    {
      "data": {
          "type": "dois",
          "attributes": {
              "url": "https://example.org/RelatedItem1",
              "prefix": "10.21384/ExampleArticle",
              "creators": [
                  {
                      "name": "Garcia, Sofia",
                      "nameType": "Personal",
                      "givenName": "Sofia",
                      "familyName": "Garcia",
                      "affiliation": [
                          {
                              "name": "Arizona State University",
                              "schemeUri": "https://ror.org",
                              "affiliationIdentifier": "https://ror.org/03efmqc40"
                          }
                      ],
                      "nameIdentifiers": [
                          {
                              "schemeUri": "https://orcid.org",
                              "nameIdentifier": "https://orcid.org/0000-0001-5727-2427",
                              "nameIdentifierScheme": "ORCID"
                          }
                      ]
                  }
              ],
              "titles": [
                  {
                      "lang": "en",
                      "title": "Example Article Title"
                  }
              ],
              "publisher": "Example Publisher",
              "publicationYear": 2022,
              "types": {
                  "resourceTypeGeneral": "JournalArticle"
              },
              "relatedIdentifiers": [
                  {
                      "relationType": "IsPublishedIn",
                      "relatedIdentifier": "1234-5678",
                      "relatedIdentifierType": "ISSN"
                  }
              ],
              "relatedItems": [
                  {
                      "issue": "4",
                      "number": "2",
                      "titles": [
                          {
                              "title": "Journal of Metadata Examples"
                          }
                      ],
                      "volume": "3",
                      "lastPage": "35",
                      "firstPage": "20",
                      "publisher": "Example Publisher",
                      "numberType": "Article",
                      "relationType": "IsPublishedIn",
                      "publicationYear": "2022",
                      "relatedItemType": "Journal",
                      "relatedItemIdentifier": {
                          "relatedItemIdentifier": "1234-5678",
                          "relatedItemIdentifierType": "ISSN"
                      }
                  }
              ]
          }
      }
    }

Example: Digitized book chapter in a book (with no identifier)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. tab-set-code::

  .. code:: xml

    <?xml version="1.0" encoding="UTF-8"?>
    <resource
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns="http://datacite.org/schema/kernel-4" xsi:schemaLocation="http://datacite.org/schema/kernel-4 http://schema.datacite.org/meta/kernel-4.4/metadata.xsd">
      <identifier identifierType="DOI">10.21384/ExampleBookChapter</identifier>
      <creators>
        <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
        </creator>
      </creators>
      <titles>
        <title xml:lang="en">Example Chapter Title</title>
      </titles>
      <publisher xml:lang="en">Example Publisher</publisher>
      <publicationYear>1980</publicationYear>
      <resourceType resourceTypeGeneral="BookChapter"></resourceType>
      <relatedItems>
        <relatedItem relationType="IsPublishedIn" relatedItemType="Book">
          <titles>
            <title>Example Book Title</title>
          </titles>
          <publicationYear>1980</publicationYear>
          <volume>I</volume>
          <firstPage>110</firstPage>
          <lastPage>155</lastPage>
          <publisher>Example Publisher</publisher>
          <edition>2nd edition</edition>
          <contributors>
            <contributor contributorType="Editor">
              <contributorName nameType="Personal">Miller, Elizabeth</contributorName>
            </contributor>
          </contributors>
        </relatedItem>
      </relatedItems>
    </resource>
  
  .. code:: json

    {
      "data": {
          "type": "dois",
          "attributes": {
              "url": "https://example.org/RelatedItem3",
              "prefix": "10.21384/ExampleBookChapter",
              "creators": [
                  {
                      "name": "Garcia, Sofia",
                      "nameType": "Personal",
                      "givenName": "Sofia",
                      "familyName": "Garcia"
                  }
              ],
              "titles": [
                  {
                      "lang": "en",
                      "title": "Example Chapter Title"
                  }
              ],
              "publisher": "Example Publisher",
              "publicationYear": 1980,
              "types": {
                  "resourceTypeGeneral": "BookChapter"
              },
              "relatedItems": [
                  {
                      "titles": [
                          {
                              "title": "Example Book Title"
                          }
                      ],
                      "volume": "I",
                      "edition": "2nd edition",
                      "creators": [],
                      "lastPage": "155",
                      "firstPage": "110",
                      "publisher": "Example Publisher",
                      "contributors": [
                          {
                              "name": "Miller, Elizabeth",
                              "nameType": "Personal",
                              "givenName": "Elizabeth",
                              "familyName": "Miller",
                              "affiliation": [],
                              "contributorType": "Editor",
                              "nameIdentifiers": []
                          }
                      ],
                      "relationType": "IsPublishedIn",
                      "publicationYear": "1980",
                      "relatedItemType": "Book"
                  }
              ]
          }
      }
    }




Example: Digitized book chapter in a book (with an ISBN)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. tab-set-code::

  .. code:: xml

    <?xml version="1.0" encoding="UTF-8"?>
    <resource
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns="http://datacite.org/schema/kernel-4" xsi:schemaLocation="http://datacite.org/schema/kernel-4 http://schema.datacite.org/meta/kernel-4.4/metadata.xsd">
      <identifier identifierType="DOI">10.21384/ExampleBookChapter</identifier>
      <creators>
        <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
        </creator>
      </creators>
      <titles>
        <title xml:lang="en">Example Chapter Title</title>
      </titles>
      <publisher xml:lang="en">Example Publisher</publisher>
      <publicationYear>2016</publicationYear>
      <resourceType resourceTypeGeneral="BookChapter"></resourceType>
      <relatedIdentifiers>
        <relatedIdentifier relatedIdentifierType="ISBN" relationType="IsPublishedIn">0-12-345678-1</relatedIdentifier>
      </relatedIdentifiers>
      <relatedItems>
        <relatedItem relationType="IsPublishedIn" relatedItemType="Book">
          <relatedItemIdentifier relatedItemIdentifierType="ISBN">0-12-345678-1</relatedItemIdentifier>
          <creators>
            <creator>
              <creatorName nameType="Personal">Garcia, Sofia</creatorName>
              <givenName>Sofia</givenName>
              <familyName>Garcia</familyName>
            </creator>
          </creators>
          <titles>
            <title>Example Book Title</title>
          </titles>
          <publicationYear>2016</publicationYear>
          <number numberType="Chapter">4</number>
          <firstPage>45</firstPage>
          <lastPage>63</lastPage>
          <publisher>Example Publisher</publisher>
        </relatedItem>
      </relatedItems>
    </resource>

  .. code:: json

    {
      "data": {
          "type": "dois",
          "attributes": {
              "url": "https://example.org/RelatedItem3",
              "prefix": "10.21384/ExampleBookChapter",
              "creators": [
                  {
                      "name": "Garcia, Sofia",
                      "nameType": "Personal",
                      "givenName": "Sofia",
                      "familyName": "Garcia"
                  }
              ],
              "titles": [
                  {
                      "lang": "en",
                      "title": "Example Chapter Title"
                  }
              ],
              "publisher": "Example Publisher",
              "publicationYear": 2016,
              "types": {
                  "resourceTypeGeneral": "BookChapter"
              },
              "relatedIdentifiers": [
                  {
                      "relationType": "IsPublishedIn",
                      "relatedIdentifier": "0-12-345678-1",
                      "relatedIdentifierType": "ISBN"
                  }
              ],
              "relatedItems": [
                  {
                      "number": "4",
                      "titles": [
                          {
                              "title": "Example Book Title"
                          }
                      ],
                      "creators": [
                          {
                              "name": "Garcia, Sofia",
                              "nameType": "Personal",
                              "givenName": "Sofia",
                              "familyName": "Garcia"
                          }
                      ],
                      "lastPage": "63",
                      "firstPage": "45",
                      "publisher": "Example Publisher",
                      "numberType": "Chapter",
                      "relationType": "IsPublishedIn",
                      "publicationYear": "2016",
                      "relatedItemType": "Book",
                      "relatedItemIdentifier": {
                          "relatedItemIdentifier": "0-12-345678-1",
                          "relatedItemIdentifierType": "ISBN"
                      }
                  }
              ]
          }
      }
   }


Use case: Describing related resources
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The related item property can also be used to describe other types of relations between the resource being registered and related resources.


Describing related resources without identifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When a related resource does not have an identifier, the related item property can be used on its own.

.. code:: xml

  <relatedItems>
    <relatedItem relationType="References" relatedItemType="Dissertation">
      <creators>
        <creator>
          <creatorName nameType="Personal">Miller, Elizabeth</creatorName>
          <givenName>Elizabeth</givenName>
          <familyName>Miller</familyName>
        </creator>
      </creators>
      <titles>
        <title>Example Dissertation Title</title>
      </titles>
      <publicationYear>1960</publicationYear>
      <publisher>Example University</publisher>
    </relatedItem>
  </relatedItems>


Describing related resources with identifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Most related resources will have at least one of the identifier types specified in :doc:`/appendices/appendix_1/relatedIdentifierType`.

In this case, the :ref:`12` property is strongly recommended for indexing. In addition, the :ref:`20` property *may* be used to provide additional information about the related item.

.. code:: xml

  <relatedIdentifiers>
    <relatedIdentifier relationType="IsCitedBy" relatedIdentifierType="DOI" resourceTypeGeneral="JournalArticle">10.21384/ExampleJournalArticle</relatedIdentifier>
  </relatedIdentifiers>
  <relatedItems>
    <relatedItem relationType="IsCitedBy" relatedItemType="JournalArticle">
      <relatedItemIdentifier relatedItemIdentifierType="DOI">10.21384/ExampleJournalArticle</relatedItemIdentifier>
      <creators>
        <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
        </creator>
      </creators>
      <titles>
        <title>Example Article Title</title>
      </titles>
      <publicationYear>2021</publicationYear>
      <publisher>Example Publisher</publisher>
    </relatedItem>
  </relatedItems>
