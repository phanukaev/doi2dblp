# doi2dblp

A simple bash script to automatically retrieve bibtex entries from
[DBLP](https://dblp.org) based on a paper's doi.

## Usage

``` bash
doi2dblp [options...] doi
```


### Parameters

-   **`doi`**
    The digital object identifier for which a bibfile should be retrieved.
    This can be either the raw identifier or a URL.
    The following are valid examples:
    +   10.1145/2783446.2783605
    +   https://doi.org/10.1145/2783446.2783605
    +   dx.doi.org/10.1145/2783446.2783605

### Accepted options

-   **`--help`**
    Display usage information and exit.
-   **`--outfile` FILE, `-o` FILE**
    Append to the specified FILE, rather than printing the retrieved
    bibfile to stdout.
-   **`--standard`**
    Retrieve the standard bibfile. This is the default.
    Overrides any previous `--condensed` or `--crossref` options.
-   **`--condensed`**
    Retrieve the condensed bibfile.
    Overrides any previous `--standard` or `--crossref` options.
-   **`--crossref`**
    Retrieve the bibfile with crossref.
    Overrides any previous `--standard` or `--condensed` options.
