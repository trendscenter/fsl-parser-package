# fsl-parser-package

This package includes fsl_parser, that parses the freesurfer files (specified in inputspec.json) as dependencies and returns the covariates (X) and dependent (y) matrices as dataframes. A sample inputspec.json can be found in tests. 
# How to install
pip install fslparser
# How to run
import fslparser \
from fslparser import parsers \
args = json.loads(sys.stdin.read())
(X, y) = parsers.fsl_parser(args) 
