PIDINST Schema [#f1]_ Mapping
=================================================================

.. _Table 7:

Table 7: PIDINST to DataCite Mapping
------------------------------------------------------

.. list-table::
   :header-rows: 1
   :widths: auto
   :class: longtable
   :name: Table 6: PIDINST to DataCite Mapping

   * - PIDINST Property
     - DataCite v. 4.5
     - Comments
   * - **Identifier**
     - :ref:`1`
     -
   * - identifierType
     - :ref:`1.a` "DOI"
     -
   * - **Name**
     - :ref:`3`
     - May be the title of a dataset, the name of a piece of software or instrument.
   * - **Owner**
     - | :ref:`7` with :ref:`7.a`:
       | :ref:`HostingInstitution`
     - Can be used for the owner of an instrument, i.e. the institution responsible for the management of the instrument. This may include the legal owner, the operator, or an institute providing access to the instrument. Use the contributorType “hostingInstitution”. The instrument owner may also be included in :ref:`4`. [#f2]_
   * - ownerName
     - :ref:`7.1`
     -
   * - ownerIdentifier
     - :ref:`7.4`
     -
   * - ownerIdentifierType
     - :ref:`7.4.a`
     -
   * - **Manufacturer**
     - :ref:`2`
     - The instrument's manufacturer(s) or developer. This may also be the owner for custom-build instruments.
   * - manufacturerName
     - :ref:`2.1`
     -
   * - manufacturerIdentifier
     - :ref:`2.4`
     -
   * - manufacturerIdentifierType
     - :ref:`2.4.a`
     -
   * - | **Model**
       | modelName
       | modelIdentifier
       | modelIdentifierType
     - | :ref:`17` with :ref:`17.a`:
       | :ref:`TechnicalInfo`
     - Detailed information associated with an instrument instance, e.g. model (model name and model identifier), instrument type (name and identifier), or measured variable.
   * - **Description**
     - | :ref:`17` with :ref:`17.a`:
       | :ref:`Abstract`
     - Technical description of the device and its capabilities.
   * - | **InstrumentType**
       | instrumentTypeName
       | instrumentTypeIdentifier
       | instrumentTypeIdentifierType
     - | :ref:`17` with :ref:`17.a`:
       | :ref:`TechnicalInfo`
     -
   * - **MeasuredVariable**
     - | :ref:`17` with :ref:`17.a`:
       | :ref:`TechnicalInfo`
     - The variable(s) that this instrument measures or observes.
   * - **Date**
     - :ref:`8`
     - Dates relevant to the instrument.
   * - dateType
     - :ref:`8.a`
     - To indicate the date when the instrument started to be in operation (Commissioned), or ceased to be in operation (DeCommissioned), use :ref:`8.a` "Other" and add "Commissioned" resp. "Decommissioned" in :ref:`8.b`.
   * - **RelatedIdentifier**
     - :ref:`12`
     -
   * - relatedIdentifierType
     - :ref:`12.a`
     -
   * - relationType
     - :ref:`12.b`
     - RelationTypes applicable to instruments.
   * -
     - :ref:`Describes`, :ref:`IsDescribedBy`
     -  The linked resource is a document describing the instrument.
   * -
     - :ref:`IsNewVersionOf`, :ref:`IsPreviousVersionOf`
     - If an instrument is substantially modified, a new DOI may be attributed to the new version. In that case the old and the new DOI should be linked to each other. IsNewVersionOf should be used in the new DOI record to link the old instrument before the modification.
   * -
     - :ref:`HasPart`, :ref:`IsPartOf`
     - In the case of a complex instrument, having multiple components that may be considered as instruments in their own right, with their own DOIs, these DOIs should be linked. HasPart should be used in the DOI record of the compound instrument to link the components. IsPartOf should be used in the DOI records of the components to link the compound instrument.
   * -
     - :ref:`HasMetadata`, :ref:`IsMetadataFor`
     - If there is additional metadata describing the instrument, possibly using a community specific metadata standard, that metadata record may be linked using HasMetadata.
   * -
     - :ref:`Collects`, :ref:`IsCollectedBy`
     - If the instrument has been used to collect data (e.g., to measure a physical quantity in some research activity), Collects may be used to link the instrument to the resulting dataset.
   * - **AlternateIdentifier**
     - :ref:`11`
     - May be used for the instrument's serial number. Other possible uses include an owner's inventory number or an entry in some instrument database.
   * - alternateIdentifierType
     - :ref:`11.a`
     - The type of the AlternateIdentifier.

.. rubric:: Footnotes
.. [#f1] Krahl, R., Darroch, L., Huber, R., Devaraju, A., Klump, J., Habermann, T., Stocker, M., & The Research Data Alliance Persistent Identification of Instruments Working Group members (2022). Metadata Schema for the Persistent Identification of Instruments (1.0). Research Data Alliance. https://doi.org/10.15497/RDA00070
.. [#f2] The :doc:`/appendices/appendix_3` values may also be used for :ref:`4` (e.g., ``:unap`` for not applicable).
