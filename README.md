# awesome-software-supply-chain-security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A compilation of resources in the software supply chain security domain, with emphasis on open source.

## About the categories

There is no prescribed taxonomy for this domain. The [supply-chain-synthesis](https://github.com/AevaOnline/supply-chain-synthesis/) repo offers a long-form read on why that's the case, plus helpful pointers to understand and navigate it as it evolves.

For `awesome-software-supply-chain-security` we take the following high-level approach: different actors in the supply chain contribute **attestations** to the elements represented in the chain. In this process view, attestations are _emitted_, _augmented_ (e.g., during composition) and _verified_. Using this lens we can identify a large group of "subjects" (dependencies), distinct categories of "facts" (licenses or vulnerabilities) and the specific role of identity, provenance and build systems. This is the rationale behind the current headings, which are expected to evolve with the domain.

## Dependency management

This section includes: package management, library management, dependency management, vendored dependency management, by-hash searches, package, library and dependency naming, library behavior labeling, library publishing, registries and repositories, publishing gates and scans, dependency lifecycle.

* Online services that help understand what a specific dependency _is_ (usually feeding it a package identifier, such as `purl`, CPE or another form of `ecosystem:name:version`, or alternatively via hash):
  * [NSRL](https://www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl/about-nsrl/library-contents): hashes for [COTS software](https://www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl/about-nsrl/library-contents), well-integrated in tooling from [sleuthkit/hfind](http://manpages.ubuntu.com/manpages/bionic/man1/hfind.1.html) to [nsrllookup](https://github.com/rjhansen/nsrllookup)
  * A source that can be queried via a public API (HTTP and DNS!) and can be more open source-aware is [CIRCL hashlookup](https://www.circl.lu/services/hashlookup/)
  * [Repology](https://repology.org/) has legendary coverage for Linux packages across multiple distribution; its [repology-updater](https://github.com/repology/repology-updater) and other infrastructure pieces are open source. It provides an updater for [WikiData](https://github.com/repology/repology-wikidata-bot) which also has properties of interest for the supply chain security domain.
  * Tidelift's [libraries.io](https://libraries.io/) provides an [API](https://libraries.io/api) and supports over 30 package ecosystems
  * The [Software Heritage Project]() has massive ingestion capabilities and [offers an API](https://archive.softwareheritage.org/api/1/known/doc/) which can efficiently check whether a hash is known, and provide certain information on the file if so
  * [ClearlyDefined](https://docs.clearlydefined.io/using-data) provides licensing information for open source components, given their coordinates

### SBOM

This section includes: package/library scanners and detectors, SBOM formats, standards, authoring and validation, and a few applications.

### Vulnerability information exchange

## Point-of-use validations

This section includes: admission and ingestion policies, pull-time verification, 

## Identity and provenance

This section includes: 

## Frameworks and best practice references

This section includes: reference architectures and authoritative compilations of supply chain attacks and the emerging categories.

## Build techniques

This section includes: reproducible builds, hermetic builds, bootstrappable builds, special considerations for CI/CD systems, best practices building artifacts such as OCI containers, etc.

## Others in need of categorization

## Talks, articles, media coverage and other reading

