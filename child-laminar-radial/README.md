# README.md

These are the R functions needed for the motion coherence psychophysics project. For more information about this project, see our (currently unshared) Databrary volume: <http://databrary.org/volume/218>. We expect to share the dataset once we have submitted the manuscript for review.

- Folders
    - *analyses/data-aggregate/* contains the merged CSV file for all participants across sessions.
    - *analyses/data-participant-metadata/* contains a CSV file with participant-level metadata that is not included in the other data files. **Contains PII and is not shared on GitHub.** Included reference here for completeness. Raw data available (to authorized researchers) at <http://databrary.org/volume/218>.
    - *analyses/data-pilot/* contains block-level data files for participants who were pilots. **Contains PII in the filename and is not shared on GitHub**. Included reference here for completeness. Raw data available (to authorized researchers) at <http://databrary.org/volume/218>.
    - *analyses/data-study-bysession/* contains the block-level data files for participants who were included in the study. **Contains PII in the filename and is not shared on GitHub**. Included reference here for completeness. Raw data available (to authorized researchers) at <http://databrary.org/volume/218>.
    - *analyses/img/* contains plots generated by the analysis functions.
- Core R scripts/functions
    - *analyses/import.clean.export.R* creates the aggregate data file stored in *data-aggregate/* from individual session files. `source("analyses/import.clean.R")` to run.
    - *analyses/plot.aggregate.R* imports the aggregate data file and creates some aggregate plots. `source("analyses/plot.aggregate.R")` to run.
- Reports
    - To generate summary reports `source("render_all.R")` then `render_all()`
    - To inspect the reports, see the files in `html/`.
    - Summary plots of [child](https://rawgit.com/gilmore-lab/moco-3-pattern-psychophysics/master/child-laminar-radial/html/child.html), and [adult](https://rawgit.com/gilmore-lab/moco-3-pattern-psychophysics/master/child-laminar-radial/html/adult.html) data.
    - Modeling of [child](https://rawgit.com/gilmore-lab/moco-3-pattern-psychophysics/master/child-laminar-radial/html/child.models.html) and [adult](https://rawgit.com/gilmore-lab/moco-3-pattern-psychophysics/master/child-laminar-radial/html/adult.models.html) data.