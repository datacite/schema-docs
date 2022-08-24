descriptionType
=====================================

*Used by:*

* :ref:`17.a`

*Options:*

.. contents:: :local:


Abstract
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** A brief description of the resource and the context in which the resource was created.

**Usage Notes:** *Recommended for discovery.* Use "<br>" to indicate a line break for improved rendering of multiple paragraphs, but otherwise no html markup.

Example: https://data.datacite.org/application/vnd.datacite.datacite+xml/10.1594/PANGAEA.771774


Methods
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** The methodology employed for the study or research.

**Usage Notes:** *Recommended for discovery.* Full documentation about methods supports open science.

Example: https://data.datacite.org/application/vnd.datacite.datacite+xml/10.6078/D1K01X

.. _SeriesInformation:

SeriesInformation
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Information about a repeating series, such as volume, issue, number.

**Usage Notes:** The information previously encoded as a description with this type should now be explicitly provided in tagged fields using the new :doc:`/properties/recommended_optional/property_relateditem` property with relationType "IsPublishedIn" selected.


TableOfContents
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** A listing of the Table of Contents.

**Usage Notes:** Use "<br>" to indicate a line break for improved rendering of multiple paragraphs, but otherwise no html markup.

Example: https://data.datacite.org/application/vnd.datacite.datacite+xml/10.5678/LCRS/FOR816.CIT.1031

.. _TechnicalInfo:

TechnicalInfo
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Detailed information that may be associated with design, implementation, operation, use, and/or maintenance of a process, system, or instrument.

**Usage Notes:** For software description, this may include the contents of a “readme.txt” and necessary environmental information (hardware, operational software, applications/programs with version information, a human-readable synopsis of software purpose) that cannot be described using other properties (e.g., programming language). For other uses, this can include specific and detailed information as necessary and appropriate. The information entered will be unstructured and not parsed, so it may be useful to format the information using tags and/or line breaks.



Other
~~~~~~~~~~~~~~~~~~~~~~~~~

**Definition:** Other description information that does not fit into an existing category.

**Usage Notes:** Use for any other description type.
