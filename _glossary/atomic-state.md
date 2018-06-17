---
title: Atomic state
oneliner: a state that has no substates
---

# Atomic state

An atomic state is a [state](state.html){:.glossary} that has no _substates_.  States that have substates are either [compound states](compound-state.html){:.glossary} or [parallel states](parallel-state.html){:.glossary}.

Atomic states are also called _simple states_.

Atomic states do not define "initial" states either.

## Notation

Atomic states can use the same notation as described in [state](state.html.html).

For atomic states that have no actions, and are otherwise empty, a very small, rounded rectangle can be used with only the name of the state inside.

## SCXML

In SCXML, an atomic state is any state that has no _state_ children:

``` xml
<state id="my_atomic_state">
  <onentry>
    <script>do_the_thing()</script>
  </onentry>
</state>
```

## xstate

In xstate, an atomic state has no `states` property.

``` js
my_atomic_state: {
  onEntry: "do_the_thing"
}
```
