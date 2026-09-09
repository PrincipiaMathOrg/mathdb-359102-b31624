# MathDB 359102

Lean 4 formalization of the Principia project [MathDB 359102](https://principia-staging.anton-8d8.workers.dev/app/projects/b31624917bb44ffc82dfddc13b986c10), in the Palomar layout.

Let H be the Hilbert space under consideration, and let M⊆ H be bounded. The set M is **uniformly separated** if _x≠ y∈ M\|x-y\|≠ 0. **Uniform separation conjecture.** If M is bounded and uniformly separated, then M is ℓ^1-bounded. This is posed as an open question in the paper; no resolution is supplied there.

## Layout

- `Challenge.lean` states the advertised results with `sorry`; it may import only Lean core, Mathlib, Tau Ceti or CSLib.
- `Solution.lean` proves the same declarations by importing the development in `MathDB359102/`.
- `comparator.json` lists the declarations Comparator checks between the two.
- `formalization.yaml` records the public description, provenance, authorship, automation and review status. Replace every `TEMPLATE` value.

## Checks

```text
lake exe cache get
lake build
ruby scripts/validate-formalization.rb
./scripts/verify-comparator.sh
```

## Submission

The project owner submits the pinned commit to Palomar from the project page on Principia, which uses https://submit.palomar-registry.org/ on their behalf. Only a responsible author or maintainer, or someone with their approval, may submit.

Repository: https://github.com/PrincipiaMathOrg/mathdb-359102-b31624
