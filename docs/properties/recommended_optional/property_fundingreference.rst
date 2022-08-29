19. FundingReference
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Information about financial support (funding) for the resource being registered.

**Allowed values, examples, other constraints:**

It is a best practice to supply funding information when financial support has been received.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <fundingReferences>
    <fundingReference>
      <funderName>European Commission</funderName>
      <funderIdentifier funderIdentifierType="Crossref Funder ID">https://doi.org/10.13039/501100000780</funderIdentifier>
      <awardNumber awardURI="https://cordis.europa.eu/project/rcn/100180_en.html">282625</awardNumber>
      <awardTitle>MOTivational strength of ecosystem services and alternative ways to express the value of BIOdiversity</awardTitle>
      </fundingReference>
    <fundingReference>
      <funderName>European Commission</funderName>
      <funderIdentifier funderIdentifierType="Crossref Funder ID">https://doi.org/10.13039/501100000780</funderIdentifier>
      <awardNumber awardURI="https://cordis.europa.eu/project/rcn/100603_en.html">284382</awardNumber>
      <awardTitle>Institutionalizing global genetic-resource commons. Global Strategies for accessing and using essential public knowledge assets in the life sciences</awardTitle>
    </fundingReference>
  </fundingReferences>

.. _19.1:

19.1 funderName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Name of the funding provider

**Allowed values, examples, other constraints:**

Example: Gordon and Betty Moore Foundation

.. _19.2:

19.2 funderIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Uniquely identifies a funding entity, according to various types.

**Allowed values, examples, other constraints:**

Example: https://doi.org/10.13039/100000936

.. _19.2.a:

19.2.a funderIdentifierType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The type of the funderIdentifier

**Allowed values, examples, other constraints:**

If funderIdentifier is used, funderIdentifierType is mandatory.

*Controlled List Values:*

* Crossref Funder ID [#f1]_
* GRID
* ISNI
* ROR
* Other

.. _19.2.b:

19.2.b schemeURI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the funder identifier scheme

**Allowed values, examples, other constraints:**

Examples:

* https://www.crossref.org/services/funder-registry/
* https://ror.org/

.. _19.3:

19.3 awardNumber
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The code assigned by the funder to a sponsored award (grant)

**Allowed values, examples, other constraints:**

Example: GBMF3859.01

.. _19.3.a:

19.3.a awardURI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI leading to a page provided by the funder for more information about the award (grant).

**Allowed values, examples, other constraints:**

Example: https://www.moore.org/grants/list/GBMF3859.01

Note: In case the award or grant has an ID or DOI, the full URL of the grant DOI can be included here, e.g. https://doi.org/10.35802/221400.

.. _19.4:

19.4 awardTitle
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The human readable title or name of the award (grant)

**Allowed values, examples, other constraints:**

Example: Socioenvironmental Monitoring of the Amazon Basin and Xingu



.. rubric:: Footnotes
.. [#f1] The Crossref service is called “Funder Registry” (https://www.crossref.org/services/funder-registry/) and Crossref Funder ID is the name for a Crossref identifier.
