.. _10:

10. ResourceType
====================

**Obligation:** Mandatory

**Occurrences:** 1

**Definition:** A description of the resource.

**Allowed values, examples, other constraints:**

Free text. The recommended content is a single term of some detail so that a pair can be formed with the resourceTypeGeneral sub-property. For example, a resourceType of “Census Data” paired with a resourceTypeGeneral of “Dataset” yields “Dataset/Census Data”.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

 <resourceType resourceTypeGeneral="Dataset">Census Data</resourceType>

.. _10.a:

10.a resourceTypeGeneral
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The general type of a resource.

**Allowed values, examples, other constraints:**

*Controlled List Values:*

* :ref:`Audiovisual`
* :ref:`Book`
* :ref:`BookChapter`
* :ref:`Collection`
* :ref:`ComputationalNotebook`
* :ref:`ConferencePaper`
* :ref:`ConferenceProceeding`
* :ref:`DataPaper`
* :ref:`Dataset`
* :ref:`Dissertation`
* :ref:`Event`
* :ref:`Image`
* :ref:`InteractiveResource`
* :ref:`Instrument`
* :ref:`Journal`
* :ref:`JournalArticle`
* :ref:`Model`
* :ref:`OutputManagementPlan`
* :ref:`PeerReview`
* :ref:`PhysicalObject`
* :ref:`Preprint`
* :ref:`Report`
* :ref:`Service`
* :ref:`Software`
* :ref:`Sound`
* :ref:`Standard`
* :ref:`StudyRegistration`
* :ref:`Text`
* :ref:`Workflow`
* :ref:`resourceTypeGeneral_Other`

See :doc:`Appendix 1: Controlled List Definitions - resourceTypeGeneral </appendices/appendix_1/resourceTypeGeneral>` for definitions and examples.
