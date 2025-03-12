Schema and Examples
=====================================

XML Schema
--------------------------------

The XML Schema is available here:
https://schema.datacite.org/meta/kernel-4.6/metadata.xsd


JSON Representation
--------------------------------

The `DataCite XML to JSON Mapping <https://support.datacite.org/docs/datacite-xml-to-json-mapping>`_  is available on the DataCite Support site.


Examples
------------------------


Demonstration Examples
~~~~~~~~~~~~~~~~~~~~~~~~

.. tabs::

   .. tab:: XML

        * `Full DataCite metadata example (all properties) <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-full-v4.xml>`_
        * `Dataset resourceTypeGeneral <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-dataset-v4.xml>`_
        * `Award resourceTypeGeneral <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-award-v4.xml>`_
        * `Project resourceTypeGeneral <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-project-v4.xml>`_
        * `Coverage dateType <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-coverage-v4.xml>`_
        * Connecting a translation to the original work: 

            * `Translation <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-translation-translated-v4.xml>`_
            * `Original (translated) work <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-translation-original-v4.xml>`_
        * `Document containing two languages in parallel <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-parallel-languages-v4.xml>`_
        * `Multilingual metadata <http://schema.datacite.org/meta/kernel-4.6/example/datacite-example-multilingual-v4.xml>`_

        * RelatedItem:

            * `Journal article in a journal (with an ISSN) <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem1-v4.xml>`_
            * `Digitized book chapter in a book (with no identifier) <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem2-v4.xml>`_
            * `Digitized book chapter in a book (with an ISBN) <https://schema.datacite.org/meta/kernel-4.6/example/datacite-example-relateditem3-v4.xml>`_


   .. tab:: JSON

        * `Full DataCite metadata example (all properties) <https://api.test.datacite.org/dois/10.82433/B09Z-4K37?publisher=true&affiliation=true>`_
        * `Dataset resourceTypeGeneral <https://api.test.datacite.org/dois/10.82433/9184-DY35?publisher=true&affiliation=true>`_
        * `Award resourceTypeGeneral <https://api.test.datacite.org/dois/10.82433/p1zt-4c67?publisher=true&affiliation=true>`_
        * `Project resourceTypeGeneral <https://api.test.datacite.org/dois/10.82433/84dj-am41?publisher=true&affiliation=true>`_
        * `Coverage dateType <https://api.test.datacite.org/dois/10.82433/pgk2-ar97?publisher=true&affiliation=true>`_
        * Connecting a translation to the original work: 

            * `Translation <https://api.test.datacite.org/dois/10.82433/45e5-xy14?publisher=true&affiliation=true>`_
            * `Original (translated) work <https://api.test.datacite.org/dois/10.82433/pma6-nf93?publisher=true&affiliation=true>`_
        * `Document containing two languages in parallel <https://api.test.datacite.org/dois/10.82433/4r08-sa38?publisher=true&affiliation=true>`_
        * `Multilingual metadata <https://api.test.datacite.org/dois/10.82433/byt7-2g42?publisher=true&affiliation=true>`_

        * RelatedItem:

            * `Journal article in a journal (with an ISSN) <https://api.test.datacite.org/dois/10.82433/q54d-pf76?publisher=true&affiliation=true>`_
            * `Digitized book chapter in a book (with no identifier) <https://api.test.datacite.org/dois/10.82433/eck0-f231?publisher=true&affiliation=true>`_
            * `Digitized book chapter in a book (with an ISBN) <https://api.test.datacite.org/dois/10.82433/4fdh-rh04?publisher=true&affiliation=true>`_




Live Examples
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. note::

    Because these live examples link to real DOIs, the metadata may change.

.. tabs::

   .. tab:: XML

        * `Software resourceTypeGeneral <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5281/zenodo.7635478>`_
        * `GeoLocation <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.1594/PANGAEA.770250>`_
        * `(GeoLocation) Polygon <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.15129/3da7087a-91a3-40be-9a83-7e412156db59>`_
        * `HasMetadata as related resource <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.26164/leopoldina_10_00390>`_
        * `IsIdenticalTo as related resource <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5282/oph.2>`_
        * `Contributor <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.4228/zalf.sy6a-xt12>`_
        * `Workflow resourceTypeGeneral  <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.48546/WORKFLOWHUB.WORKFLOW.412.1>`_
        * `FundingReference <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5281/zenodo.47394>`_
        * Blog post published simultaneously in two languages:

            * `Blog post in Spanish <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5438/S7C0-Y897>`_
            * `Blog post in English <https://api.datacite.org/dois/application/vnd.datacite.datacite+xml/10.5438/1HG2-BF13>`_


   .. tab:: JSON

        * `Software resourceTypeGeneral <https://api.datacite.org/dois/10.5281/zenodo.7635478?publisher=true&affiliation=true>`_
        * `GeoLocation <https://api.datacite.org/dois/10.1594/PANGAEA.770250?publisher=true&affiliation=true>`_
        * `(GeoLocation) Polygon <https://schema.datacite.orgttps://api.datacite.org/dois/10.15129/3da7087a-91a3-40be-9a83-7e412156db59?publisher=true&affiliation=true>`_
        * `HasMetadata as related resource <https://api.datacite.org/dois/10.26164/leopoldina_10_00390?publisher=true&affiliation=true>`_
        * `IsIdenticalTo as related resource <https://api.datacite.org/dois/10.5282/oph.2?publisher=true&affiliation=true>`_
        * `Contributor <https://api.datacite.org/dois/10.4228/zalf.sy6a-xt12?publisher=true&affiliation=true>`_
        * `Workflow resourceTypeGeneral <https://schema.datacitettps://api.datacite.org/dois/10.48546/WORKFLOWHUB.WORKFLOW.412.1?publisher=true&affiliation=true>`_
        * `FundingReference <https://api.datacite.org/dois/10.5281/zenodo.47394?publisher=true&affiliation=true>`_
        * Blog post published simultaneously in two languages:

            * `Blog post in Spanish <https://api.datacite.org/dois/10.5438/S7C0-Y897?publisher=true&affiliation=true>`_
            * `Blog post in English  <https://api.datacite.org/dois/10.5438/1HG2-BF13?publisher=true&affiliation=true>`_
       


