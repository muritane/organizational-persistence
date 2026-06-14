# Admissible Path Filter

## Endpoint Compression, Bounded Transition, Recoverability, and the Collapse of False Possibility

---

# Abstract

This document defines an admissible path filter.

The central claim is:

> A described endpoint is not an executable possibility unless an admissible transformation path connects the current state to that endpoint within a bounded environment.

Many statements appear possible only because they suppress the transformation path.

They name a destination while omitting:

```text
intermediate states
transition constraints
resources
losses
precision limits
support structures
coordination requirements
activation paths
continuity conditions
```

Once the path is restored, many apparent possibilities collapse.

The issue is not that the endpoint is logically contradictory.

The issue is that the endpoint may not be reachable by any realizable sequence of bounded transitions.

In compressed form:

> Possibility without a path is only endpoint description. Operational possibility requires admissible transition.

This filter extends the constrained-transformation, recoverability, and executability frameworks by focusing on a specific failure mode:

```text
current state
→ desired endpoint
```

being treated as if it already implies:

```text
current state
→ admissible transition chain
→ desired endpoint
```

The missing distinction is:

```text
describable endpoint
≠
reachable state
```

A marker on a map is not a route.

A goal is not a transition model.

A label is not capacity.

A serving is not produced by naming a fraction of an apple.

A future is not reached by describing it.

---

# 0. Orientation

Let:

```text
x_t
```

represent the current state of a system at time `t`.

Let:

```text
y
```

represent a proposed target state, goal, endpoint, destination, output, or desired future.

Let:

```text
T
```

represent a transformation.

Let:

```text
K
```

represent the active constraint regime.

Let:

```text
A_K(x_t)
```

represent the set of states reachable from `x_t` under constraint regime `K`.

Let:

```text
P = (x_t, x_1, x_2, ..., y)
```

represent a path from the current state to the target.

Let:

```text
E_i = (x_i, x_{i+1})
```

represent one transition edge in the path.

The central question is not first:

```text
Can y be described?
```

but:

```text
Does there exist an admissible path from x_t to y?
```

In compressed form:

> A target becomes operationally relevant only when a bounded transition chain can connect the present to the target.

---

# 1. Endpoint Description Is Not Reachability

A statement may describe a possible endpoint:

```text
one apple feeds one million people
```

or:

```text
the organization becomes innovative
```

or:

```text
the robot reaches the target pose
```

or:

```text
the car arrives at the destination
```

or:

```text
the institution optimizes public value
```

But endpoint description does not provide a path.

To become operationally meaningful, the statement must specify or imply:

```text
current state
→ transition sequence
→ endpoint
```

Without this, the statement remains a description of a possible final state, not a claim about executable transformation.

In compressed form:

> Naming where something should end up does not explain how it gets there.

---

# 2. Path Suppression

Path suppression occurs when a statement compresses away the intermediate transformations required to move from one state to another.

The compressed form is:

```text
x_t → y
```

The expanded form is:

```text
x_t
→ x_1
→ x_2
→ x_3
→ ...
→ y
```

Each local transition must be admissible:

```text
(x_i, x_{i+1}) ∈ T_K
```

where `T_K` is the transition relation permitted by the active constraints.

If even one required transition is impossible, unavailable, unsupported, or incompatible with the constraint surface, the path fails.

In compressed form:

> A path is not valid because its endpoint is imaginable. It is valid only if each step is admissible.

---

# 3. The Map Marker Is Not the Route

A map marker identifies a target location.

It does not establish reachability.

For a routing system, the relevant object is not merely:

```text
destination
```

but:

```text
current location
+ graph of roads
+ admissible edges
+ costs
+ constraints
+ route
```

A routing system does not reason:

```text
Paris exists
therefore arrive in Paris
```

It asks:

```text
Which neighboring state is reachable next?
```

Then:

```text
Which state is reachable after that?
```

and continues until a path is found or no admissible path exists.

In compressed form:

> A destination is a target state. A route is a proof of reachability.

---

# 4. A* as a Path-Reality Discipline

A* search does not search arbitrary fantasies.

It searches a graph.

A graph defines:

