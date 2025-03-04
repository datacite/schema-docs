Schema and Examples
=====================================

XML Schema
--------------------------------

The XML Schema is available here:
https://schema.datacite.org/meta/kernel-4.6/metadata.xsd

Examples
------------------------

Demonstration Examples
~~~~~~~~~~~~~~~~~~~~~~~~

* Full DataCite metadata example: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-full-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/B09Z-4K37?publisher=true&affiliation=true>`_
* Example for Dataset resourceTypeGeneral: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-dataset-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/9184-DY35?publisher=true&affiliation=true>`_
* Example for Award resourceTypeGeneral: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-award-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/p1zt-4c6?publisher=true&affiliation=true>`_
* Example for Project resourceTypeGeneral: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-project-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/84dj-am41?publisher=true&affiliation=true>`_
* Example for Coverage dateType: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-coverage-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/pgk2-ar97?publisher=true&affiliation=true>`_
* Example connecting a translation to the original work: 

    * Example of a translation: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-translation-translated-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/45e5-xy14?publisher=true&affiliation=true>`_
    * Example of the original (translated) work: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-translation-original-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/pma6-nf93?publisher=true&affiliation=true>`_
* Example of a document containing two languages in parallel: `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-parallel-languages-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/4r08-sa38?publisher=true&affiliation=true>`_
* Example showing multilingual metadata: `XML <http://schema.datacite.org/meta/kernel-4.6/example/datacite-example-multilingual-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/byt7-2g42?publisher=true&affiliation=true>`_

* Examples with RelatedItem:

    * Journal article in a journal (with an ISSN): `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem1-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/q54d-pf76?publisher=true&affiliation=true>`_
    * Digitized book chapter in a book (with no identifier): `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem2-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/eck0-f231?publisher=true&affiliation=true>`_
    * Digitized book chapter in a book (with an ISBN): `XML <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem3-v4.xml>`_, `JSON <https://api.test.datacite.org/dois/10.82433/4fdh-rh04?publisher=true&affiliation=true>`_

Live Examples
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. note::

    Because these live examples link to real DOIs, the metadata may change.

* Example for Software resourceTypeGeneral: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5281/zenodo.7635478>`_, `JSON <https://api.datacite.org/dois/10.5281/zenodo.7635478?publisher=true&affiliation=true>`_
* Example with GeoLocation: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.1594/PANGAEA.770250>`_, `JSON <https://api.datacite.org/dois/10.1594/PANGAEA.770250?publisher=true&affiliation=true>`_
* Example with (GeoLocation) Polygon: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.15129/3da7087a-91a3-40be-9a83-7e412156db59>`_, `JSON <https://api.datacite.org/dois/10.15129/3da7087a-91a3-40be-9a83-7e412156db59?publisher=true&affiliation=true>`_
* Example with HasMetadata as related resource: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.26164/leopoldina_10_00390>`_, `JSON <https://api.datacite.org/dois/10.26164/leopoldina_10_00390?publisher=true&affiliation=true>`_
* Example with IsIdenticalTo as related resource: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5282/oph.2>`_, `JSON <https://api.datacite.org/dois/10.5282/oph.2?publisher=true&affiliation=true>`_
* Example with Contributor: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.4228/zalf.sy6a-xt12>`_, `JSON <https://api.datacite.org/dois/10.4228/zalf.sy6a-xt12?publisher=true&affiliation=true>`_
* Example for Workflow resourceTypeGeneral : `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.48546/WORKFLOWHUB.WORKFLOW.412.1>`_, `JSON <https://api.datacite.org/dois/10.48546/WORKFLOWHUB.WORKFLOW.412.1?publisher=true&affiliation=true>`_
* Example with FundingReference: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5281/zenodo.47394>`_, `JSON <https://api.datacite.org/dois/10.5281/zenodo.47394?publisher=true&affiliation=true>`_
* Example of a blog post published simultaneously in two languages:

    * Blog post in Spanish: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5438/S7C0-Y897>`_, `JSON <https://api.datacite.org/dois/10.5438/S7C0-Y897?publisher=true&affiliation=true>`_
    * Blog post in English: `XML <https://schema.datacite.org/meta/kernel-4.6/https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5438/1HG2-BF13>`_, `JSON <https://api.datacite.org/dois/10.5438/1HG2-BF13?publisher=true&affiliation=true>`_
