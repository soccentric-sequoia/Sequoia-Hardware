# Sequoia-Hardware

## Project Summary

Sequoia-Hardware is the hardware-inventory leaf for the Sequoia project. The current repository
contains a README and ignore configuration but no source files, build manifest, board manifest,
hardware description, executable test, or deployment script. Consequently, there is not enough
repository evidence to describe a hardware driver, board layout, peripheral contract, or supported
device beyond the project name. This README records that limitation directly so downstream
documentation does not confuse the repository placeholder with the active implementation in
Sequoia-HAL or the image recipes in Sequoia-OS.

The intended role can be inferred only at the ecosystem level: physical board facts may eventually
be used by the HAL, configuration manifests, operating system image, and fleet services. Those
relationships are not implemented in this repository today. There is no setup or usage command to
validate, and no test command is declared. A future contribution should establish the board
identity, revisioned hardware artifacts, ownership of generated files, and a small validation path
before claiming support. Until then, feature status is `unknown` or `planned`, not implemented.
Manual review is left on every row as requested and must be performed against the actual target
hardware once this repository gains content.

The absence of files is itself an important scan result: there is no evidence of a board identifier,
revision policy, physical interface ownership, or release artifact in this leaf. Those facts may
exist in private planning material or in the HAL and OS repositories, but cannot be attributed to
Sequoia-Hardware without checked-in references. The inventory is a handoff list for the next
implementation pass, not a specification of supported hardware.

## Feature Inventory

| # | Name / Description | Implemented? | Test Coverage? | Manual Test |
| --- | --- | --- | --- | --- |
|   1 | Repository placeholder and project identity  | Implemented  | No automated tests found   | [ ] Manual verification required |
|   2 | Sequoia board specification                  | Unknown      | No source/spec files found | [ ] Manual verification required |
|   3 | Hardware revision and component inventory    | Planned      | No tests found             | [ ] Manual verification required |
|   4 | Peripheral pinout and electrical constraints | Planned      | No tests found             | [ ] Manual verification required |
|   5 | Schematics, CAD, or production artifacts     | Unknown      | No artifacts found         | [ ] Manual verification required |
|   6 | Interface contract consumed by Sequoia-HAL   | Unknown      | No contract tests found    | [ ] Manual verification required |
|   7 | Setup, provisioning, and bring-up procedure  | Planned      | No command declared        | [ ] Manual verification required |
|   8 | Hardware acceptance test suite               | Planned      | No test files found        | [ ] Manual verification required |

## Current Limitation

There is no build or test command in this repository. Consult Sequoia-HAL for implemented hardware
access and Sequoia-OS for image-level integration.
