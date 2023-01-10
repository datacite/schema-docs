.. _8:

8. Date
====================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** Different dates relevant to the work.

**Allowed values, examples, other constraints:**

YYYY, YYYY-MM-DD, YYYY- MM-DDThh:mm:ssTZD or any other format or level of granularity described in `W3CDTF <https://www.w3.org/TR/NOTE-datetime>`_. Use `RKMS-ISO8601 <http://www.ukoln.ac.uk/metadata/dcmi/collection-RKMS-ISO8601/>`_ standard for depicting date ranges.

Example: 2004-03-02/2005- 06-02.

Years before 0000 must be prefixed with a - sign, e.g., -0054 to indicate 55 BC.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <dates>
      <date dateType="Issued">2022-08-01</date>
      <date dateType="Other" dateInformation="Conceptualized">2020-01-01</date>
  </dates>

.. _8.a:

8.a dateType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of date.

**Allowed values, examples, other constraints:**

If Date is used, dateType is mandatory.

*Controlled List Values:*

* :ref:`Accepted`
* :ref:`Available`
* :ref:`Copyrighted`
* :ref:`Collected`
* :ref:`Created`
* :ref:`Issued`
* :ref:`Submitted`
* :ref:`Updated`
* :ref:`Valid`
* :ref:`Withdrawn`
* :ref:`dateType_Other`

See :doc:`Appendix 1: Controlled List Definitions - dateType </appendices/appendix_1/dateType>` for definitions and recommendations.

.. _8.b:

8.b dateInformation
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Specific information about the date, if appropriate.

**Allowed values, examples, other constraints:**

Free text.

May be used to provide more information about the publication, release, or collection date details, for example. May also be used to clarify dates in ancient history. Examples: 55 BC, 55 BCE.
