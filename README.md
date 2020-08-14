# GH Action Workflow Templates for CI

Currently these workflows serve R repos only!

The following workflows are served for every R-related package (standardized):
- R CMD Check  
    - `R-CMD-Production`: to check whether package might be installed in production environment  
        The Environment is served by Docker Container `cfgo/gh-actions:base` for every shiny-related repo/package (and cfgo/Docker:API for any plumber API related repo/package)  
    - `R-CMD-Windows`: to check on windows machines for several R-versions (currently R 3.6 and R 4.0) - could be enhanced to also check for MacOS
- lintr to suggest linting changes
- covr to calculate and report (in HTML) overall testing and example coverage of the package

## More information

### In General
- [GH Action Docs](https://help.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions)

### GH Actions for R
- [Intro Video from RStudio Conference 2020](https://www.jimhester.com/talk/2020-rsc-github-actions/)
- [Ropensci GitHub Actions Quick Intro](https://ropenscilabs.github.io/actions_sandbox/)
- [Detailed Intro](https://www.edwardthomson.com/blog/github_actions_advent_calendar.html)

### Examples
- [R-Lib](https://github.com/r-lib/actions/blob/master/examples/README.md)
