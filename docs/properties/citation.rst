Citation
=====================================

Because many users of this schema are members of a variety of academic disciplines, DataCite remains
discipline-agnostic concerning matters pertaining to academic style sheet requirements. Therefore,
DataCite encourages rather than requires a particular citation format [5]_. In keeping with this approach, the
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


*A special note regarding citation of dynamic datasets:*

For datasets that are continuously and rapidly updated, there are special challenges both in citation and
preservation. For citation, four approaches are possible:

a) Cite a specific slice [6]_ or subset (the set of updates to the dataset made during a particular period of time or to a particular area of the dataset); Example:

  Data Request T.Jansen; SAHFOS; Work published 2014 via SAHFOS ; Area Def: 54-65°N, 0-45°W. Temporal Def: 1980-2012 (April-August) Taxonomic Def: All zooplankton; (dataset). https://doi.org/10.7487/2014.15.1.1

b) Cite a specific snap-shot (a copy of the entire dataset made at a specific time; Example:

  König-Langlo, G., & Sieger, R. (2010). BSRN snapshot 2010-01 as ISO image file (3.75 GB) [Data set]. PANGAEA - Data Publisher for Earth & Environmental Science. (dataset). https://doi.org/10.1594/pangaea.833424

c) Cite the continuously updated dataset6 but add an Access Date and Time to the citation. Example:

  Doe, J. and R. Roe. 2001. The FOO Data Set. Version 2.3. The FOO Data Center. (dataset). https://doi.org/10.xxxx/notfoo.547983. Accessed 1 May 2011.

d) Cite a query [7]_, time-stamped for re-execution against a versioned database. The RDA recommended citation for this approach is:

  R. Roe. 2017. "The Moo Data Query" created at 2017-07-21 10:25:30 PID https://doi.org/10.xxxx/notmoo.857988. Subset of Moo Database (dataset). PID https://doi.org/10.xxxx/bigmoo.360873.

Notes:
  The “slice,” “snap‐shot” and "query" options require unique identifiers. Be aware that the third
  option (c) necessarily means that following the citation does not result in access to the resource
  as cited. This limits reproducibility of the work that uses this form of citation.
  In addition, please note that access date and time may be combined with the first (a), second (b)
  and fourth (d) options, but it must be used with the third option (c).

  The fourth option (d) may shift more work onto repositories to store database versions for all
  the queries, so not all repositories will be able to support this alternative.


.. rubric:: Footnotes

.. [5] In collaboration with CrossRef, DataCite has created a DOI Citation Formatter Service available at https://citation.crosscite.org/. The user can choose from more than 500 different citation formats in 45 different languages.
.. [6] Ball, A. & Duke, M. (2015, July 30). ‘How to Cite Datasets and Link to Publications’. DCC How-to Guides. Edinburgh : Digital Curation Centre. Retrieved April 13, 2017, from: http://www.dcc.ac.uk/resources/how-guides/cite- datasets#sec:versions
.. [7] Rauber, A., Uytvanck, D. V., Asmi, A., & Proll, S. (2016, February 09). Identification of Reproducible Subsets for Data Citation, Sharing and Re-Use. Retrieved April 13, 2017, from https://www.rd- alliance.org/system/files/documents/TCDL-RDA-Guidelines_160411.pdf
