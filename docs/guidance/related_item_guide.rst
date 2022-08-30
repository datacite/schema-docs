Using RelatedItem for publication information and related resources
================================================================================

The :doc:`/properties/recommended_optional/property_relateditem` property was developed to satisfy two distinct use cases.

The first use case is **providing publication information** for journal articles, book chapters, and other resources that are published within another item. This information about the related item (the container) is needed to formulate a complete citation of the primary resource being described. For example, a book title is necessary to cite a book chapter, and a journal title and volume/issue number are necessary to cite a journal article.

The second use case is **providing information about related resources.**

- When a related resource *does not have an identifier*, the :doc:`/properties/recommended_optional/property_relateditem` property should be used to provide information about the related resource.
- When a related resource *has an identifier*, the :doc:`/properties/recommended_optional/property_relatedidentifier` property should *always* be used. In addition, the :doc:`/properties/recommended_optional/property_relateditem` property may *optionally* be used to provide information about the related resource.

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

The related item that the resource is published in may have an identifier of this own. When the related item has an identifier, it may be included in the :ref:`20.1` attribute. In addition, the :doc:`/properties/recommended_optional/property_relatedidentifier` property should also be supplied.

Example: Journal article in a journal (with an ISSN)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: xml

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
    <title xml:lang="en-US">Example Article Title/title>
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


Example: Digitized book chapter in a book (with no identifier)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: xml

  <identifier identifierType="DOI">10.21384/ExampleBookChapter</identifier>
  <creators>
    <creator>
      <creatorName nameType="Personal"></creatorName>
      <givenName>Sofia</givenName>
      <familyName>Garcia</familyName>
      </creatorName>
    </creator>
  </creators>
  <titles>
    <title xml:lang="en-US">Example Chapter Title/title>
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
      <edition>2nd edition</edition>
      <publisher>Example Publisher</publisher>
    </relatedItem>
  </relatedItems>

Example: Digitized book chapter in a book (with an ISBN)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code:: xml

  <identifier identifierType="DOI">10.21384/ExampleBookChapter</identifier>
  <creators>
    <creator>
      <creatorName nameType="Personal">Garcia, Sofia</creatorName>
      <givenName>Sofia</givenName>
      <familyName>Garcia</familyName>
    </creator>
  </creators>
  <titles>
    <title xml:lang="en-US">Example Chapter Title/title>
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
      <titles>
        <title>Example Book Title</title>
      </titles>
      <creators>
        <creator>
          <creatorName nameType="Personal">Garcia, Sofia</creatorName>
          <givenName>Sofia</givenName>
          <familyName>Garcia</familyName>
        </creator>
      </creators>
      <publicationYear>2016</publicationYear>
      <number numberType="Chapter">4</number>
      <firstPage>45</firstPage>
      <lastPage>63</lastPage>
      <publisher>Example Publisher</publisher>
    </relatedItem>
  </relatedItems>


Use case: Describing related resources
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The related item property can also be used to describe other types of relations between the resource being registered and related resources.


Describing related resources without identifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When a related resource does not have an identifier, the related item property can be used on its own.

.. code:: xml

  <relatedItems>
    <relatedItem relationType="References" relatedItemType="Dissertation">
      <titles>
        <title>Example Dissertation Title</title>
      </titles>
      <creators>
        <creator>
          <creatorName nameType="Personal">Miller, Elizabeth</creatorName>
          <givenName>Elizabeth</givenName>
          <familyName>Miller</familyName>
        </creator>
      </creators>
      <publicationYear>1960</publicationYear>
      <publisher>Example University</publisher>
    </relatedItem>
  </relatedItems>


Describing related resources with identifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Most related resources will have at least one of the identifier types specified in :doc:`/appendices/appendix_1/relatedIdentifierType`.

In this case, the :doc:`/properties/recommended_optional/property_relatedidentifier` property is strongly recommended for indexing. In addition, the :doc:`/properties/recommended_optional/property_relateditem` property *may* be used to provide additional information about the related item.

.. code:: xml

  <relatedIdentifiers>
    <relatedIdentifier relationType="IsCitedBy" relatedIdentifierType="DOI" resourceTypeGeneral="JournalArticle">10.21384/ExampleJournalArticle</relatedIdentifier>
  </relatedIdentifiers>
  <relatedItems>
    <relatedItem relationType="IsCitedBy" relatedItemType="JournalArticle">
      <relatedItemIdentifier relatedItemIdentifierType="DOI">10.21384/ExampleJournalArticle</relatedItemIdentifier>
      <titles>
        <title>Example Article Title</title>
      </titles>
      <creators>
        <creator>
          <creatorName nameType="Personal">Miller, Elizabeth</creatorName>
          <givenName>Elizabeth</givenName>
          <familyName>Miller</familyName>
        </creator>
      </creators>
      <publicationYear>2021</publicationYear>
      <publisher>Example Publisher</publisher>
    </relatedItem>
  </relatedItems>
