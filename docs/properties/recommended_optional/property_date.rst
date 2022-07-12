8. Date
====================

**Occurrences:** 0-n

**Definition:** Different dates relevant to the work

**Allowed values, examples, other constraints:**

YYYY, YYYY-MM-DD, YYYY- MM-DDThh:mm:ssTZD or any other format or level of granularity described in W3CDTF [22]_. Use RKMS- ISO8601 [23]_ standard for depicting date ranges.

Example: 2004-03-02/2005- 06-02.

Years before 0000 must be prefixed with a - sign, e.g., -0054 to indicate 55 BC.

*Sub-properties:*

.. contents:: :local:


8.a dateType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of date

**Allowed values, examples, other constraints:**

If Date is used, dateType is mandatory.

*Controlled List Values:*

* Accepted
* Available
* Copyrighted
* Collected
* Created
* Issued
* Submitted
* Updated
* Valid
* Withdrawn
* Other

See :doc:`Appendix 1: Controlled List Definitions - dateType </appendices/appendix_1/dateType>` for definitions and recommendations.

8.b dateInformation
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Specific information about the date, if appropriate

**Allowed values, examples, other constraints:**

Free text.

May be used to provide more information about the publication, release, or collection date details, for example. May also be used to clarify dates in ancient history. Examples: 55 BC, 55 BCE.

.. rubric:: Footnotes
.. [22] https://www.w3.org/TR/NOTE-datetime
.. [23] The standard is documented here: http://www.ukoln.ac.uk/metadata/dcmi/collection -RKMS-ISO8601/
