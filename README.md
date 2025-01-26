# BST 258 Problem Set Template

This is a template repository for problem sets for the Spring 2025 edition of
BST 258 at HSPH. As the course progresses, some of our focus will transition to
applying techniques and tools from statistical causal inference in examples of
data analysis. Doing so in the real world requires proficiency with the tools
necessary to ensure computationally reproducible results are obtained from code
produced to implement a given analysis. At a bare minimum, such tools include

1. *Version control*, e.g., with `git` and collaborative programming platforms
    like GitHub. If you are new to version control, you may find the
    [introductory workshop](https://swcarpentry.github.io/git-novice/)
    developed and maintained by Software/Data Carpentry useful.
2. *Virtual environments*, which help to ensure that the software dependencies
     of a given project remain consistent across potentially different computing
    environments (including, e.g., your own machine later in time). We will use
    the [`renv` package](https://rstudio.github.io/renv/) for the
    [R programming language and environment](https://www.r-project.org/).
3. *Literate programming* notebooks, which help to embed code and results in a
    single plain-text document, ideally in a manner that can be both easily read
    and converted into a variety of formats. We will use
    [`Quarto`](https://quarto.org/), an open-source scientific and technical
    publishing system that extends `R Markdown`.

Note the directory structure of this repository

```{sh}
❯ tree -a -L 2 --noreport
.
├── .Rprofile
├── .git
│   ├── COMMIT_EDITMSG
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── MERGE_RR
│   ├── config
│   ├── description
│   ├── hooks
│   ├── index
│   ├── info
│   ├── logs
│   ├── objects
│   ├── packed-refs
│   ├── refs
│   └── rr-cache
├── .github
│   ├── .gitignore
│   └── workflows
├── .gitignore
├── .here
├── README.md
├── refs.bib
├── renv
│   ├── .gitignore
│   ├── activate.R
│   ├── library
│   ├── settings.json
│   └── staging
├── renv.lock
└── template.qmd
```

The above includes a `renv` subdirectory (and associated `.Rprofile`), a
Quarto file `template.qmd` with corresponding BibTeX database `refs.bib`, and a
few hidden files (like `.here` from the [`here` R
package](https://here.r-lib.org/) and `.gitignore`) and auxiliary directories
(like `.git`). *It is important that you familiarize yourself with these tools,
including their basic anatomy.*

For some perspective on why one might adopt such a setup, consider reading
[this brief piece](https://doi.org/10.1093/biostatistics/kxq028) by David
Donoho.
