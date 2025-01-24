# docs.mint.sh

Updates mint.json documentation file for mintlify

## Overview

Updates or creates navigation entries in mint.json file for mintlify documentation.
Copies markdown files to documentation directory and maintains navigation structure.

## Index

* [dsh:docs:mint](#dshdocsmint)

## docs

### dsh:docs:mint

Updates or creates navigation entries in mint.json file for mintlify documentation.
Copies markdown files to documentation directory and maintains navigation structure.

#### Example

```bash
dsh:docs:mint "README.md"
dsh:docs:mint "CONTRIBUTING.md" "/custom/path/mint.json" "docs/"
```

#### Arguments

* **$1** (markdown): Path to markdown file to add to documentation
* **$2** (mintFile): [Optional] Path to mint.json file (defaults to ../../docs/yellowteam.cloud/mint.json)
* **$3** (mindFileHrefPrefix): [Optional] Prefix for navigation href (defaults to "projects/${DSH_CLI["name"]}/")

#### Exit codes

* **0**: If successful
* **1**: If markdown file not found
* **2**: If default mint.json not found
* **3**: If failed to initialize navigation array
* **4**: If failed to add group
* **5**: If failed to add page to group

#### See also

* [dsh:log](#dshlog)

