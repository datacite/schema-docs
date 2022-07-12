DataCite Properties
=====================================

:doc:`mandatory/index` provides a detailed description of the mandatory properties, which must be supplied with any
initial metadata submission to DataCite, together with their sub-properties. **If one of the required
properties is unavailable**, please use one of the standard (machine-recognizable) codes listed in
:doc:`/appendices/appendix_3`.

In :doc:`recommended_optional/index`, the Recommended and Optional properties are described in detail. For
an example of how to make a submission in XML format, please see the `XML Examples <https://schema.datacite.org/meta/kernel-4.0/>`_ provided on the
DataCite Metadata Schema [8]_ website.

Throughout this document, a naming convention has been used for all properties and sub-properties as
follows: properties begin with a capital letter, whereas sub-properties begin with a lower case letter. If
the name is a compound of more than one word, subsequent words begin with capital letters. [9]_

“ID” indicates major properties by hierarchical number, and modifiers on those
properties by lowercase letters. In the XML schema, the hierarchical numbers indicate elements of the
schema, while lowercase letters indicate attributes of the related numbered element.

“Occurrence (Occ)” indicates cardinality/quantity constraints for the properties as
follows:

* 0-n = optional and repeatable
* 0-1 = optional, but not repeatable
* 1-n = required and repeatable
* 1 = required, but not repeatable

NOTE:
XML provides an xml:lang attribute [10]_ that can be used on the properties ``Title``, ``Subject``, ``Rights``,
``Description``, and ``RelatedItem Title``, as well as on the properties ``Creator``,
``Contributor`` and ``Publisher`` for organizational names. This provides a way to describe the
language used for the content of the specified properties. The schema provides a ``Language`` property
to be used to describe the language of the resource.

.. toctree::
   mandatory/index
   recommended_optional/index

.. rubric:: Footnotes
.. [8] https://schema.datacite.org/
.. [9] This convention is known as “camelCase.” https://en.wikipedia.org/wiki/CamelCase
.. [10] Allowed values IETF BCP 47, ISO 639-1 language codes, e.g. en, de, fr
