.. _19:

19. FundingReference
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Information about financial support (funding) for the resource being registered.

**Allowed values, examples, other constraints:**

It is a best practice to supply funding information when financial support has been received.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none

.. rubric:: Example

.. tabs::

   .. code-tab:: xml

      <fundingReferences>
        <fundingReference>
          <funderName>European Commission</funderName>
          <funderIdentifier funderIdentifierType="ROR">https://ror.org/00k4n6c32</funderIdentifier>
          <awardNumber awardURI="https://cordis.europa.eu/project/rcn/100180_en.html">282625</awardNumber>
          <awardTitle>MOTivational strength of ecosystem services and alternative ways to express the value of BIOdiversity</awardTitle>
          </fundingReference>
        <fundingReference>
          <funderName>Therapeutic Innovation Australia</funderName>
          <funderIdentifier funderIdentifierType="ROR">https://ror.org/01rde0531</funderIdentifier>
          <awardNumber awardURI="https://doi.org/10.82292/hbrw-rw97"></awardNumber>
          <awardTitle>Products for Cartilage and Bone Repair using Human Induced Pluripotent Stem Cell-Derived Organoids and Decellularized Organoid Scaffolds</awardTitle>
        </fundingReference>
      </fundingReferences>
   
   .. code-tab:: json

      "fundingReferences": [
        {
          "awardUri": "https://cordis.europa.eu/project/rcn/100180_en.html",
          "awardTitle": "MOTivational strength of ecosystem services and alternative ways to express the value of BIOdiversity",
          "funderName": "European Commission",
          "awardNumber": "282625",
          "funderIdentifier": "https://ror.org/00k4n6c32",
          "funderIdentifierType": "ROR"
        },
        {
          "awardUri": "https://doi.org/10.82292/hbrw-rw97",
          "awardTitle": "Products for Cartilage and Bone Repair using Human Induced Pluripotent Stem Cell-Derived Organoids and Decellularized Organoid Scaffolds",
          "funderName": "Therapeutic Innovation Australia",
          "funderIdentifier": "https://ror.org/01rde0531",
          "funderIdentifierType": "ROR"
        }
      ]



.. _19.1:

19.1 funderName
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** Name of the funding provider.

**Allowed values, examples, other constraints:**

If FundingReference is used, then funderName is mandatory.

Example: Gordon and Betty Moore Foundation

.. _19.2:

19.2 funderIdentifier
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Uniquely identifies a funding entity, according to various types.

**Allowed values, examples, other constraints:**

Example: https://ror.org/00k4n6c32

.. _19.2.a:

19.2.a funderIdentifierType
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** The type of the funderIdentifier.

**Allowed values, examples, other constraints:**

If funderIdentifier is used, funderIdentifierType is mandatory.

*Controlled List Values:*

* ROR
* Crossref Funder ID [#f1]_
* GRID [#f2]_
* ISNI
* Other

.. _19.2.b:

19.2.b schemeURI
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** The URI of the funder identifier scheme.

**Allowed values, examples, other constraints:**

Examples:

* https://ror.org/
* https://www.crossref.org/services/funder-registry/

.. _19.3:

19.3 awardNumber
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The code assigned by the funder to a sponsored award (grant).

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

**Definition:** The human readable title or name of the award (grant).

**Allowed values, examples, other constraints:**

Example: Socioenvironmental Monitoring of the Amazon Basin and Xingu



.. rubric:: Footnotes
.. [#f1] Crossref Funder IDs and the Open Funder Registry are being replaced by ROR. See: https://ror.readme.io/docs/funder-registry
.. [#f2] GRID is no longer openly available and recommends use of ROR. See: https://ror.readme.io/docs/grid