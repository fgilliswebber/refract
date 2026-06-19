# Western to New Zealand viewpoint – the concept of Whales as recognised legal persons
## Artefacts
- Dummy ontology: [Source](Files/source.ttl) | [Target](Files/target.ttl)
- SPARQL for CQs: [CQ1](Files/CQ1.rq) | [CQ2](Files/CQ2.rq) | [CQ3](Files/CQ3.rq) | [CQ4](Files/CQ4.rq) | [CQ5](Files/CQ5.rq)
- TMF for target viewpoint: [JSON-LD](Files/TMF.json) | [Turtle](Files/TMF.ttl)
- Shapes graphs:
  - Macro: [ShapeLocalisation](../../../ShapesGraphs/ShapeLocalisation/README.md)
  - Micro: [ShapeAddObjectProperty](../../../RefactoringActions/AddObjectProperty/ShapeAddObjectProperty.ttl) | [ShapeAddPropertyDomainRange](../../../RefactoringActions/AddPropertyDomainRange/ShapeAddPropertyDomainRange.ttl) | [ShapeAddSuperclassAssertion](../../../RefactoringActions/AddSuperclassAssertion/ShapeAddSuperclassAssertion.ttl) | [ShapeAddPropertyRestriction](../../../RefactoringActions/AddPropertyRestriction/ShapeAddPropertyRestriction.ttl) | [ShapeChangeAnnotationValue](../../../RefactoringActions/ChangeAnnotationValue/ShapeChangeAnnotationValue.ttl)

## Description
The goal is to transform a marine ontology to reflect the New Zealand legal framework, which extends legal personhood to non-human natural entities such as whales, introducing a guardian relationship and reclassifying whales as natural legal persons.

## Competency Questions
**CQ1:** Is `mar:Whale` a subclass of `mar:NaturalLegalPerson`?
- Source: No
- Target: Yes

**CQ2:** Does `marnz:hasGuardian` exist?
- Target: Yes

**CQ3:** What is the domain of `marnz:hasGuardian`?
- Target: `mar:NaturalLegalPerson`

**CQ4:** What is the range of `marnz:hasGuardian`?
- Target: `mar:Guardian`

**CQ5:** Does `mar:Whale` have a `someValuesFrom` restriction on `marnz:hasGuardian`?
- Target: Yes

## Evaluation
- TMF validation: [Using SHACL](Evaluation/TMFValidation.md)

---
## Rationale for classification as ontology localisation
- _Different viewpoint_ - the target ontology adopts a New Zealand political community viewpoint, which recognises whales as legal persons under New Zealand law.
- _Different URI_ - the target is published to a new URI, reflecting the new viewpoint.
- _Semantic change driven by a community-specific viewpoint_ - the New Zealand legal framework extends legal personhood to non-human natural entities such as whales, a concept absent from the source ontology.
