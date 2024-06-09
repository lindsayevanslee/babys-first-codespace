# babys-first-codespace

First foray into GitHub Codespaces

[This YouTube video](https://www.youtube.com/watch?v%253DYDfZ5raWbs4) got me started 

Initialized with a blank template and then manually copied from `src/datascience-py-r` folder of [Data Science with Python and R](https://github.com/microsoft/datascience-py-r/tree/main) codespace by Microsoft.

Added `requirements.txt` to specify additional python packages to install (following pattern shown in `postCreateCommand` specification in `devcontainer.json`)

Can add more R packages via `apt-packages` but seems like there aren't many CRAN packages there:
https://stackoverflow.com/questions/2170043/r-apt-get-install-r-cran-foo-vs-install-packagesfoo
https://packages.ubuntu.com/

Tried to then add r-packages feature but couldn't get it to work: https://github.com/rocker-org/devcontainer-features/tree/main/src/r-packages

Next tried using [`rocker/tidyverse`](https://rocker-project.org/images/) image as a base instead, based on this blog post: https://www.kleinbutsignificant.com/post/2024-01-17-using-github-codespaces-for-quarto-development/