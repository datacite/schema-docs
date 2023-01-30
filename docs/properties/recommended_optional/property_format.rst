.. _14:

14. Format
====================

**Obligation:** Optional

**Occurrences:** 0-n

**Definition:** Technical format of the resource.

**Allowed values, examples, other constraints:**

Free text.

Use file extension or MIME type where possible, e.g., PDF, XML, MPG or application/pdf, text/xml, video/mpeg.

If :ref:`21` is used, indicating the file format with :ref:`21.1.a` is mandatory.

.. rubric:: Example XML

.. code:: xml

  <formats>
      <format>application/xml</format>
  </formats>
