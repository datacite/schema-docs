FORCE11 Software Citation Principles [#f1]_ Mapping
=================================================================

*FORCE11 requirements:*

.. contents:: :local:

Unique identifier – recommend a DOI
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Identifier with identifierType ‘DOI’

**Comments:** For software a decision may need to be made about whether the ID is for a specific version of a piece of software (recommended by Force11 Software Citation Principles), for a piece of software i.e. all versions or for the latest version.


Software name
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Title

**Comments:** May be the title of a dataset or the name of a piece of software.


Author
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Creator

**Comments:** May include those responsible for software creation.


Contributor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Contributor

**Comments:** For software, if there is an alternate entity that “holds, archives, publishes, prints, distributes, releases, issues, or produces the code, use the contributorType “HostingInstitution” for the code repository.


Contributor role
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** contributorType

**Comments:** See Definition in contributorType Appendix: Distributor: Includes distribution of software. See Example for HostingInstitution: Includes software or run code repositories.


Version number
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Version

**Comments:** See Version example: Software engineering practice follows this approach of tracking changes and giving new version numbers.


Release date
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** PublicationYear

**Comments:** See definition: In the case of resources such as software where there may be multiple releases in one year, other DataCite metadata or information such as the landing page should enable users to identify the newest one.


Location/repository
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Publisher or Contributor/contributorType ‘HostingInstitution’

**Comments:** For software, use Publisher for Code Repository, following the data model. If there is an alternate entity that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the contributorType "hostingInstitution" for the code repository."


Indexed citations (and links between software versions)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** relationType +

**Comments:** RelationTypes applicable to software.

* HasVersion, IsVersionOf

   * HasVersion: The registered resource such as a software package or code repository has a versioned instance (indicates A has the instance B). It may, e.g., be used to relate an un- versioned code repository to one of its specific software versions.
   * IsVersionOf: The registered resource is an instance of a target resource (indicates that A is an instance of B). It may, e.g., be used to relate a specific version of a software package to its software code repository
* IsNewVersionOf, IsPreviousVersionOf

   * IsNewVersionOf: Can be used for “edition or software release etc.”
   * IsPreviousVersionOf: Can be used for “edition or software release etc.”
* IsDerivedFrom, IsSourceOf

   * IsDerivedFrom and IsSourceOf: Can be used to denote software that is a fork of other software or is the origin of a fork.
* IsPartOf, HasPart

   * IsPartOf and HasPart: May be used for individual software modules
* IsDocumentedBy, Documents

   * IsDocumentedBy and Documents: Points to software documentation, e.g.
* IsVariantFormOf, IsOriginalFormOf

   * IsVariantFormOf and IsOriginalFormOf: May be used for different software operating systems or compiler formats, for example. Indicates that A is a variant or different form or packaging of B.
* IsRequiredBy, Requires

   * IsRequiredBy: The registered resource A is called by or is required by software resource B.
   * Requires: The registered resource A calls or requires software resource B.


Software licenses
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Rights

**Comments:** See example: May be used for software licenses.


Description
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Description

Description with descriptionType ‘TechnicalInfo’

Description with descriptionType ‘Abstract’

**Comments:** TechnicalInfo: For software description, this may include a readme.text, and necessary environmental information (hardware, operational software, applications/programs) that cannot be described using other properties such as ‘Format/version’ or ‘Description/summary’


Keywords
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**DataCite v 4.1:** Subject

**Comments:** Existing guidance applies: Subject, keyword, classification code, or key phrase describing the resource.



.. rubric:: Footnotes
.. [#f1] Smith AM, Katz DS, Niemeyer KE, FORCE11 Software Citation Working Group. (2016) Software citation principles. PeerJ Computer Science 2:e86 https://doi.org/10.7717/peerj-cs.86
