---
name: m3-review
description: Review project sources and diffs against Material 3 foundations, styles, and components. Use for code-only reviews without running applications, browsers, or devices.
---

# Material 3 review

Review project sources against the Material 3 skills available in this collection.
Use only project files and the local Material 3 skill references.
Do not run applications, tests, previews, browsers, emulators, devices, or assistive tools.
Inspect test source and stored results as project evidence without executing checks.
For a requested live review, use [m3-review-runtime](../m3-review-runtime/SKILL.md) as a separate task.
Do not make runtime review a prerequisite for this source review.
Use this workflow in the main agent or a dedicated review agent.
Review and report. Change application files only when the user also requests fixes.

## Set the scope

- Use change review by default for requests about recent work, a diff, or a pull request.
- Use full review when the user requests an application-wide evaluation.
- For change review, identify the comparison base and inspect the complete relevant diff, including new files.
- If the base is unclear, use available task context. State the selected base and any limits.
- Trace changed UI into affected screens, shared components, and primary and secondary user journeys.
- Check surrounding UI when changes can affect consistency, navigation, layout, or behavior.
- For full review, inventory routes, screens, shared components, and representative user journeys.
- Record the platform, supported layouts, themes, locales, input methods, and relevant product constraints.
- State assumptions when product goals or supported contexts are unknown. Ask only when missing information prevents useful review.

## Discover the complete review criteria

Discover the current skill inventory at review time. Do not rely on a fixed list of component names.
Locate sibling `m3-foundation-*`, `m3-styles-*`, and `m3-components-*` skills relative to this skill directory.
If skills are installed separately, use the available skill catalog to locate them.
Report missing skills that prevent an area from receiving a complete review.

Read each skill's name and description to assess applicability across the entire inventory.
Mark each skill as applicable, not applicable, or not verified. Give a reason for exclusions and verification gaps.
Group related entries in the report when their status and reason match. Keep every discovered skill traceable.
Read the full instructions of every applicable skill before making findings in that area.
Apply their criteria through source inspection only. Do not execute their runtime verification instructions.
Read linked source maps and references when rules depend on measurements, tokens, diagrams, or platform details.

Consider all three groups:

| Group | Review focus |
| --- | --- |
| Foundations | Usability, accessibility, structure, focus, inputs, gestures, adaptive layouts, density, spacing, states, selection, writing, localization, and research limits |
| Styles | Color systems and roles, contrast, typography, icons, shape, elevation, spacing, and motion |
| Components | Component choice, hierarchy, composition, anatomy, tokens, behavior, labels, accessibility, layouts, and interaction states |

Use the discovered skills as the detailed criteria. This table does not replace their instructions.
Distinguish mandatory rules, recommendations, and illustrative examples.
Do not turn an example, preferred tactic, or platform-specific rule into a universal requirement.
Preserve documented exceptions and conditions. Do not invent missing measurements or behavior.
If sources conflict, report the conflict and its effect. Do not silently select a rule.

## Gather evidence

Inspect implementation files, design tokens, UI copy, configuration, assets, and test source.
Trace source declarations and control flow to identify causes and locate fixes.
Treat stored screenshots and test results as supporting artifacts. State their origin and limits.

Select source checks according to the affected experience and applicable skills:

- Trace primary tasks, action hierarchy, feedback, error prevention, and recovery through the code.
- Inspect code for empty, loading, success, error, disabled, selected, hover, focus, pressed, and drag states.
- Inspect accessible names, semantics, keyboard handlers, focus management, and assistive input support.
- Inspect breakpoints, text scaling, reflow rules, content limits, theme tokens, and language direction.
- Compare declared contrast values, dimensions, spacing, typography, and motion against applicable thresholds.
- Check copy for consequences, clarity, grouping, grammar, capitalization, and localization risks.
- Check source consistency across affected screens and shared components.

