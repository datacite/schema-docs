.. _15:

15. Version
====================

**Obligation:** Optional

**Occurrences:** 0-1

**Definition:** The version number of the resource.

**Allowed values, examples, other constraints:**

Suggested practice: track major_version.minor_version. Register a new identifier for a major version change. Individual stewards need to determine which are major vs. minor versions [#f1]_.

Software engineering practice follows this approach of tracking changes and giving new version numbers.

May be used in conjunction with properties :ref:`11` and :ref:`12` to indicate various information updates. May be used in conjunction with property :ref:`17` to indicate the nature and file/record range of version.

.. rubric:: Example XML

.. code:: xml

  <version>2.1</version>


.. rubric:: Footnotes
.. [#f1] Based on the work of the Earth Science Information Partners (ESIP). For more guidance, see: http://wiki.esipfed.org/index.php/Interagency_Data_Stewardship/Citations/provider_guidelines#Note_on_Versioning_and_Locators
