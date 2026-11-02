# BShot-3PAQA

Dataset for the WACV 2027 paper *BShot-3PAQA: Phase-Structured Basketball Shot Quality Assessment Enabled by a Biomechanical Rubric and Annotated Dataset*.

## BShot-3PAQA Dataset

BShot-3PAQA contains 216 three-point jump shots from six public NBA YouTube videos (two highlight compilations, two poor-form sequences and two full game broadcasts). Each shot is split into four phases (Set, Load and Lift, Release, Follow-through) and scored on ten biomechanical items, each rated 0, 1, 2 or unclear. The overall score is the sum of the valid items divided by twice the number of valid items, times 100. Only annotations are released. Clips are given as timestamps into the source videos listed in `sources.csv`.

`annotations/shots.csv` has one row per shot and `annotations/phases.csv` one row per phase segment. `splits/` holds the train, validation and test splits used in the paper (144/28/36), plus the 8 shots removed by crop-confidence filtering.

