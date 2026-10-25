# REA Replica

[Português (Brasil)](README.pt-BR.md)

REA Replica is a Codex skill that combines authorized REA artifact analysis with the Replica clean-room application reconstruction workflow.

## What it does

- Routes public product research and user-visible behavior through `replica-recon`.
- Uses `reverse-engineer-anything` when a conclusion requires authorized binary, package, firmware, managed-code, JavaScript/Electron, runtime, or version-comparison evidence.
- Separates observations, inferences, and unknowns.
- Turns evidence into independent product requirements, interface contracts, and testable outcomes.
- Coordinates architecture, design, implementation, backend work, testing, branding, launch, and deployment through the installed `replica-*` skills.
- Prevents proprietary source, decompiled code, private APIs, credentials, assets, branding, and distinctive copy from entering the rebuilt product.

## Language support

The skill responds in the user's language and explicitly supports English (US) and Portuguese (Brazil). Tool names, skill names, file paths, Evidence IDs, API identifiers, and code remain unchanged.

## Requirements

Install and configure:

- `reverse-engineer-anything`
- The Replica skill collection (`replica-*`)
- REA tools when artifact analysis is required

This repository orchestrates those dependencies; it does not bundle them.

## Installation

Clone the repository into the Codex skills directory using the folder name `rea-replica`:

```bash
git clone https://github.com/wsavliscrds-art/Rea-replica.git ~/.codex/skills/rea-replica
```

On Windows PowerShell:

```powershell
git clone https://github.com/wsavliscrds-art/Rea-replica.git "$env:USERPROFILE\.codex\skills\rea-replica"
```

Start a new Codex message after installation.

## Usage

```text
Use $rea-replica to analyze this application and plan a clean-room reconstruction.
```

The skill can also be selected automatically when the request matches its description.

## Responsible use

Only analyze artifacts you own, are authorized to inspect, or may legitimately study for interoperability, compatibility, archival, or security-research purposes. Never bypass authentication, paywalls, licensing, or access controls.

The rebuilt product must use fresh implementation code and original branding and assets. REA evidence describes behavior and constraints; it is not source code for the replacement.

## License

MIT. See [LICENSE](LICENSE).
