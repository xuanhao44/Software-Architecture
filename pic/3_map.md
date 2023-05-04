# Understanding quality attributes

## 1 Architecture and Requirements

- 1.1 Functional requirements
  - Functionality has a strange relationship to architecture: functionality does not determine architecture.
- 1.2 Quality attribute requirements
  - Two Categories of QA
    - runtime
      - Availability
      - performance
      - usability
      - security
    - properties of the development of system
      - Modifiability
      - Testability
  - QA Considerations
    - Untestable definitions
    - Overlapping concerns
    - sloved by quality attribute scenario!
- 1.3 Constraints

## 2 Quality attribute scenario

- Stimulus. The stimulus is a condition that requires a response when it arrives at a system.
- Source of stimulus. This is some entity (a human, a computer system, or any other actuator) that generated the stimulus.
- Response. The response is the activity undertaken as the result of the arrival of the stimulus.
- Response measure. When the response occurs, it should be measurable in some fashion so that the requirement can be tested.
- Environment. The stimulus occurs under certain conditions. The system may be in an overload condition or in normal operation, or some other relevant state.
- Artifact. This may be a collection of systems, the whole system, or some piece or pieces of it. Some artifact is stimulated.

## 3 An architectural tactic

- **Achieving Quality Attributes through Tactics**
- A tactic is a design decision for a single quality attribute
- A tactic does not consider tradeoffs among quality attributes
- Architectural patterns can be seen as “packages” of tactics, in which tradeoffs are considered

## 4 Architectural design decisions

- Allocation of responsibilities
- Coordination model
- Data model
- Management of resource
- Mapping among architectural elements
- Binding time decisions
