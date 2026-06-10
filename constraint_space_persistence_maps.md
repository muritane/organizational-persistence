# Constraint-Space Persistence Maps

## From Object Placement to Control-Space Authoring

---

# Abstract

This document refines the persistence-map framework by shifting the primary user interaction away from placing objects in physical or 3D space and toward authoring the conditions under which persistent organizations can exist.

The central claim is:

> A persistence map should not treat objects as the primary editable primitives. It should treat constraints, conditions, supports, flows, reserves, degradation, regeneration, and identity predicates as the editable primitives. Objects, organizations, processes, and spatial views are then derived projections of the underlying constraint space.

In this view, the user does not primarily create a robot, a whirlpool, a factory, or an institution as an object.

The user defines the conditions under which such an organization becomes viable, remains viable, degrades, regenerates, transforms, collapses, or is replaced.

The map is therefore not a world editor in the ordinary 3D sense.

It is a control-space editor for persistent organization.

---

# 0. Orientation

Let:

```text
W
```

represent a world or local environment.

Let:

```text
G_t
```

represent the global background field of time, entropy, degradation exposure, and implementation cost.

Let:

```text
K
```

represent the set of constraints and conditions currently active in the world.

Let:

```text
O
```

represent an organization, identity, process, agent, institution, robot, city, supply chain, or other persistent pattern.

Let:

```text
I_O(x)
```

represent the identity predicate of organization `O`.

Let:

```text
P_O(K, G_t)
```

represent the viability region of `O` under constraints `K` and background field `G_t`.

Let:

```text
A(O, x_t, K)
```

represent the reachable viable futures of `O` from state `x_t` under constraints `K`.

The central modeling move is:

```text
user edits K
system derives P_O, A(O, x_t, K), visible flows, objects, states, and projections
```

---

# 1. Core Shift

The previous temptation is:

```text
place object
add behavior
add support
simulate consequences
```

The refined approach is:

```text
author conditions
compute viable organizations
derive projections
inspect consequences
```

The user does not directly place persistent systems into existence.

The user modifies the constraint field in which persistent systems may or may not become viable.

In compressed form:

```text
Persistence Map = constraint-space interface for deriving viable organization
```

---

# 2. Why 3D Object Editing Is the Wrong Primitive

Most simulation and game engines begin with objects:

```text
mesh
rigid body
actor
component
scene node
position
rotation
material
```

This is useful for rendering and physical simulation.

But persistence questions are different.

They ask:

```text
What can continue?
What must be supported?
What is degrading?
What can regenerate?
What identity remains coherent?
Which futures remain reachable?
Which constraints are binding?
```

A 3D object can be a useful projection.

It should not be the source of truth.

The source of truth should be the constraint structure that makes an organization viable or nonviable.

---

# 3. The User Acts on Conditions, Not Objects

The editable primitives should be things like:

```text
constraint
condition
boundary rule
support relation
flow availability
reserve variable
degradation exposure
regeneration rule
identity predicate
transition guard
control capacity
affordance condition
```

The visible objects are derived from these primitives.

For example, instead of directly adding a whirlpool as an object, the user defines:

```text
liquid medium exists
flow gradient exists
boundary geometry exists
pressure/gravity relation exists
turbulence remains within tolerance
```

If these conditions are jointly satisfied, the system may derive:

```text
whirlpool-pattern viable
```

If the sustaining conditions disappear, the system derives:

```text
whirlpool-pattern collapses
```

The whirlpool is not a placed object.

It is a viable pattern in a constraint field.

---

# 4. Global Background Field

The first constraint is not user-created.

It is the implementation constraint of reality.

Anything physically implemented is exposed to degradation over time.

```text
physical implementation
→ time exposure
→ entropy / degradation / drift / wear / decay
→ maintenance or regeneration requirement
```

This background field is globally enabled by default.

```text
∀ implemented entity E:
  degradation_exposure(E) ≥ 0
```

For physical entities, degradation exposure is normally non-zero.

The user may disable or alter this field for analysis, but the default assumption is:

```text
time passes
implemented things degrade
persistence requires compensation
```

---

# 5. Constraints as Components

In the refined ontology, a component is not primarily a physical part.

A component is a constraint-bearing condition bundle.

For example, a battery-like support is not first represented as:

