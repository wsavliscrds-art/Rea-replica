---
name: rea-replica
description: Combine REA artifact analysis with the Replica workflow to understand an app and rebuild an original, clean-room alternative. Use when the user wants evidence-backed reverse engineering followed by recon, architecture, design, implementation, testing, parity analysis, branding, launch, or deployment. Skip for ordinary source-repository analysis or when only one narrow Replica stage is requested.
---

# REA Replica

Orchestrate the installed `reverse-engineer-anything` and `replica-*` skills. Do not duplicate their detailed procedures. Load and follow only the skills relevant to the current stage.

## Language

Respond in the language used by the user. Support both English (US) and Portuguese (Brazil) terminology and examples. Keep tool names, skill names, file paths, Evidence IDs, API identifiers, and code unchanged. When the user mixes languages, prefer the language of the latest substantive request unless they ask for bilingual output.

## Establish scope and authority

Identify the target, platform, requested product slice, and intended outcome. Before using REA on a shipped artifact or runtime, establish that the user owns the target, is authorized to analyze it, or has a legitimate interoperability, security-research, archival, or compatibility purpose. If authority is unclear and technical inspection would materially exceed public observation, ask before continuing.

Public pages, documentation, app-store listings, screenshots, and the user's own normal account can proceed through `replica-recon`. Never bypass authentication, paywalls, access controls, licensing, or platform protections.

## Choose the evidence route

- Use ordinary repository tools for source code the user supplied. Do not invoke REA merely because the project is an application.
- Use `replica-recon` for public-product research, user-visible flows, screens, states, components, and feature inventory.
- Use `reverse-engineer-anything` when a conclusion depends on an authorized binary, package, Electron/JavaScript artifact, firmware image, managed assembly, passive runtime observation, or version comparison.
- When both routes apply, maintain one finding ledger. Label every entry as observed, inferred, or unknown; include REA Evidence IDs for technical findings and URLs or screenshot identifiers for public findings.

Start with the smallest useful inspection. Do not execute, fuzz, stress, or instrument a third-party production target unless the user explicitly requests it, has authority, and the chosen REA workflow supports it safely. Passive evidence does not prove runtime behavior.

## Preserve a clean-room boundary

Translate evidence into product behavior, interface contracts, data concepts, constraints, and testable outcomes. Do not copy or ship original source, decompiled code, proprietary assets, trademarks, licensed fonts, secret material, credentials, private API endpoints, or distinctive product copy.

Keep original screenshots and technical evidence as references only. Write implementation code fresh. Prefer official public APIs and the user's own credentials for integrations. When uncertain whether a detail is functional behavior or protected implementation expression, describe the requirement at a higher level and choose an independent design.

## Route the reconstruction

Use the existing Replica artifacts under `replica/` so every stage can reuse prior work:

1. `replica-recon` creates the screen, flow, component, inferred-data, and feature map. Enrich it with authorized REA conclusions without placing proprietary code in the map.
2. `replica-architect` turns the map into an independent stack, schema, API, and build order.
3. `replica-design` specifies original design tokens and components; `replica-brand` removes target branding and creates the user's identity.
4. `replica-build` implements a thin vertical slice, then the remaining screens and states. Use `replica-backend` for auth, data, payments, jobs, email, and official integrations.
5. `replica-test` tests only the user's clone. Use `replica-diff` for feature, layout, and behavior parity without treating color or branding differences as defects.
6. Use `replica-entrepreneur`, `replica-launch`, and `replica-deploy` only when the user asks to commercialize or ship the result.

Do not force the entire sequence for a narrow request. Resume from existing valid artifacts, record gaps, and recommend the next stage rather than silently expanding scope.

## Deliver the result

Summarize the target and authorization basis, evidence used, conclusions with confidence, remaining unknowns, clean-room exclusions, Replica artifacts created or updated, and the next recommended stage. Keep technical evidence separate from implementation decisions. Close any REA session opened for the investigation when finished.
