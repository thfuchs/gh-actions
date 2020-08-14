# GH Action Workflow Templates for CI

Currently these workflows serve R repos only!

The following workflows are served for every R-related package (standardized):
- R CMD Check  
    - `R-CMD-Production`: to check whether package might be installed in production environment  
        The Environment is served by Docker Container `cfgo/gh-actions:base` for every shiny-related repo/package (and cfgo/Docker:API for any plumber API related repo/package)  
    - `R-CMD-Windows`: to check on windows machines for several R-versions (currently R 3.6 and R 4.0) - could be enhanced to also check for MacOS
- lintr to suggest linting changes
- covr to calculate and report (in HTML) overall testing and example coverage of the package

For more information on GitHub Action Workflows for R, see the [r-lib/actions](https://github.com/r-lib/actions) repo