```text
3D object at position p
```

It is represented as a condition bundle:

```text
reserve variable: charge
capacity constraint: charge ≤ max_charge
degradation: self_discharge + aging
support relation: can supply electrical power
regeneration condition: charger flow available
failure condition: charge ≤ minimum_operating_threshold
```

The UI may display this as a battery.

But ontologically, it is a bundle of persistence-relevant constraints and affordances.

---

# 6. Organizations as Derived Stable Patterns

An organization is not an object manually placed into the world.

An organization is a persistent identity over a coupled set of conditions, transformations, supports, flows, reserves, and constraints.

A robot organization may be derived when conditions such as the following are satisfied:

```text
energy reserve exists
control loop can close
sensors produce usable observations
actuators can transform commands into motion
structure remains within tolerance
software/control policy remains executable
maintenance or replacement path exists
identity predicate holds
```

Then the system can derive:

```text
Robot_A exists as a viable organization
```

If enough of these conditions fail, the system derives:

```text
Robot_A degraded
Robot_A immobilized
Robot_A orphaned
Robot_A no longer viable
Robot_A identity predicate failed
```

The organization is therefore a computed persistence pattern, not merely an object record.

---

# 7. Diamond and Whirlpool as Constraint-Space Cases

A whirlpool and a diamond are not fundamentally separated by object versus process.

Both are persistent organizations under constraints.

They differ in the conditions required to preserve identity.

A whirlpool has low structural retention and high dependence on sustaining flow:

```text
requires liquid medium
requires flow gradient
requires boundary conditions
requires continuous reconstitution
collapses quickly when conditions fail
```

A diamond has high structural retention and low routine input dependence:

```text
requires compatible environment
retains lattice structure over long timescales
has low ordinary degradation rate
has almost no intrinsic self-repair
lost material is not restored by the diamond itself
```

The important distinction is:

```text
durability ≠ regeneration
```

A diamond is durable but not meaningfully self-regenerating.

A whirlpool is not durable as stored structure, but can be continuously reconstituted if sustaining conditions persist.

Both are represented by conditions over identity-relevant structure.

---

# 8. Projection Principle

The system should derive projections from constraint space.

Possible projections include:

```text
3D spatial view
graph view
flow view
support view
reachability view
viability view
reserve view
degradation view
regeneration view
failure-cascade view
control-distance view
epistemic uncertainty view
```

None of these projections is the full model.

Each is a lossy view of the same underlying constraint-space state.

The core principle is:

```text
constraint space is primary
projection space is secondary
```

A 3D view answers:

```text
where does this appear to be?
```

A constraint-space view answers:

```text
under what conditions can this continue to exist?
```

---

# 9. User Interaction Model

The primary user operations are:

```text
add condition
remove condition
modify constraint
change support relation
change flow availability
change degradation function
change regeneration rule
change identity predicate
change boundary condition
change observation assumption
fork scenario
scrub time
compare reachable futures
```

The user does not directly command:

```text
make object exist forever
move identity without cost
repair without support
create flow without source
remove degradation without changing physics
```

Instead, the user changes the control-space conditions and the system derives what becomes possible.

---

# 10. Example: Creating a Robot by Constraint Conditions

Wrong framing:

```text
place robot at x,y,z
```

Better framing:

```text
define a local organization whose identity is viable if:
  power reserve exists
  power can be converted into computation and actuation
  observations can be generated
  control signals can be generated
  actuators can affect the environment
  structure remains coherent
  degradation remains below failure threshold
  regeneration/support paths exist
```

The system may then derive a robot projection:

```text
Robot_A:
  viable now
  reserve declining
  actuator support degraded
  reachable motion set shrinking
  maintenance required before T_failure
```

The robot appears in the map because the underlying organization is viable.

It disappears, collapses, or changes status when the relevant conditions are no longer jointly satisfiable.

---

# 11. Example: Support Is Recursive

Support is not an afterthought.

A robot may require:

```text
charging support
repair support
software update support
calibration support
spare-part support
operator support
logistics support
power-grid support
manufacturing support
knowledge support
```

Each support structure is itself implemented and exposed to degradation.

Therefore support must be recursively represented:

