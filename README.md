# universe
Setup for R-universe

If you want to change which packages or package versions are listed on our [R-universe site](https://polyploids.r-universe.dev),
please edit the packages.json file.  URLs must point to a Git repository, but it can be on any site (GitHub, GitLab, etc.).
See https://github.com/r-universe-org/demo-registry/blob/master/packages.json for an example.  If your default branch is not
guaranteed to be installable, you can use `branch` to point to a stable branch or release.

Please feel free to add any R packages pertinent to the molecular breeding of polyploid crops.

R-universe is still under development, but there should be more features soon, like the ability to categorize and organize
packages and vignettes.  Everything is pulled from GitHub, so if for example you want to have your picture show up in the
maintainers list, just add the picture to your GitHub profile.

## Diagnosing problems

A couple hours after you add your package to the list, or after you make a commit to your package, you should
see it reflected in the Builds tab of our [R-universe site](https://polyploids.r-universe.dev).  If it's not there or
if any icons are showing up red (especially under the "Src" column), take a look at
[GitHub Actions](https://github.com/r-universe/polyploids/actions) for your package.  If "Build Source Package"
is red, click on it to see the output of `R CMD build`.
