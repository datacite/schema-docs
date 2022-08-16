3. Title
====================

**Occurrences:** 1-n

**Definition:** A name or title by which a resource is known. May be the title of a dataset or the name of a piece of software or instrument.

**Allowed values, examples, other constraints:**

Free text.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

::

  <titles>
      <title xml:lang="en">Example title</title>
      <title xml:lang="en" titleType="Subtitle">Example subtitle</title>
  </titles>

3.a titleType
~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The type of Title (other than the Main Title)

**Allowed values, examples, other constraints:**

*Controlled List Values:*

* AlternativeTitle
* Subtitle
* TranslatedTitle
* Other
