DataCite Metadata Schema Documentation for the Publication and Citation of Research Data and Other Research Outputs
============================================================================================================================================

.. note::

   This is a **draft** proposal for version 4.5 of the DataCite Metadata Schema. The `proposal <https://docs.google.com/document/d/1UyQQwtjnu-4_4zXE4TFZ74-mjLZI3NkEf8RrF0WeOdI/edit?usp=sharing>`_ was open for public comment through October 31, 2022.

   The most recent schema release (4.4) is available at: https://schema.datacite.org/

.. note::

  DataCite Metadata Working Group; (2023): DataCite Metadata Schema for the Publication and Citation of Research Data and Other Research Output v4.5; DataCite e.V. https://doi.org/10.14454/g8e5-6293

Contributors from the DataCite Metadata Working Group:

.. |Jan Ashton| raw:: html

   <a class="orcid" href="https://orcid.org/0000-0003-4676-5263"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Jan Ashton</a>

.. |Isabel Bernal| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0003-2506-9947"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Isabel Bernal</a>

.. |Felix Burger| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0001-6836-1193"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Felix Burger</a>

.. |Madeleine de Smaele| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0002-8963-3415"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Madeleine de Smaele</a>

.. |Samantha Foulger| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0003-2551-6399"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Samantha Foulger</a>

.. |Vanessa Gabriel| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0002-2058-5160"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Vanessa Gabriel</a>

.. |Ted Habermann| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0003-3585-6733"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Ted Habermann</a>

.. |Joseph Padfield| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0002-2572-6428"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Joseph Padfield</a>

.. |Sarah Ramdeen| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0003-1135-5942"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Sarah Ramdeen</a>

.. |Anne Raugh| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0002-8300-9443"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Anne Raugh</a>

.. |Wendy Robertson| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0002-3368-5080"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Wendy Robertson</a>

.. |Mike Shallcross| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0001-6289-5717"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Mike Shallcross</a>

.. |Mohamed Yahia| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0001-7829-1918"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Mohamed Yahia</a>

.. |Kelly Stathis| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0001-6133-4045"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Kelly Stathis</a>

.. |Kristian Garza| raw:: html

  <a class="orcid" href="https://orcid.org/0000-0003-3484-6875"><img alt="ORCID logo" src="https://info.orcid.org/wp-content/uploads/2019/11/orcid_16x16.png"/>Kristian Garza</a>

.. |British Library| raw:: html

   <a class="affiliation" href="https://ror.org/05dhe8b71"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>British Library</a>

.. |Spanish National Research Council (CSIC)| raw:: html

   <a class="affiliation" href="https://ror.org/02gfc7t72"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>Spanish National Research Council (CSIC)</a>

.. |TIB| raw:: html

   <a class="affiliation" href="https://ror.org/04aj4c181"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>TIB</a>

.. |TU Delft Library| raw:: html

   <a class="affiliation" href="https://ror.org/02e2c7k09"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>TU Delft Library</a>

.. |ETH Zurich| raw:: html

  <a class="affiliation" href="https://ror.org/05a28rw58"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>ETH Zurich</a>

.. |University Library of the LMU Munich| raw:: html

  <a class="affiliation" href="https://ror.org/05591te55"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>University Library of the LMU Munich</a>

.. |Metadata Game Changers| raw:: html

  <a class="affiliation" href="https://ror.org/05bp8ka05"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>Metadata Game Changers</a>

.. |The National Gallery| raw:: html

  <a class="affiliation" href="https://ror.org/043kfff89"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>The National Gallery</a>

.. |Columbia University| raw:: html

  <a class="affiliation" href="https://ror.org/00hj8s172"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>Columbia University</a>

.. |University of Maryland| raw:: html

  <a class="affiliation" href="https://ror.org/047s2c258"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>University of Maryland</a>

.. |University of Iowa| raw:: html

  <a class="affiliation" href="https://ror.org/036jqmy94"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>University of Iowa</a>

.. |Inter-university Consortium for Political and Social Research| raw:: html

  <a class="affiliation" href="https://ror.org/02q7mkh03"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>Inter-university Consortium for Political and Social Research</a>

.. |INIST-CNRS| raw:: html

  <a class="affiliation" href="https://ror.org/02mn0vt57"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>INIST-CNRS</a>

.. |DataCite| raw:: html

  <a class="affiliation" href="https://ror.org/04wxnsj81"><img alt="ROR logo" src="https://raw.githubusercontent.com/ror-community/ror-logos/main/ror-icon-rgb.svg"/>DataCite</a>

.. only:: not latex

  * |Jan Ashton|, |British Library| (co-chair of working group)
  * |Isabel Bernal|, |Spanish National Research Council (CSIC)| (co-chair of working group)
  * |Felix Burger|, |TIB|
  * |Madeleine de Smaele|, |TU Delft Library|
  * |Samantha Foulger|, |ETH Zurich|
  * |Vanessa Gabriel|, |University Library of the LMU Munich|
  * |Ted Habermann|, |Metadata Game Changers|
  * |Joseph Padfield|, |The National Gallery|
  * |Sarah Ramdeen|, |Columbia University|
  * |Anne Raugh|, |University of Maryland|
  * |Wendy Robertson|, |University of Iowa|
  * |Mike Shallcross|, |Inter-university Consortium for Political and Social Research|
  * |Mohamed Yahia|, |INIST-CNRS|
  * |Kelly Stathis|, |DataCite|
  * |Kristian Garza|, |DataCite|

.. only:: latex

  * Jan Ashton, British Library (co-chair of working group)
  * Isabel Bernal, Spanish National Research Council (CSIC) (co-chair of working group)
  * Felix Burger, TIB
  * Madeleine de Smaele, TU Delft Library
  * Samantha Foulger, ETH Zurich
  * Vanessa Gabriel, University Library of the LMU Munich
  * Ted Habermann, Metadata Game Changers
  * Joseph Padfield, The National Gallery
  * Sarah Ramdeen, Columbia University
  * Anne Raugh, University of Maryland
  * Wendy Robertson, University of Iowa
  * Mike Shallcross, Inter-university Consortium for Political and Social Research
  * Mohamed Yahia, INIST-CNRS
  * Kelly Stathis, DataCite
  * Kristian Garza, DataCite


Contents
-----------

.. toctree::
   :titlesonly:

   introduction/index
   properties/index
   appendices/index
   mappings/index
   guidance/index
   xml