```text
Robot_A needs Charger_1
Charger_1 needs GridPower_1
GridPower_1 needs MaintenanceCrew_1
MaintenanceCrew_1 needs Transport_1, Food_1, Tools_1, Training_1
...
```

The recursion cannot be expanded infinitely.

The map should expand only support detail that materially affects:

```text
viability
reachability
regeneration
reserve
affordance capacity
control distance
collapse risk
```

---

# 12. Local Computability of Degradation

Degradation should not require a central server to continuously update every entity.

The server can store:

```text
last known state
last update time
degradation function
support conditions
thresholds
```

Then effective state can be evaluated lazily:

```text
effective_state(T) = apply_degradation(state_at_t0, T - t0, conditions)
```

Pure degradation can be locally computed from the global clock.

Topology-changing consequences should materialize as events.

For example:

```text
battery self-discharges locally
battery crosses low-power threshold
low-power event is emitted
robot affordance set shrinks
reachable futures are recomputed
```

This avoids simulating everything continuously while preserving the reality-like assumption that degradation is always active.

---

# 13. State Reconstruction and Counterfactual Editing

The framework should support timeless debugging.

Given evidence, logs, observations, and constraints, the system reconstructs:

```text
state sequence
possible branches
binding constraints
support failures
flow interruptions
reserve depletion
identity transitions
reachable futures
```

The user can then edit constraints at a past state:

```text
what if this support relation existed?
what if this degradation rate were lower?
what if this reserve were larger?
what if this flow were interrupted earlier?
what if this identity predicate were stricter?
```

The system derives the altered projection.

The purpose is not to replay objects.

The purpose is to inspect how constraint changes alter viability and reachability.

---

# 14. The IDE Shape

The tool is an IDE for constraint-space persistence.

Core panels may include:

```text
Constraint editor
Condition graph
Timeline scrubber
Identity inspector
Flow/support graph
Viability-region viewer
Reachability viewer
Degradation/regeneration balance
Counterfactual branch manager
Projection selector
Event log
```

The 3D view, if present, is only one projection.

It should not dominate the tool.

The central editing surface should expose the constraint graph and the consequences of modifying it.

---

# 15. Formal Sketch

Let:

```text
K = {k_1, k_2, ..., k_n}
```

be active constraints and conditions.

Let:

```text
E(K, G_t)
```

be the set of derived entities, organizations, flows, supports, and affordances under `K` and background field `G_t`.

Let:

```text
Π_i(E)
```

be projection `i`, such as a 3D view, flow graph, reachability map, or viability overlay.

Then:

```text
user action: K → K'
```

The system computes:

```text
E(K, G_t) → E(K', G_t)
```

and updates projections:

```text
Π_i(E(K, G_t)) → Π_i(E(K', G_t))
```

The user edits constraints.

The system derives worlds.

---

# 16. Design Warning

Do not make human-facing categories into base ontology too early.

Avoid primitive labels such as:

```text
flow-dominated
structure-dominated
support-dominated
regeneration-dominated
```

These may be useful later as summaries or UI labels.

But the base ontology should use relations and functions:

```text
degradation rate
regeneration capacity
flow-through rate
reserve capacity
identity tolerance
repair accessibility
support dependence
control distance
```

Categories should emerge from the parameter space.

They should not define it.

---

# 17. Strategic Principle

The user is not playing with objects.

The user is playing with the conditions under which persistent organization is possible.

The map should answer:

```text
Which conditions are active?
Which organizations become viable under them?
Which organizations cease to be viable when they change?
Which supports are recursively required?
Which constraints are binding?
Which futures remain reachable?
Which interventions expand the viable region?
```

The compressed strategic principle is:

> Author constraint space; derive persistence projections.

---

# 18. Closing Statement

This refinement moves the persistence-map framework away from object placement and toward control-space authoring.

The primary editable material is not the 3D world.

The primary editable material is the set of constraints, conditions, supports, flows, reserves, degradation functions, regeneration rules, and identity predicates that determine whether an organization can exist and persist.

Objects and spatial representations still matter.

But they are projections.

The deeper map is the map of conditions under which viable organization can appear, continue, transform, recover, or collapse.

In compressed form:

> A constraint-space persistence map is an IDE for editing the conditions of possible persistence and deriving the objects, organizations, flows, and futures that those conditions permit.
