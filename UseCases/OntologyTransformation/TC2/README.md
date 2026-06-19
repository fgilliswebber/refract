# Provenance reframing – change of cultural heritage ontology from acquisition to contested heritage
## Artefacts
- Dummy ontology: [Source](Files/source.ttl) | [Target](Files/target.ttl)
- SPARQL for CQs: [CQ1](Files/CQ1.rq) | [CQ2](Files/CQ2.rq) | [CQ3](Files/CQ3.rq) | [CQ4](Files/CQ4.rq) | [CQ5](Files/CQ5.rq) | [CQ6](Files/CQ6.rq) | [CQ7](Files/CQ7.rq) | [CQ8](Files/CQ8.rq)
- TMF for target viewpoint: [JSON-LD](Files/TMF.json) | [Turtle](Files/TMF.ttl)
- Shapes graphs:
  - Macro: [ShapeTransformation](../../../ShapesGraphs/ShapeTransformation/README.md)
  - Micro: [ShapeRenameClass](../../../RefactoringActions/RenameClass/ShapeRenameClass.ttl) | [ShapeAddClass](../../../RefactoringActions/AddClass/ShapeAddClass.ttl) | [ShapeAddAnnotationLangString](../../../RefactoringActions/AddAnnotationLangString/ShapeAddAnnotationLangString.ttl) | [ShapeAddInstance](../../../RefactoringActions/AddInstance/ShapeAddInstance.ttl) | [ShapeChangeInstanceAssertion](../../../RefactoringActions/ChangeInstanceAssertion/ShapeChangeInstanceAssertion.ttl) | [ShapeDeleteAnnotation](../../../RefactoringActions/DeleteAnnotation/ShapeDeleteAnnotation.ttl) | [ShapeAddInstancePropertyAssertion](../../../RefactoringActions/AddInstancePropertyAssertion/ShapeAddInstancePropertyAssertion.ttl) | [ShapeAddAnnotation](../../../RefactoringActions/AddAnnotation/ShapeAddAnnotation.ttl)

## Description
The goal is to transform a cultural heritage ontology from a neutral museum acquisition viewpoint to a contested heritage viewpoint, reframing the same entities from a different ethical and cultural perspective.

## Competency Questions
**CQ1:** Does `chc:HumanRemains` exist?
- Source: No
- Target: Yes

**CQ2:** Is `ch:SarahBaartman` an instance of `chc:HumanRemains`?
- Target: Yes

**CQ3:** What is the `skos:prefLabel` of `ch:SarahBaartman`?
- Target: Empty result set

**CQ4:** What is the `rdfs:label` of `ch:SarahBaartman`?
- Target: `Sarah Baartman`

**CQ5:** What is the `chc:donationConsentStatus` of `ch:SarahBaartman`?
- Target: `chc:ConsentNotGivenImplicit`

**CQ6:** What is the `ch:removedFromDisplay` value for `ch:SarahBaartman`?
- Target: `1974`

**CQ7:** What is the `chc:repatriationDate` for `ch:SarahBaartman`?
- Target: `2002-05-06`

**CQ8:** Does `ch:VenusHottentote` exist?
- Source: Yes
- Target: No

## Evaluation
- Shapes graph validation: [Using SHACL meta-validation](Evaluation/ShapesGraphValidation.md)
- TMF validation: [Using SHACL](Evaluation/TMFValidation.md)

---
## Rationale for classification as ontology transformation
- _Different viewpoint_ - the target ontology adopts a contested heritage viewpoint, replacing the neutral museum acquisition viewpoint of the source ontology.
- _Different URI_ - the target is published to a new URI, reflecting the new viewpoint.
- _Semantic change driven by viewpoint change_ - the reclassification of Sarah Baartman from a museum specimen to human remains, the addition of consent status metadata, and the repatriation provenance represent a fundamental reframing of the same entity from a different ethical and cultural perspective.
