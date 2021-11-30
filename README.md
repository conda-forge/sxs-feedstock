About sxs
=========

Home: https://github.com/sxs-collaboration/sxs

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/sxs-feedstock/blob/master/LICENSE.txt)

Summary: A collection of python code used by the SXS collaboration

Development: https://github.com/sxs-collaboration/sxs

This package provides a number of utilities for use by the SXS collaboration, and others who use our data.
For example, the `metadata` subpackage provides functions for reading and analyzing the metadata files
provided with SXS simulations for describing the physics they represent.  Another important subpackage is
`zenodo`, which provides handy functions for interacting with zenodo.org in general, and in particular our
collection of simulation data on that site.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=7193&branchName=master">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/sxs-feedstock?branchName=master">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=7193&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/sxs-feedstock?branchName=master&jobName=linux&configuration=linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=7193&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/sxs-feedstock?branchName=master&jobName=osx&configuration=osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=7193&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/sxs-feedstock?branchName=master&jobName=win&configuration=win_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-sxs-green.svg)](https://anaconda.org/conda-forge/sxs) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/sxs.svg)](https://anaconda.org/conda-forge/sxs) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sxs.svg)](https://anaconda.org/conda-forge/sxs) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/sxs.svg)](https://anaconda.org/conda-forge/sxs) |
| [![Conda Recipe](https://img.shields.io/badge/recipe-sxs--ecosystem-green.svg)](https://anaconda.org/conda-forge/sxs-ecosystem) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/sxs-ecosystem.svg)](https://anaconda.org/conda-forge/sxs-ecosystem) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/sxs-ecosystem.svg)](https://anaconda.org/conda-forge/sxs-ecosystem) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/sxs-ecosystem.svg)](https://anaconda.org/conda-forge/sxs-ecosystem) |

Installing sxs
==============

Installing `sxs` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `sxs, sxs-ecosystem` can be installed with:

```
conda install sxs sxs-ecosystem
```

It is possible to list all of the versions of `sxs` available on your platform with:

```
conda search sxs --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating sxs-feedstock
======================

If you would like to improve the sxs recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/sxs-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@moble](https://github.com/moble/)

