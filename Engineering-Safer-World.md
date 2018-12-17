# Engineering a Safer World: Systems Thinking Applied to Safety
by Nancy Leveson

## Terms

- hazard
- interactive coplexity
- system accident: accident that araises in interactions among components rather
    than failure of individual component
- dysfunctional interactions: interactions that can lead to hazardous states in
    the controlled process
- safety constraints
- control structure
- STAMP: systems-theoretic accident model and processes
- dead time: actuator does not respond immediately to an external signal
- time constants: delays in responding to manipulated variables
- feedback delays: sensors may obtain values only at certain sampling intervals

## Table of of contents

I. Foundations
1. Why do we need something different?
2. Questioning the foundations of traditional safety engineering
3. Systems theory and its relationship to safety
II STAMP: An accident model based on systems theory



## Notes (from [A New Accident Model for Enigneering Safer Systems][1])

[1]: http://sunnyday.mit.edu/accidents/safetyscience-single.pdf

Redundancy may even increase risk by adding complexity. All software problems
detected during the flight testing of a NASA experimental aircraft using two
versions of the computer based control system resulted from errors in the
redundancy management system added to protect against software errors - the much
simpler control software itself worked perfectly. Overconfidence in redundancy
and misunderstanding of the failure modes of software-implemented components has
played an important role in recent aerospace accidents, such as the loss of the
Ariane 5 on its first flight.

Increasing dependence on info systems creating the potential for loss of
information or incorrect information that can lead to unacceptable physical,
scientific or finanical losses.

We are attempting to build systems that are beyond our ability to intellectually
manage.

Inadequacies in communication between humans and machines is becoming an
increasingly important factor in accidents.

Most software-related accidents have been system accidents, usually operation is
exactly what software engineers intended

Safety is an emergent property taht arises when the system copmonents interact
within an environment.

curse of flexibility - computer has eliminated many physical constraints of
electromechanical dvices.

It is possible and even quite easy to build software that we cannot understand
in terms of being able to determine how it will behave under all conditions.

increase in system accidents stemming from intellectual unmanageability reltaed
to interactively complex & tightly coupled designs that allow potentially unsafe
interactions to go undetected during development

Control software contriubts to accident by not enforcing appropriate constraints
on behavior or by commanding behavior that violates the constraints.

### Classification of accident factors

```
1. Inadequate enforcement of constraints (control actions)
    1.1 Unidentified hazards
    1.2 Inappropriate, ineffective, or missing control actions for identified
        hazards
    1.2.1 Design of control algorithm (process) does not enforce constraints
        - Flaw(s) in creation process
        - Process changes without appropriate change in control algorithm
            (asynchronous evolution)
        - Incorrect modification or adaptation
    1.2.2 Process models inconsistent, incomplete, or incorrect (lack of linkup)
        - Flaw(s) in creation process
        - Flaw(s) in updating proces (asynchronous evolution)
        - Time lags and measurement inaccuracies not accounted for
    1.2.3 Inadequate coordination among controllers and decision makers
        (boundary and overlap areas)
2. Inadequate execution of control action
    2.1 Communication flaw
    2.2 Inadequate actuator operation
    2.3 Time log
3. Inadequate or missing feedback
    3.1 Not provided in system design
    3.2 Communication flaw
    3.3 Time lag
    3.4 Inadequate sensor operation (incorrect or no information provided)
```
