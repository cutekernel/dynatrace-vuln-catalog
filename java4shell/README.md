# Java4Shell dashboard

Dynatrace dashboard for assessing Java runtime exposure to **Java4Shell (CVE-2026-114938)**.

## Contents

- [`java4shell-cve-2026-114938.json`](./java4shell-cve-2026-114938.json) — dashboard definition.

## Dashboard coverage

The dashboard queries detected Java process-group instances and provides:

- Affected, not-affected, and unknown-version process counts.
- Host and Java-version filters.
- Affected processes grouped by host and version.
- Java support status, including end-of-life and approaching end-of-life runtimes.
- Fixed-release guidance and a mitigation note for delayed patching.

## Import

Import the JSON definition into a Dynatrace environment with access to:

- `dt.entity.process_group_instance`
- `dt.entity.host`
- Java software-technology metadata

Review the version ranges, fixed releases, and mitigation guidance against the current vendor advisory before using the dashboard operationally.
