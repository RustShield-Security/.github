# RustShield Security

RustShield Security builds security-assessment tooling for MAVLink-based UAV and robotics laboratory workflows.

Our current public project is RustShield Gateway, a Rust-based MAVLink security gateway technical preview for controlled SITL/laboratory validation.

## Current Public Project

### RustShield Gateway

RustShield Gateway sits between a Ground Control Station and a MAVLink vehicle or simulator. It observes MAVLink traffic, applies selected semantic command policies, and produces logs, metrics and public evidence summaries for security review.

Public release:

https://github.com/RustShield-Security/rustshield-gateway/releases/tag/v0.1.0-lab-preview

Repository:

https://github.com/RustShield-Security/rustshield-gateway

## Focus Areas

- MAVLink security assessment.
- Critical and high-risk command policy.
- MAVLink signing observe/audit/enforce laboratory paths.
- Shadow enforcement for non-blocking impact analysis.
- Read-only observability and evidence capture.
- Controlled SITL and laboratory validation workflows.

## What We Do Not Claim

- No certified flight readiness.
- No real UAV operation validation.
- No hardware/radio validation in the public preview.
- No complete MAVLink security coverage.
- No replacement for autopilot hardening, key management or network segmentation.

## Commercial / Lab Pilots

RustShield Security is open to assessment, laboratory pilot and partner-integration discussions with UAV integrators, drone security labs, robotics security teams and critical-infrastructure inspection groups.

Contact:

rustshield.security@proton.me
