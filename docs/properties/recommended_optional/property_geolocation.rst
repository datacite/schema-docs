.. _18:

18. GeoLocation
====================

**Obligation:** Recommended

**Occurrences:** 0-n

**Definition:** Spatial region or named place where the data was gathered or about which the data is focused.

**Allowed values, examples, other constraints:**

Repeat this property to indicate several different locations.

*Sub-properties:*

.. contents:: :local:

.. rubric:: Example XML

.. code:: xml

  <geoLocations>
    <geoLocation>
      <geoLocationPlace>Disko Bay</geoLocationPlace>
      <geoLocationPoint>
        <pointLongitude>-52.000000</pointLongitude>
        <pointLatitude>69.000000</pointLatitude>
      </geoLocationPoint>
    </geoLocation>
    <geoLocation>
      <geoLocationBox>
        <westBoundLongitude>-123.27</westBoundLongitude>
        <eastBoundLongitude>-123.225</eastBoundLongitude>
        <southBoundLatitude>49.24</southBoundLatitude>
        <northBoundLatitude>49.28</northBoundLatitude>
      </geoLocationBox>
    </geoLocation>
  </geoLocations>


.. _18.1:

18.1 geoLocationPoint
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** A point location in space.

**Allowed values, examples, other constraints:**

A point contains a single longitude-latitude pair.

Use WGS 84 (World Geodetic System) coordinates and use only decimal numbers for coordinates.

.. _18.1.1:

18.1.1 pointLongitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Longitudinal dimension of point.

**Allowed values, examples, other constraints:**

If geoLocationPoint is used, pointLongitude is mandatory. Longitude of the geographic point expressed in decimal degrees (positive east).

Example: -67.302

Domain: -180 <= pointLongitude <= 180

.. _18.1.2:

18.1.2 pointLatitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Latitudinal dimension of point.

**Allowed values, examples, other constraints:**

If geoLocationPoint is used, pointLatitude is mandatory.

Latitude of the geographic point expressed in decimal degrees (positive north)

Example: 31.233

Domain: -90 <= pointLatitude <= 90

.. _18.2:

18.2 geoLocationBox
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** The spatial limits of a box.

**Allowed values, examples, other constraints:**

A box is defined by two geographic points. Left low corner and right upper corner. Each point is defined by its longitude and latitude.

Use WGS 84 (World Geodetic System) coordinates and use only decimal numbers for coordinates.

.. _18.2.1:

18.2.1 westBoundLongitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Western longitudinal dimension of box.

**Allowed values, examples, other constraints:**

If geoLocationBox is used, westBoundLongitude is mandatory. Longitude of the geographic point expressed in decimal degrees (positive east).

Domain: -180.00 ≤ westBoundLongitude ≤ 180.00

.. _18.2.2:

18.2.2 eastBoundLongitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Eastern longitudinal dimension of box.

**Allowed values, examples, other constraints:**

If geoLocationBox is used, eastBoundLongitude is mandatory. Longitude of the geographic point expressed in decimal degrees (positive east).

Domain: -180.00 ≤ eastBoundLongitude ≤ 180.00

.. _18.2.3:

18.2.3 southBoundLatitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Southern latitudinal dimension of box.

**Allowed values, examples, other constraints:**

If geoLocationBox is used, southBoundLatitude is mandatory. Latitude of the geographic point expressed in decimal degrees (positive north).

Domain: -90.00 ≤ southBoundingLatitude ≤ 90.00

.. _18.2.4:

18.2.4 northBoundLatitude
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 1

**Definition:** Northern latitudinal dimension of box.

**Allowed values, examples, other constraints:**

If geoLocationBox is used, northBoundLatitude is mandatory. Latitude of the geographic point expressed in decimal degrees (positive north).

Domain: -90.00 ≤ northBoundingLatitude ≤ 90.00

.. _18.3:

18.3 geoLocationPlace
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-1

**Definition:** Description of a geographic location.

**Allowed values, examples, other constraints:**

Free text. Use to describe a geographic location.

.. _18.4:

18.4 geoLocationPolygon
~~~~~~~~~~~~~~~~~~~~~~~~~

**Occurrences:** 0-n

**Definition:** A drawn polygon area, defined by a set of points and lines connecting the points in a closed chain.

**Allowed values, examples, other constraints:**

A polygon is delimited by geographic points. Each point is defined by a longitude-latitude pair. The last point should be the same as the first point.

Use WGS 84 (World Geodetic System) coordinates and use only decimal numbers for coordinates.

.. _18.4.1:

18.4.1 polygonPoint
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 4-n

**Definition:** A point location in a polygon.

**Allowed values, examples, other constraints:**

If geoLocationPolygon is used, polygonPoint must be used as well. There must be at least 4 non-aligned points to make a closed curve, with the last point described the same as the first point.

.. _18.4.1.1:

18.4.1.1 pointLongitude
##########################

**Occurrences:** 1

**Definition:** Longitudinal dimension of point.

**Allowed values, examples, other constraints:**

If polygonPoint is used, pointLongitude is mandatory. Longitude of the geographic point expressed in decimal degrees (positive east).

Domain: -180 <= pointLongitude <= 180

.. _18.4.1.2:

18.4.1.2 pointLatitude
##########################

**Occurrences:** 1

**Definition:** Latitudinal dimension of point.

**Allowed values, examples, other constraints:**

If polygonPoint is used, pointLatitude is mandatory. Latitude of the geographic point expressed in decimal degrees (positive north).

Domain: -90 <= pointLatitude <= 90

.. _18.4.2:

18.4.2 inPolygonPoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Occurrences:** 0-1

**Definition:** For any bound area that is larger than half the earth, define a (random) point inside. [#f1]_

**Allowed values, examples, other constraints:**

inPolygonPoint is only necessary to indicate the "inside" of the polygon if the polygon is larger than half the earth. Otherwise the smallest of the two areas bounded by the polygon will be used.

.. _18.4.2.1:

18.4.2.1 pointLongitude
##########################

**Occurrences:** 1

**Definition:** Longitudinal dimension of point.

**Allowed values, examples, other constraints:**

If inPolygonPoint is used, pointLongitude is mandatory. Longitude of the geographic point expressed in decimal degrees (positive east).

.. _18.4.2.2:

18.4.2.2 pointLatitude
##########################

**Occurrences:** 1

**Definition:** Latitudinal dimension of point.

**Allowed values, examples, other constraints:**

If inPolygonPoint is used, pointLatitude is mandatory. Latitude of the geographic point expressed in decimal degrees (positive north).



.. rubric:: Footnotes
.. [#f1] A polygon that crosses the anti-meridian (i.e. the 180th meridian) can be represented by cutting it into two polygons such that neither crosses the anti-meridian.
