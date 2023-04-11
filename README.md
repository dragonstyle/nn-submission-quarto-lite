# Notebooks Now! Submission Template

This submission template is for a simple notebook-based publication with one source file, supporting data, bibliography, and MyST build configuration.

## Source file

The source file for this template is a Jupyter notebook. There is not necessarily anything special about this notebook. It may contain markdown cells, code cells, and outputs from common Python packages, including pandas, matplotlib, plotly, and altair. Specific markdown cells may be tagged in their metadata as `"part": "abstract"`, or `"part": "availability"` - these cells will be extracted from the document and included as the specified part in the built output.

## Supporting material

### Notebook data

By convention, all data should be saved in `data/` directory. There is nothing magic about this directory; references to your data from your notebook must still specify the correct relative path.

### Bibliography

The bibliography must be specified in bibtex format, by convention as `references.bib`.

## MyST configuration

A `myst.yml` file must be provided to configure notebook metadata and exports.

## Building output artfiacts

To build PDF/JATS output from your source data, you must have the MyST CLI installed

```
npm install myst-cli
```

Then build all exports defined in the `myst.yml` file:

```
myst build --all
```
