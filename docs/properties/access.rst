.. _22:

22. Access
====================

**Obligation:** Optional

**Occurrences:** 0-1

**Definition:** Access information relevant to the resource as a whole.

**Allowed values, examples, other constraints:**

Include information on how to access the resource, including any restrictions on access.

To describe access conditions for specific content URLs, use :ref:`21.1.c` (part of :ref:`21`).

To provide copyright or licensing information, use the :ref:`16` property. To provide an embargo date, use the :ref:`8` property with dateType :ref:`Available`.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none

.. rubric:: Example

.. tabs::

   .. code-tab:: xml

        <access accessType="Restricted">Available to researchers at XYZ institution</access>
   
   .. code-tab:: json

      "access": {
        "accessType": "Restricted"
        "access": "Available to researchers at XYZ institution"
      }



.. _22.a:

22.a accessType
~~~~~~~~~~~~~~~~~~~

**Occurrences:** 1

**Definition:** The type of access for which the resource is available.

**Allowed values, examples, other constraints:** 

If Access is used, accessType is mandatory.

*Controlled List Values:*

 * :ref:`public`
 * :ref:`restricted`

See :doc:`Appendix 1: Controlled List Definitions - accessType </appendices/appendix-1/accessType>` for definitions.