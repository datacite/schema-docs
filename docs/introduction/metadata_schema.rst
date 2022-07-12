
The Metadata Schema
=====================================

The DataCite Metadata Schema is a list of core metadata properties chosen for accurate and consistent identification of a resource for citation and retrieval purposes, with recommended use instructions in the documentation. The resource that is being identified can be of any kind, but it is typically a dataset. We use the term ‘dataset’ in its broadest sense. We mean it to include not only numerical data, but any other research objects in keeping with `DataCite’s mission <https://www.datacite.org/mission.html>`_. The metadata schema properties are presented and described in detail in the section `DataCite Metadata Properties <https://www.datacite.org/mission.html>`_ in this document.

While DataCite’s Metadata Schema has been expanded with each new version, it is, nevertheless, intended to be generic to the broadest range of research datasets, rather than customized to the needs of any particular discipline. DataCite metadata primarily supports citation and discovery of data; it is **not** intended to supplant or replace the discipline- or community-specific metadata that fully describes the data and is vital for understanding and reuse.

DataCite clients are strongly encouraged to provide metadata in English whenever possible, in addition to any other language that may be required by the funder or hosting organization. The DataCite Metadata Schema supports language attributes for core properties.

This release of the Metadata Schema contains better support for textual publications. Important changes are the addition of specific resource types such as journal, journal article, dissertation, etc., and also includes computational notebook and peer review, so that these types can be better identified.

Also, a new property, *relatedItem*, is introduced which contains information about a resource related to the one being registered, e.g., a journal article, conference paper, or a book series. It can be used to describe a text citation where relatedIdentifier cannot be used because the related resource does not have an identifier.

The remainder of the Version 4.4 changes are in response to requests from DataCite community members, people like you that have used the metadata schema and have imagined ways in which it might work better for their particular use cases. We are indebted to everyone who has provided us with their feedback, allowing us to improve our service for the broader DataCite community.

For a list of all changes, see :doc:`version_update`.

Lastly, we continue to support openness and the future extensibility of the schema by collaborating with the Dublin Core Metadata Initiative (DCMI) Science and Metadata Community (SAM) [4]_ to maintain a DataCite to Dublin Core crosswalk, available at `DataCite Metadata Schema <https://schema.datacite.org/meta/kernel-4.4/>`_.


.. rubric:: Footnotes

.. [4] For more information on DCMI SAM, see http://www.dublincore.org/groups/sam/
