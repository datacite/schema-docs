.. _5:

5. PublicationYear
====================

**Obligation:** Mandatory

**Occurrences:** 1

**Definition:** The year when the data was or will be made publicly available. In the case of resources such as software or dynamic data where there may be multiple releases in one year, include the Date property and sub-properties (dateType/dateInformation) to provide more information about the publication or release date details.

**Allowed values, examples, other constraints:**

YYYY

If an embargo period has been in effect, use the date when the embargo period ends.
In the case of datasets, "publish" is understood to mean making the data available on a specific date to the community of researchers.
If there is no standard publication year value, use the date that would be preferred from a citation perspective.

.. rubric:: Example XML

.. code:: xml

  <publicationYear>2022</publicationYear>

.. rubric:: PublicationYear—Additional guidance

PublicationYear : the year when the data was or will be made publicly available. In the case of datasets, "publish" is understood to mean making the data available on a specific date to the community of researchers.

* If that date cannot be determined, use the date of registration.
* If an embargo period has been in effect, use the date when the embargo period ends.
* If there is no standard publication year value, use the date that would be preferred from a citation perspective.
* In the case of resources such as software or dynamic data where there may be multiple releases in one year, include the Date property and sub-properties (dateType/dateInformation) to provide more information about the publication or release date details.

.. _PublicationYear_digitised_version:

*In the case of a digitised version of a physical object*

If the DOI is being used to identify a digitised version of an original item, the recommended approach is to supply the PublicationYear for the digital version and not the original object.

The :ref:`3` field may be used to convey the approximate or known date of the original object. Other metadata properties available for additional date information about the object include :ref:`6` and :ref:`17`. However, only :ref:`3` will be part of the citation.

Here are two examples of citations using dates or date information in the titles.

  Schmidt, S., Andersen, V., Belviso, S., & Marty, J.-C. (2002). Dissolved and particulate thorium 234 concentration at time series station DYFAMED from date 1995-05-07 (Data set). PANGAEA - Data Publisher for Earth & Environmental Science. https://doi.org/10.1594/pangaea.183607

  Tape, K. D. (2015). Aerial Images of Alaska’s Arctic Coastal Plain; 1948-1949. U.S. Geological Survey. (Image). https://doi.org/10.5066/f79021tb
