.. _3:

3. Title
====================

**Obligation:** Mandatory

**Occurrences:** 1-n

**Definition:** A name or title by which a resource is known. May be the title of a dataset or the name of a piece of software or an instrument.

**Allowed values, examples, other constraints:**

Free text.

*Sub-properties:*

.. contents:: :local:
    :backlinks: none

.. rubric:: Example XML

.. code:: xml

  <titles>
      <title xml:lang="en">Example title</title>
      <title xml:lang="en" titleType="Subtitle">Example subtitle</title>
  </titles>

.. _3.a:

3.a titleType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The type of Title (other than the Main Title).

**Allowed values, examples, other constraints:**

*Controlled List Values:*

* AlternativeTitle
* Subtitle
* TranslatedTitle
* Other

The titleType subproperty is used when more than a single title is provided. Unless otherwise indicated by titleType, a title is considered to be the main title.
