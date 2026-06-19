# Structural Action

**Definition type:** OWL Class \
**Fragment identifier:** `fract:StructuralAction` \
**URI:** `https://w3id.org/refract#StructuralAction`

An atomic action that adds or removes an ontology element, such as a class, object property, or annotation property, without necessarily affecting the semantic meaning of the ontology. For example, adding an object property is a structural change; the semantic meaning of the ontology is only affected once an assertion is made using that property. A refactoring action may be both a structural and a semantic action  for example, adding a class introduces a new ontology element and simultaneously carries ontological commitment.

For the list of structural actions, see [Local Action](LocalAction.md).

## Position in class hierarchy

`owl:Thing` → `rdfs:Class` → `prov:Activity` → `fract:RefactoringAction` → `fract:LocalAction` → `fract:AtomicAction` → `fract:StructuralAction`

## See also

* [Atomic Action](AtomicAction.md)
* Atomic Action > [Semantic Action](SemanticAction.md)
* Atomic Action > [Annotation Action](AnnotationAction.md)
