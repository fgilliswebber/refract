# Lexical enrichment – making an ontology multilingual
## Artefacts
- Source ontology: [fragment](Files/source.ttl) from [Model of Multiple Viewpoints (MULTI)](https://semanticweb.tools/ont/multi)
- Target ontology: [revised fragment](Files/target.ttl)
- SPARQL for CQs: [CQ1](Files/CQ1.rq)
- TMF for target viewpoint: [JSON-LD](Files/TMF.json) | [Turtle](Files/TMF.ttl)
- Shapes graphs:
  - Macro: [ShapeRefactoring](../../ShapesGraphs/ShapeRefactoring/README.md)
  - Micro: [ShapeAddAnnotationLangString](../../RefactoringActions/AddAnnotationLangString/ShapeAddAnnotationLangString.ttl)

## Description
_Example fragment for MULTI_ \
For `https://semanticweb.tools/ont/multi#Viewpoint`, add a language-specific label (`"Standpunt"@af`) to `Viewpoint`.

## Competency Questions
**CQ1:** What is the Afrikaans label for `multi:Viewpoint`?
- Target: 'Standpunt'

## Evaluation
- Shapes graph validation: [Using SHACL meta-validation](Evaluation/ShapesGraphValidation.md)
- TMF validation: [Using SHACL](Evaluation/TMFValidation.md)

---
## Rationale for classification as ontology refactoring
- _Same viewpoint_ - MULTI's viewpoint modelling perspective is unchanged.
- _Same URI_ - updated in place, versioned.
- _Structural change only_ - annotation axioms, in this case, multilingual labels, are ignored by reasoners and have no impact on the ontology's semantic content.
