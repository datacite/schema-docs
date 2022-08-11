Citation
=====================================

Because many users of this schema are members of a variety of academic disciplines, DataCite remains
discipline-agnostic concerning matters pertaining to academic style sheet requirements. Therefore,
DataCite encourages rather than requires a particular citation format [#f1]_. In keeping with this approach, the
following is the *preferred* format for rendering a DataCite citation for human readers using the
mandatory properties of the schema:

   Creator (PublicationYear): Title. Publisher. (resourceTypeGeneral). Identifier

It may also be desirable to include information from optional properties, such as Version. This is
particularly important to include when citing software. For example:

   Creator (PublicationYear): Title. Version. Publisher. (resourceTypeGeneral). Identifier

For citation purposes, DataCite prefers that DOI names are displayed as linkable, permanent URLs, for
example, “https://doi.org/10.1038/sdata.2016.18”; however, the Identifier may appear in its original
format. If the original format is chosen, be sure to include the characters “doi:" prepended to the
Identifier as in “doi:10.1038/sdata.2016.18.”

For resources that do not have a standard publication year value, DataCite recommends that
PublicationYear should include the date that is preferred for use in a citation.

Here are several examples:

* Irino, T; Tada, R (2009): Chemical and mineral compositions of sediments from ODP Site 127-797. V. 2.1. Geological Institute, University of Tokyo. (dataset). https://doi.org/10.1594/PANGAEA.726855
* Geofon operator (2009): GEFON event gfz2009kciu (NW Balkan Region). GeoForschungsZentrum Potsdam (GFZ). (dataset). https://doi.org/10.1594/GFZ.GEOFON.gfz2009kciu
* Denhard, Michael (2009): dphase_mpeps: MicroPEPS LAF-Ensemble run by DWD for the MAP DPHASE project. World Data Center for Climate. (dataset.) https://doi.org/10.1594/WDCC/dphase_mpeps


.. rubric:: Footnotes

.. [#f1] In collaboration with CrossRef, DataCite has created a DOI Citation Formatter Service available at https://citation.crosscite.org/. The user can choose from more than 500 different citation formats in 45 different languages.