```text
nodes
edges
costs
admissible transitions
```

The algorithm expands reachable successor states from the current state.

It does not jump to the goal merely because the goal is known.

At each step, the algorithm asks:

```text
from this node, which next nodes are reachable?
```

The heuristic may point toward the destination.

But the heuristic is not the path.

The destination estimate does not override edge admissibility.

If there is no edge, there is no transition.

If there is no transition chain, there is no route.

In compressed form:

> A* separates desire from reachability: the goal guides search, but admissible edges determine movement.

---

# 5. The Apple Example

Suppose there is:

```text
1 apple
```

and:

```text
1,000,000 people
```

One may say:

```text
each person receives 1/1,000,000 of an apple
```

As arithmetic, this is valid.

As execution, it suppresses the transformation path.

To realize the claim, one needs:

```text
cutting mechanism
precision
surface stability
loss management
transport
allocation
hygiene
recipient access
minimum usable portion size
```

If no device can separate the apple at the required granularity, the fractional allocation remains a mathematical endpoint rather than an executable distribution.

If the resulting portion is smaller than the threshold for usable nourishment, then the claim may remain formally true while becoming operationally irrelevant.

In compressed form:

> A fraction is not a serving unless a transformation path can produce, preserve, deliver, and use it.

---

# 6. Bounded Transition and the Rejection of Teleportation

A bounded system cannot generally move from any state to any other state in one step.

Reality does not allow arbitrary state replacement.

Movement must pass through admissible transitions.

For physical systems, this often appears as bounds on:

```text
position
velocity
acceleration
jerk
force
energy
friction
heat
material strength
control bandwidth
sensor resolution
actuator limits
```

For organizational systems, analogous bounds include:

```text
attention
coordination
trust
legitimacy
authority
information
skills
resources
time
communication capacity
institutional memory
compliance
workflow capacity
```

In compressed form:

> Bounded systems do not teleport through state space. They traverse constraint-governed paths.

---

# 7. The Zero-Jerk Assumption

In physics, jerk is the rate of change of acceleration.

A transition model that assumes instantaneous changes in acceleration effectively suppresses path smoothness.

In broader systems, a similar error occurs when a proposal assumes instantaneous reconfiguration without transition cost.

Examples:

```text
people instantly coordinate
institutions instantly adapt
systems instantly scale
skills instantly appear
trust instantly forms
rules instantly bind
models instantly update
resources instantly activate
```

These are not always literally claims about mechanical jerk.

They are claims that suppress transitional continuity.

They assume that the system can move from one regime to another without passing through the costly intermediate states required by bounded implementation.

A general zero-jerk filter asks:

```text
What transition is being treated as instantaneous?
What intermediate states are being omitted?
What rate limits are being ignored?
What support structures must change gradually?
What breaks if the change is discontinuous?
```

In compressed form:

> A zero-jerk assumption hides the cost and structure of changing how change itself changes.

---

# 8. Describability, Representability, Reachability, Executability

The admissible path filter separates four levels.

## 8.1 Describability

A state can be named or imagined.

```text
y is describable
```

This is weak.

A sentence can describe many things that have no reachable path from the current state.

## 8.2 Representability

A state can be encoded within some representation system.

```text
y ∈ representation space
```

This is stronger than describability, but still not enough.

A map may represent a destination that cannot be reached from the current position.

## 8.3 Reachability

A state is reachable when there exists a valid path under the constraint regime.

```text
y ∈ A_K(x_t)
```

This requires:

```text
∃P = (x_t, x_1, ..., y)
such that every transition in P is admissible
```

## 8.4 Executability

A reachable state becomes executable when the path can be instantiated by an execution locus with sufficient resources, activation, binding, and support.

This requires:

```text
reachable path
+ execution locus
+ resource basis
+ transition model
+ realizing mechanism
+ constraint surface
```

In compressed form:

> Describable does not imply representable. Representable does not imply reachable. Reachable does not imply executable.

---

# 9. False Possibility

False possibility is the appearance of possibility created by suppressing path, constraint, or implementation.

The common form is:

```text
I can describe y
therefore y is possible
```

