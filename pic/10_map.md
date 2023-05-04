# Patterns and Tactics

## 1 Architectural Patterns

- Module patterns
  - Layered pattern
- Component-and-Connector patterns
  - Broker pattern
  - Model-View-Controller pattern
  - Pipe-and-Filter pattern
  - Client-Server pattern
  - Peer-to-Peer pattern
  - Service-Oriented Architecture (SOA) pattern
  - Publish-Subscribe pattern
  - Shared-Data pattern
- Allocation patterns
  - Map-Reduce pattern
  - Multi-tier Pattern

## 2 Relationships Between Tactics and Patterns

- Tactics are simpler than patterns
- Patterns are built from tactics;
  - if a pattern is a molecule, a tactic is an atom.
- Tactics Augment Patterns
  - Patterns solve a specific problem
  - but may have weaknesses with respect to other qualities.

## 3 Interactions between the tactics

- Each tactic has pluses (its reason for being) and minuses – side effects.
- Use of tactics can help alleviate the minuses.
- But nothing is free…
  - Each use of tactic introduces new concerns.
- Each new concern causes new tactics to be added.
- Are we in an infinite progression?
  - No. Eventually the side-effects of each tactic become small enough to ignore.
  - Augmentation ends when requirements for a specific system are satisfied.
