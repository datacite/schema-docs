Version 4.4 Update
====================

* Addition of the new subproperty “classificationCode” in the ``Subject`` property.
* Addition of new values to the ``resourceTypeGeneral`` property:

 * Book
 * BookChapter
 * ComputationalNotebook
 * ConferencePaper
 * ConferenceProceeding
 * Dissertation
 * Journal
 * JournalArticle
 * OutputManagementPlan
 * PeerReview
 * Preprint
 * Report
 * Standard

* Addition of a new relationType: “isPublishedIn” (indicates that A is published in B)
* Addition of a new ``relatedItem`` property, with subproperties to contain specific details for containing publication information previously encoded in a ``description`` field with ``descriptionType=”SeriesInformation”`` (for example, to define the journal name, volume, and page number for an article resource). Subproperties:

 * relationType
 * relatedItemType
 * relatedItemIdentifier
 * relatedItemIdentifierType
 * creator
 * title
 * publicationYear
 * volume
 * issue
 * number
 * firstPage
 * lastPage
 * publisher
 * edition
 * contributor

Major Documentation changes:

* The title of this document has changed to: *DataCite Metadata Schema Documentation for the Publication and Citation for Research Data and Other Research Outputs*.
* Following community feedback and suggestions, this version includes further clarification as regards the following contributorTypes: DataManager, DataCurator, ResearchGroup, and HostingInstitution.