The path-aware form is:

```text
I can describe y
but is y reachable from x_t under K?
```

If the answer is no, the endpoint is not an operational possibility for the current system.

It may be:

```text
logically conceivable
mathematically definable
representationally encodable
rhetorically attractive
morally desirable
```

but it is not yet:

```text
reachable
executable
recoverable
instantiable
```

In compressed form:

> False possibility appears when endpoint description is mistaken for admissible path existence.

---

# 10. Choice After Constraints

Choice does not occur over all imaginable endpoints.

Choice occurs within an admissible region.

Let:

```text
Y_all
```

represent all describable target states.

Let:

```text
Y_rep
```

represent target states representable by the system.

Let:

```text
Y_reach(x_t,K)
```

represent target states reachable from the current state under constraints.

Let:

```text
Y_exec(x_t,K,O)
```

represent target states executable by organization `O` under those constraints.

Then:

```text
Y_exec ⊆ Y_reach ⊆ Y_rep ⊆ Y_all
```

The apparent choice set may be enormous at the descriptive level.

The effective choice set may be small at the executable level.

In extreme cases, there may be only one admissible path, or none.

In compressed form:

> Choice begins after typing, representation, reachability, and execution constraints have already reduced the space.

---

# 11. The Uniformity and Randomness Boundary Cases

A uniform field can be tracked only vacuously.

If:

```text
I(x,y,t) = c
```

for all positions and times, then there is no internal distinction to exploit.

The system can say:

```text
same
same
same
```

but no internal structure is being recovered.

An independent random field has distinctions but no stable coupling.

If:

```text
I_i ⫫ I_j
```

for relevant pixels or states, then knowing one state does not constrain another.

There may be differences everywhere, but they do not form recoverable organization.

Only constrained variation supports usable structure.

In compressed form:

> Uniformity fails distinction. Independent randomness fails recoverability. Constrained variation supports path-relevant structure.

---

# 12. Protocols as Induced Possibility Spaces

A protocol does not begin with arbitrary infinity.

It defines an operational state space.

For example:

```text
IPv4
→ 32-bit address representation
→ finite address space
→ routing and allocation constraints
```

Similarly:

```text
CAN bus
→ identifier structure
→ arbitration rules
→ timing constraints
→ admissible message behavior
```

The protocol does not merely filter a prior infinity of possible communications.

It induces the space in which communication is valid.

In compressed form:

> Constraints do not merely remove possibilities. They define the state space in which operational possibility exists.

---

# 13. Recoverability and Path Dependence

A structure is useful when relevant distinctions remain recoverable through transformation.

This means the path matters.

A source may preserve generative constraints.

A projection may preserve only appearance.

A compressed representation may preserve some distinctions while destroying others.

A transition chain may gradually degrade the distinctions required for later reconstruction.

Thus the question is not only:

```text
Is the endpoint reached?
```

but:

```text
Which distinctions survive the path?
```

A path that reaches a destination while destroying the structure needed for use may fail the actual objective.

In compressed form:

> Reachability is not enough if the path destroys the distinctions the endpoint was supposed to preserve.

---

# 14. Path-Admissibility Test

A proposed statement can be tested by asking:

## 1. What is the current state?

```text
x_t = ?
```

If the current state is unspecified, the claim may be under-typed.

## 2. What is the target state?

```text
y = ?
```

If the target is only a slogan, the claim may be under-typed.

## 3. What is the state space?

```text
X = ?
```

If the representation cannot encode the relevant states, the claim may be ill-formed.

## 4. What transitions are admissible?

```text
T_K = ?
```

If transition constraints are absent, the path is undefined.

## 5. Does a path exist?

```text
∃P : x_t → y ?
```

If no path exists, the endpoint is not reachable.

## 6. What is the cost of the path?

```text
cost(P) = ?
```

If the cost exceeds available resources, the path is not executable.

## 7. What supports the path?

```text
support(P) = ?
```

If the support structure is missing, the path remains representational.

## 8. What distinctions survive the path?

```text
D_recovered(P) = ?
```

If the path destroys the needed distinctions, the endpoint may be reached only nominally.

In compressed form:

