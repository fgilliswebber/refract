# Semantic Action

**Definition type:** OWL Class \
**Fragment identifier:** `fract:SemanticAction` \
**URI:** `https://w3id.org/refract#SemanticAction`

An atomic action that results in a change to the semantic meaning of the ontology. For example, adding a superclass assertion changes the ontological commitment of a class without introducing a new ontology element. A refactoring action may be both a semantic and a structural action - for example, adding a class introduces a new ontology element and simultaneously carries ontological commitment.

For the list of semantic actions, see [Local Action](LocalAction.md).

## Position in class hierarchy

`owl:Thing` → `rdfs:Class` → `prov:Activity` → `fract:RefactoringAction` → `fract:LocalAction` → `fract:AtomicAction` → `fract:SemanticAction`

## See also

* [Atomic Action](AtomicAction.md)
* Atomic Action > [Structural Action](StructuralAction.md)
* Atomic Action > [Annotation Action](AnnotationAction.md)
