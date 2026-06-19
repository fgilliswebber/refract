# Normalisation of naming conventions – renaming of class name(s)
## Artefacts
- Source ontology: [fragment](Files/source.ttl) from [The Ontology of Data Analysis and Management (EDAM)](https://bioportal.bioontology.org/ontologies/EDAM)
- Target ontology: [revised fragment](Files/target.ttl)
- SPARQL for CQs: [CQ1](Files/CQ1.rq) | [CQ2](Files/CQ2.rq)
- TMF for target viewpoint: [JSON-LD](Files/TMF.json) | [Turtle](Files/TMF.ttl)
- Shapes graphs:
  - Macro: [ShapeRefactoring](../../../ShapesGraphs/ShapeRefactoring/README.md)
  - Micro: [ShapeRenameClass](../../../RefactoringActions/RenameClass/ShapeRenameClass.ttl)

## Description
_Example fragment from EDAM:_ \
For `http://edamontology.org/operation_2928`, change the fragment identifier from `operation_2928` to `operationAlignment`.

## Competency Questions
**CQ1:** What is the superclass of `operation_2928`?
- Source: 'Operation' (`operation_0004`)
- Target: Empty result set

**CQ2:** Does `operationAlignment` exist in the ontology?
- Target: Yes

## Evaluation
- Shapes graph validation: [Using SHACL meta-validation](Evaluation/ShapesGraphValidation.md)
- TMF validation: [Using SHACL](Evaluation/TMFValidation.md)

---
## Rationale for classification as ontology refactoring
- _Same viewpoint_ - EDAM's bioinformatics perspective is unchanged.
- _Same URI_ - updated in place, versioned.
- _Structural change only_ - there is no change to a concept's meaning, definition, or position in the hierarchy when changing the fragment identifier.