Record file locations, relevant declarations, code paths, and expected behavior.
Separate source evidence from inferred runtime behavior. State uncertainty when evidence is incomplete.
Mark criteria that need rendered output or live interaction as outside source verification.
These limits alone do not prevent a completed source review or require a runtime review.
Do not claim that source inspection proves rendered usability, device behavior, or screen reader behavior.
Do not infer user satisfaction or research outcomes from source inspection.

## Classify findings

Use these finding types:

- **Violation:** Evidence contradicts an applicable rule under its stated conditions.
- **Improvement:** Guidance supports a better result without establishing a definite violation.
- **Unverified concern:** A plausible issue needs additional evidence before classification.

Assign severity by user impact, scope, frequency, and available recovery:

- **Critical:** Blocks an essential task for affected users without a practical recovery path.
- **Major:** Substantially impairs task completion, access, comprehension, or error recovery.
- **Minor:** Creates limited friction or inconsistency while tasks remain achievable.

Keep severity separate from finding type and evidence confidence.
Explain release blockers in the task context. Do not make every guideline deviation a release blocker.
Consolidate repeated instances with the same cause. Include representative locations and affected scope.
In change review, distinguish introduced issues, worsened issues, and relevant pre-existing issues.
Keep unrelated pre-existing issues outside the change verdict.

## Produce the report

Lead with the source review judgment and the most consequential findings.
Use **meets reviewed criteria**, **needs changes**, or **insufficient evidence** for the overall judgment.
Limit that judgment to the declared scope and verified evidence. Do not claim formal certification or complete Material compliance.
Avoid numerical scores unless the user supplies or requests a defined scoring rubric.

Include these report sections:

1. **Scope and evidence:** Review mode, comparison base, files, screens, code paths, source checks, assumptions, and limits.
2. **Findings:** Order by severity. Separate violations, improvements, and unverified concerns clearly.
3. **Coverage:** Account for every discovered skill, including exclusions and missing evidence.
4. **Area assessment:** Evaluate usability, accessibility, adaptive layout, visual styles, component behavior, and writing/localization.
5. **Fix priorities:** Identify blockers, the next improvements, and the checks needed after fixes.

For each area, use **meets reviewed criteria**, **needs changes**, **not verified**, or **not applicable**.
Support each assessment with findings or checks. State partial verification when an area has mixed coverage.
If no findings exist, say so and retain the evidence and coverage limits.

### Finding contract

Give every finding a stable ID such as `M3-001` and include:

- **Title, type, and severity.**
- **Application location:** File and line when available, plus the screen, component, or journey.
- **Evidence:** File and line references, declarations or code paths, expected behavior, and applicable conditions or source values.
- **User impact:** Explain the practical consequence.
- **Rule:** State the applicable requirement or recommendation and its conditions.
- **Skill reference:** Link the exact skill file and name the section. Add a line reference when available.
- **Source reference:** Link the original Material page cited by that skill. Include the relevant source-map section when needed.
- **Fix direction:** Describe the intended result and any constraints without prescribing unsupported details.
- **Verification:** Describe the source changes and inspections that confirm the fix. State any remaining runtime uncertainty separately.
- **Confidence and gaps:** Identify inferences or missing evidence when relevant.

Use resolvable file links for the current environment. Preserve skill names and section titles for portable handoffs.
Cite only rules and sources you have inspected. Never invent quotations, URLs, section names, or line numbers.
When the skill lacks an original source, cite the local rule and disclose the source gap.
State that the review uses the local skill snapshot. Do not require external access.

## Dedicated review agent handoff

When the user requests a dedicated review agent, give that agent this skill and the review scope.
Include the application location, comparison base, source-only scope, and relevant product constraints when available.
Use a dedicated agent only when delegation is available and authorized.
If delegation is unavailable, perform the same review directly and disclose that limit.
Do not require delegation for ordinary use of this skill.
Return the report to the requesting agent. Preserve finding IDs and references for the fixing agent.
After fixes, inspect the changed source and affected code paths. State any remaining source verification gaps.
