
<!-- README.md is generated from README.Rmd. Please edit that file -->
<!-- badges: start -->

[![OME](https://img.shields.io/badge/ecosystem-open%20music%20europe-00348A.svg)](https://dataobservatory.eu/)
[![lifecycle](https://lifecycle.r-lib.org/articles/figures/lifecycle-experimental.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![Project Status:
WIP](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10578360.svg)](https://zenodo.org/record/6950435#.YukDAXZBzIU)
<!-- badges: end -->

<br/> <br/> [Open Music Europe](https://openmuse.eu/) will pioneer new
best-practice methods and tools for data collection from multiple
sources, and integrate these into an open-source software ecosystem that
non-specialist stakeholders can use.

<img src="png/Banner_OME_Software_Ecosystem.png" width="90%" style="display: block; margin: auto;" />

*Our ambition is to create an ecosystem of statistical software that is
interoperable with the systems of ESSnet via the widely-used R
statistical environment. On the basis of this ecosystem, we are planning
a complementary, decentralised music data and intelligence hub that is
complementary to both the centralised functions of the future
`European Music Observatory` and the ESSnet. This intelligence hub, the
Open Data Observatory, has a service level similar to that of the
Eurostat Rest API (high-quality data and visualisation products with
various statistical quality control available in a Rest API meeting
Dublin Core, DataCite, and SDMX interoperability standards). In
addition, the Open Data Observatory will fill the gaps in the offering
provided by Eurostat and the ESSnet network,due to their non-music
specific mandate and cost/benefit analysis.*

## Release timeline

- `2023.10.18.`: Polifonia Stakeholder Network workshop; reuse of the
  *Polifonia Ontology Network* and joint requirement elicitation.
  [polifonia-project/stories](https://github.com/polifonia-project/stories).
- `2023.10.24.`: Task description for `rSPARQL-Anything`. GitHub
  repository:
  [antaldaniel/rSPARQL-Anything](https://github.com/antaldaniel/rSPARQL-Anything).
- `2023.11.09`: *Making Datasets Truly Interoperable and Reusable in R*
  (working paper with software code prototypes); DOI:
  [10.5281/zenodo.10091666](https://doi.org/10.5281/zenodo.10091666)
- `2023.12.01.`: The KULT package - case study of retrospective
  harmonisation of KULT 5, 10, 11, 19. Not released (sensitive data
  contents); private GitHub Repo: `dataobservatory-eu/KULT`; an update
  of the *retroharmonize* package to 0.2.5.003.
- `2023.12.17`: The *dataset* 0.2.8 is released on CRAN; supports
  [Dublin
  Core](https://dataset.dataobservatory.eu/articles/dublincore.html),
  [DataCite](https://dataset.dataobservatory.eu/articles/datacite.html)
  and to some extent SDMX and XKOS.
- `2023.12.19.`: The *eurostat* 4.0.0 is released on CRAN to maintain
  usability of the background after API change in the Eurostat data
  warehouse. GitHub repository:
  [rOpenGov/eurostat](https://github.com/rOpenGov/eurostat)
- `2024.01.08.`: A new 0.9.3 release of the *iotables* on CRAN. GitHub
  repository: [rOpenGov/iotables](https://github.com/ropengov/iotables)
  to maintain compatibility with *eurostat*.
- `2024.01.09`: The *dataset* 0.3.0; co-development planning with
  *ontologics* (see [issue
  28](https://github.com/luckinet/ontologics/issues/28)), prototype for
  *tuRtle*.
- `2024.01.28`: The *tuRtle* 0.1.0 is released on GitHub and Zenodo.

## Request new functionality

Because we aim to fill data gaps with an open-source software ecosystem
so that non-technical music researchers can work with them and make them
available in the Open Music Observatory, we embraced and slightly
modified the requirements elicitation methodology of the Polifonia
Horizon Europe project; this way we could also utilise the excellent
formal ontologies and tools developed by this project for music
research.

In short, we ask music stakeholders to tell our experts their data
“story”: what is the data problem or data gap they are struggling with
now, and how they would like to change it. We write a 2-3 pages “story”
about the required software components to be developed in a
non-technical manner.

- `Reproducible culral policy documents`: Requirement elicitation:
  Stories of
  [Michal](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/michal.html),
  [Ivana](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/ivana.html).
- `Connecting music databases and libraries`: Story of
  [Natalia](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/natalia.html).
- `Locally relevant playlists, rights management reporting`: Story of
  [Max](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/max.html);
  [Georg](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/georg.html)
  and
  [Jana](https://music.dataobservatory.eu/documents/open_music_europe/dataset-development/stories/jana.html).

Polifonia uses the *eXtreme Design* methodology complemented with some
user-experience design concepts; this method utilises software design
patterns and competency questions. Using software design patterns is
commonplace in object-oriented languages, and work very well in
OWL/RDF/Python (used in our knowledge coordination layer), but not
always straightforward in functional programming. To retain the
applicability of this methodology across the different layers of our
software ecosystem, the new R packages developed in Open Music Europe
are object-oriented, and they utilise the relatively simple but
versatile S3 object-oriented class system of the R statistical ecosystem
and language.

## Report a problem, issues, bug

- [eurostat](https://github.com/rOpenGov/eurostat/issues/): R tools to
  access open data from Eurostat. Data search, download, manipulation
  and visualization.
- [iotables](https://github.com/rOpenGov/iotables/issues/): Importing
  and Manipulating Symmetric Input-Output Tables (a tool for economic,
  social and environmental impact analysis).
- [retroharmonize](https://github.com/rOpenGov/retroharmonize/issues/):
  Facilitate retrospective (ex-post) harmonization of survey data in a
  reproducible manner.
- [dataset](https://github.com/dataobservatory-eu/dataset/issues):
  Create interoperable and well described data frames in R.
- [statcodelists](https://github.com/antaldaniel/statcodelists/issues):
  Promote the reuse and exchange of statistical information and related
  metadata with making the internationally standardized SDMX code lists
  available for the R use.
- [regions](https://github.com/rOpenGov/regions/issues): Working with
  Sub-national Statistics in R.
- [tuRtle](https://github.com/dataobservatory-eu/tuRtle/issues): Parse
  or export R data with the Turtle syntax for the Resource Description
  Framework (RDF).

## Project background

- `2017.05.10.`: Retrieval and Analysis of Eurostat Open Data with the
  eurostat Package; subsequently maintained and improved through
  2017-2023.
- `2018.01.30.`: The *iotables* R package first released on CRAN, adding
  functionality to *eurostat*.
- `2020.06.04`: The *regions* extension to is first released on CRAN; it
  supports the metadata reconciliation of subnational statistics and
  complements the usability of *eurostat*. It goes through further
  releases till 2021.
- `2020.09.21.`: The first CRAN release of the *retroharmonize* R
  package.
- `2021.06.17.`: The discontinued, orphaned *spotifyr* package is taken
  over by REPREX and re-released on CRAN under version 2.2.1; goes
  through minor changes till 2022. GitHub repository:
  [charlie86/spotifyr](https://github.com/charlie86/spotifyr)
- `2022.06.28`: The *statcodelists* 0.9.2 package is released on CRAN to
  support the further usability of the *retroharmonize* and *dataset*
  packages. GitHub repository:
  [antaldaniel/statcodelists](https://github.com/antaldaniel/statcodelists/),
  product website:
  \[statcodelists\](<https://statcodelists.dataobservatory.eu/>.
- `2022.12.02.` The *dataset* 0.1.9. prototype for inviting
  requirements, future contributors, and users.
- `2023.04.30.`: The *SurveyHarmonies* system for ex-ante survey
  harmonisation.
- `2023.04.30.`: *Eviota*, a minimum viable product for integrated
  financial and sustainability reporting for music SMEs.

## Code of Conduct

Please note that the all our open source components are released with a
[Contributor Code of
Conduct](https://contributor-covenant.org/version/2/1/CODE_OF_CONDUCT.html).
By contributing to this project, you agree to abide by its terms.
