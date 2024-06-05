# Structured information service: preliminary notes

```{abstract}
Preliminary design notes for an information architecture for publishing source-of-truth documentation snippets, metadata and other structured "factoids" via an API for consumption, inter alia, by a Datalink service. This document is to support largely internal discussions in the Data Services teams.

Everything, including package names, is subject to change.
```

## Usecase

The primary usecase is to serve, via an API, single source-of-truth structured documentation snippets to RSP services. For example, a portal user and a notebook user should be presented with the same canonical rich description of the LSST U-band filter.

The secondary usecase is to build documents that are at least partially generated from these source of truth snippets. An example would be to build a document with all the column descriptions in the source catalog.

The third usecase is to provide partial or complete technical consolidation with other structured data retrieval services. Examples of these would be: checkerboard (github->slack lookup), glossary, authorDB, contactsDB. Note: these examples are given as an indication of capability. None of these services will be forcibly changed or retired and certainly without permission of their developers. An example we don't have: asking a service (eg via squarebot) backed by a citation cff store for the canonical reference for a package (the portal, gafalefawr) and getting back a URL to that citation, and/or a bibtex code etc.




