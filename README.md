# Ecological Traitdata Standard (ETS)

This repository hosts the **Ecological Traitdata Standard**, which defines terms for the use in datasets containing quantitative and qualitative functional traits. 

The repository contains: 

- the 'source file' of the glossary (in .csv format), defining the terms and containing the URIs.
- the source files of the documentation website (.Rmd, .yml), which are parsed in [RStudio as a Rmarkdown Website](http://rmarkdown.rstudio.com/rmarkdown_websites.html) and served via [Github pages](https://pages.github.com/) (output in folder docs) to https://ecologicaltraitdata.github.io/ETS/. 

A machine readable version will be generated and hosted by GFBio in RDF format.

## fields

The glossary contains several fields which are defined as follows: 

| field        | definition                          |
|--------------|-------------------------------------|
| Namespace    | The collection of terms that the term is part of.   | 
| Identifier   | The Uniform Resource Identifier used to uniquely identify a term.  If the term is an exact duplicate from Darwin Core or other glossaries, Identifier will forward directly to this definition. |
| Refines      | If the definition builds on terms of the Darwin Core or other Glossaries, the original term is linked here (URI) |
| Replaces     | The URI of the term  that is replaced by this term. | 
| Deprecated   | Flaggin deprecated terms. If TRUE, the term should not be used for new datasets, but will be maintained for compatibility. |
| ReplacedBy   | If a term is deprecated not be used any more, this field provides the URI of the  replacement term. |
| Version      |  | 
| DateIssued   |  | 
| DateModified |  | 
| Definition   | A statement that represents the concept and essential nature of the term.  | 
| Comment      | Clarification and examples. |

## Contribute

Please use the [issues-page](https://github.com/EcologicalTraitData/ETS/issues) for discussion and revision on individual terms, and settle the issue here before filing a pull-request that implements an update. 

## Versioning

**Current Version is 0.6**

Terminologies must provide a stability of definitions. If publications refer to the URI of a term, the definition found must be stable and be true to the definition intended by the author.

That said, definitions of terms can only be broadened or made more explicit, if the original sense of the definition remains valid. The discussion leading to a refinement of a term should consider this. If a definition changes substantially, it should receive an own URI and replace any redundant or deprecated terms. The deprecated terms will remain available at the same URI. 

At some point, a new major version of the Traitdata Standard may be issued, providing new versioned URIs for all terms of the standard that have been altered since the previous major version. 

## Suggested Citation

To refer to **this version** of the ETS please cite: 
  
  > Schneider et al. (2017) Ecological Traitdata Standard, v0.6, URL: https://ecologicaltraitdata.github.io/ETS/v0.6/ , DOI: [10.5281/zenodo.1041733](https://doi.org/10.5281/zenodo.1041733)  

Please also cite the methods paper for the rationale and general considerations of semantic standardization of trait data: 
  
  > Florian D. Schneider, Malte Jochum, Gaetane LeProvost, Andreas Ostrowski, Caterina Penone, Nadja K. Simons (in preparation) Introducing an Ecological Trait-data Standard. 
  
## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Ecological Traitdata Standard </span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Florian D. Schneider, Nadja K. Simons, Caterina Penone, Andreas Ostrowski</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