> A path claim is well-formed only when current state, target state, state space, admissible transitions, costs, supports, and preserved distinctions are sufficiently specified.

---

# 15. Diagnostic Outcomes

The admissible path filter can classify claims into several outcomes.

## 15.1 Outside Target Domain

The statement is exploratory, aesthetic, speculative, or descriptive and is not being asserted as reachable or executable.

No path test is needed yet.

## 15.2 Endpoint-Only

The statement names a desired endpoint but gives no path.

Example:

```text
make society coordinated
```

Outcome:

```text
under-typed
```

## 15.3 Path-Sketched

The statement gives a rough path but omits key constraints, resources, or supports.

Outcome:

```text
under-typed but potentially repairable
```

## 15.4 Path-Admissible

The statement specifies a current state, target state, transition chain, constraints, resources, and support structure sufficient for at least one executable transition path.

Outcome:

```text
well-typed for reachability/execution analysis
```

## 15.5 Path-Impossible

The statement requires a transition incompatible with the constraint surface.

Examples:

```text
instant coordination without communication
infinite division without a separating mechanism
control over an unobservable variable
arrival without route
capacity without activation path
```

Outcome:

```text
ill-typed as specified
```

In compressed form:

> A failed path claim may be missing detail, or it may require an impossible transition. These are different failures.

---

# 16. Relation to Executability

The admissible path filter is narrower than the executability filter.

The executability filter asks:

```text
Does this abstraction possess the minimum structure required to make contact with execution?
```

The admissible path filter asks:

```text
Does this claim suppress the transition path between current state and endpoint?
```

The two filters overlap.

A claim with no admissible path usually fails executability.

But a path may be admissible in abstract while still failing execution because no locus, resource, binding mechanism, or support structure can instantiate it.

Thus:

```text
admissible path
≠
full executability
```

but:

```text
no admissible path
→
no execution as specified
```

In compressed form:

> Path admissibility is a prerequisite for execution, but not the whole of execution.

---

# 17. Relation to Constrained Transformation

The constrained-transformation framework begins with:

```text
distinction
+
change
+
constraint
```

and asks how recoverable structure, organization, persistence, value, and control emerge.

The admissible path filter applies this logic to claims about action and possibility.

It says:

```text
change is not arbitrary replacement
```

but:

```text
bounded transition under constraint
```

A target state matters only if it lies inside the reachable region induced by the transformation regime.

In compressed form:

> Constrained transformation gives the ontology. The admissible path filter gives a diagnostic for claims that ignore it.

---

# 18. Relation to Persistence Maps

A persistence map is not primarily a map of where objects are.

It is a map of:

```text
reachable futures
viability regions
sustaining flows
regeneration paths
support structures
constraint surfaces
control capacity
```

The admissible path filter provides a local test for such maps.

For any proposed transition:

```text
x_t → y
```

the map must ask:

```text
is y inside the reachable viable region?
through which path?
at what cost?
with which supports?
under which constraints?
with what degradation along the way?
```

In compressed form:

> A persistence map turns endpoint fantasy into path-constrained reachability analysis.

---

# 19. Compact Derivation

A compressed derivation may be written as follows:

```text
1. A target can be described.

2. Description does not imply representation.

3. Representation does not imply reachability.

4. Reachability requires admissible transitions.

5. Admissible transitions require a constraint regime.

6. A path is a chain of admissible transitions.

7. Execution requires a realizable path plus locus, resources, support, and binding.

8. Persistence requires that identity-relevant distinctions survive the path.

9. Therefore endpoint claims are premature unless path, constraint, support, and recoverability are specified.
```

In compressed form:

> To say that a future is possible is not to name it, but to show how it remains reachable through bounded transformation.

---

# 20. Final Compression

The framework can be compressed into one chain:

```text
described endpoint
→ represented target
→ admissible state space
→ reachable path
→ executable transition
→ preserved distinctions
→ usable outcome
```

Or more simply:

> A destination is not a route. A goal is not a path. A fraction is not a serving. A label is not capacity. A future is not reachable merely because it can be named. Operational possibility begins only where a bounded transformation path exists.

