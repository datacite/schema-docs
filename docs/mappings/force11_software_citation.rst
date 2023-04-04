FORCE11 Software Citation Principles [#f1]_ Mapping
=================================================================

*FORCE11 requirements:*

.. contents:: :local:

.. _Table 6:

Table 6: FORCE11 Software Citation Principles to DataCite Mapping
------------------------------------------------------------------

.. list-table::
   :header-rows: 1
   :widths: auto
   :class: longtable
   :name: Table 5: FORCE11 Software Citation Principles to DataCite Mapping

   * - FORCE11 requirement
     - DataCite v. 4.1
     - Comments
   * - Unique identifier – recommend a DOI
     - :ref:`1` with :ref:`1.a` "DOI"
     - For software a decision may need to be made about whether the ID is for a specific version of a piece of software (recommended by FORCE11 Software Citation Principles), for a piece of software (i.e. all versions), or for the latest version.
   * - Software name
     - :ref:`3`
     - May be the title of a dataset or the name of a piece of software.
   * - Author
     - :ref:`2`
     - May include those responsible for software creation.
   * - Contributor
     - :ref:`7`
     - For software, if there is an alternate entity that “holds, archives, publishes, prints, distributes, releases, issues, or produces the code, use the :ref:`7.a` :ref:`HostingInstitution` for the code repository.
   * - Contributor role
     - :ref:`7.a`
     - | See Definition in :doc:`contributorType Appendix </appendices/appendix_1/contributorType>`:
       | :ref:`Distributor`: Includes distribution of software.
       | See Example for :ref:`HostingInstitution`: Includes software or run code repositories.
   * - Version number
     - :ref:`15`
     - See Version example: Software engineering practice follows this approach of tracking changes and giving new version numbers.
   * - Release date
     - :ref:`5`
     - See definition: In the case of resources such as software where there may be multiple releases in one year, other DataCite metadata or information such as the landing page should enable users to identify the newest one.
   * - Location/repository
     - | :ref:`4`
       | :ref:`7` with :ref:`7.a` :ref:`HostingInstitution`
     - For software, use :ref:`4` for Code Repository, following the data model. If there is an alternate entity that "holds, archives, publishes, prints, distributes, releases, issues, or produces" the code, use the :ref:`7.a` :ref:`HostingInstitution` for the code repository."
   * - Indexed citations (and links between software versions)
     - :ref:`12` with :ref:`12.b`
     - RelationTypes applicable to software.
   * -
     - :ref:`HasVersion`, :ref:`IsVersionOf`
     - | :ref:`HasVersion`: The registered resource such as a software package or code repository has a versioned instance (indicates A has the instance B). It may, e.g., be used to relate an un- versioned code repository to one of its specific software versions.
       | :ref:`IsVersionOf`: The registered resource is an instance of a target resource (indicates that A is an instance of B). It may, e.g., be used to relate a specific version of a software package to its software code repository.
   * -
     - :ref:`IsNewVersionOf`, :ref:`IsPreviousVersionOf`
     - | :ref:`IsNewVersionOf`: Can be used for “edition or software release etc.”
       | :ref:`IsPreviousVersionOf`: Can be used for “edition or software release etc.”
   * -
     - :ref:`IsDerivedFrom`, :ref:`IsSourceOf`
     - :ref:`IsDerivedFrom` and :ref:`IsSourceOf`: Can be used to denote software that is a fork of other software or is the origin of a fork.
   * -
     - :ref:`IsPartOf`, :ref:`HasPart`
     - :ref:`IsPartOf` and :ref:`HasPart`: May be used for individual software modules.
   * -
     - :ref:`IsDocumentedBy`, :ref:`Documents`
     - :ref:`IsDocumentedBy` and :ref:`Documents`: Points to software documentation.
   * -
     - :ref:`IsVariantFormOf`, :ref:`IsOriginalFormOf`
     - :ref:`IsVariantFormOf` and :ref:`IsOriginalFormOf`: May be used for different software operating systems or compiler formats, for example. Indicates that A is a variant or different form or packaging of B.
   * -
     - :ref:`IsRequiredBy`, :ref:`Requires`
     - | :ref:`IsRequiredBy`: The registered resource A is called by or is required by software resource B.
       | :ref:`Requires`: The registered resource A calls or requires software resource B.
   * - Software licenses
     - :ref:`16`
     - See example: May be used for software licenses.
   * - Description
     - | :ref:`17`
       | :ref:`17` with :ref:`17.a`: :ref:`TechnicalInfo`
       | :ref:`17` with :ref:`17.a`: :ref:`Abstract`
     - :ref:`TechnicalInfo`: For software description, this may include a readme.text, and necessary environmental information (hardware, operational software, applications/programs) that cannot be described using other properties such as ‘Format/version’ or ‘Description/summary’.
   * - Keywords
     - :ref:`6`
     - Existing guidance applies: Subject, keyword, classification code, or key phrase describing the resource.


.. rubric:: Footnotes
.. [#f1] Smith AM, Katz DS, Niemeyer KE, FORCE11 Software Citation Working Group. (2016) Software citation principles. PeerJ Computer Science 2:e86 https://doi.org/10.7717/peerj-cs.86
