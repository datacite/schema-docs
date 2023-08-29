DataCite to Dublin Core Mapping 4.5
========================================

These mappings can be used to convert records described following version 4.5 of the DataCite Metadata Schema into records that comply with the Dublin Core Metadata Initiative Schema.

.. toctree::
  :titlesonly:

  dublincore-qualified
  dublincore-local

The first mapping in :ref:`Table 4` can be used to convert records described following version 4.5 of the DataCite Metadata Schema into records that comply with the Dublin Core Metadata Initiative Schema.

The second mapping in :ref:`Table 5` provides an example of a local DataCite Dublin Core extension.

Both mappings make use of the "pid" attribute from the proposed `Scholarly Resources Application Profile (SRAP) <https://github.com/dcmi/dc-srap/blob/main/profile/srap-profile.md>`_. [#f1]_

.. [#f1] From the `Dublin Core Metadata Initiative Scholarly Resources Application Profile (SRAP) <https://github.com/dcmi/dc-srap/blob/main/profile/srap-profile.md>`_ proposal:  "We do not propose any new properties for agent-specific identifiers, but rely on  `DCMI’s draft proposal <https://github.com/dcmi/pids_in_dc>`_ of using the XML ``id`` attribute to match identifiers with the agent names.  However, we use attribute ``pid`` instead of ``id``, since W3C ``xml:id`` proposal allows just one identifier per each element. In SRAP context, the same person or organization may have multiple unique identifiers."

