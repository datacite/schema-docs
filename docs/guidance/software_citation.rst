Support for software citation
================================================================================

This page provides a quick reference guide for all the 4.1 version changes in support of software citation.

Documentation updates
~~~~~~~~~~~~~~~~~~~~~~~

*Properties:*

.. contents:: :local:


Identifier
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add: "For software, a decision may need to be made about whether the ID is for a specific version of a piece of software (recommended by Force11 Software Citation Principles), *for a piece of software i.e. all versions or for the latest version.*"

Title
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add:"May be the title of a dataset or the name of a piece of software."


Publisher
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add: "For software, use Publisher for Code Repository, following the data model. If there is an alternate entity that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the contributorType "hostingInstitution" for the code repository."


Contributor
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add: "For software, if there is an alternate entity that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the contributorType "hostingInstitution" for the code repository."


PublicationYear
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add: "In the case of resources such as software where there may be multiple releases in one year, other DataCite metadata or information such as the landing page should enable users to identify the newest one."


resourceTypeGeneral
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** New definition for Service: "An organized system of apparatus, appliances, staff, etc., for supplying some function(s) required by end users."

New example language for Service: "Data management service, *or long-term preservation service.*"

New definition for Software: "A computer program in source code (text) or compiled form. *Use this type for all software components supporting scholarly research.*"

New example language for Software: "Software supporting *scholarly* research."


relationType
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Changes to Example and Usage Notes in the relationType Appendix:

IsPartOf and HasPart: may be used for individual software modules; note that code repository-to-*version* relationships should be modeled using IsVersionOf and HasVersion

IsDocumentedBy and Documents: e.g. points to software documentation

IsVariantFormOf and IsOriginalFormOf: May be used for different software operating systems or compiler formats, for example.


Version
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add to Example: "Software engineering practice follows this approach of tracking changes and giving new version numbers."


Rights
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Add: "May be used for software licenses."


Description
^^^^^^^^^^^^^^^^^^^^^^^^

**Change to the documentation:** Change definition of TechnicalInfo: "For software description, this may include a readme.txt, and necessary environmental *information (hardware, operational software, applications/programs with version information, a human-readable synopsis of software purpose) that cannot be described using other properties (e.g. Language (software))*. For other uses, this can include specific and detailed information as necessary and appropriate."



Changes to the schema
~~~~~~~~~~~~~~~~~~~~~~~
* new relationType pair (HasVersion, IsVersionOf)

  * HasVersion The registered resource such as a software package or code repository has a versioned instance (indicates A has the instance B) e.g. it may be used to relate an un-versioned code repository to one of its specific software versions.
  * IsVersionOf The registered resource is an instance of a target resource (indicates that A is an instance of B) e.g. it may be used to relate a specific version of a software package to its software code repository.
* New relationType pair (IsRequiredBy, Requires)

  * The registered resource such as a software package (A) is required by an identified external resource (B). This may be used to indicate software dependencies.
  * The registered resource such as a software package (A) requires an identified external resource (B). This may be used to indicate software dependencies.
