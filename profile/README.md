# RustShield Security

RustShield Security builds protocol-aware security gateway proofs of concept for cyber-physical and critical-infrastructure laboratory workflows.

Our public work focuses on **stateful semantic shielding**: transparent gateways that inspect legacy or safety-critical protocol traffic, keep a small view of observed system state, apply explicit command policies, and produce reproducible lab evidence for security review.

## Public Projects

### RustShield Gateway

RustShield Gateway is a Rust-based MAVLink security gateway technical preview for controlled UAV and robotics SITL/laboratory validation.

It sits between a Ground Control Station and a MAVLink vehicle or simulator. It observes MAVLink traffic, applies selected semantic command policies, and produces logs, metrics, and public evidence summaries for security review.

Repository:

https://github.com/RustShield-Security/rustshield-gateway

Public release:

https://github.com/RustShield-Security/rustshield-gateway/releases/tag/v0.1.0-lab-preview

### RustShield Modbus Gateway

RustShield Modbus Gateway is a Rust proof of concept for stateful semantic filtering of Modbus TCP traffic in local OT/ICS lab simulations.

It runs as a transparent TCP proxy between a simulated SCADA/client and a simulated PLC. It parses Modbus TCP frames, observes read responses, keeps an in-memory view of process state, and blocks a protected `Write Single Coil` command when the observed state is unknown, stale, or unsafe.

Repository:

https://github.com/RustShield-Security/rustshield-modbus

## Focus Areas

- Protocol-aware security gateways for cyber-physical systems.
- Stateful semantic command policy for high-risk operations.
- MAVLink UAV and robotics laboratory validation.
- Modbus TCP OT/ICS laboratory simulation.
- Fail-safe handling for unknown, stale, malformed, or unsupported states.
- Read-only observability, metrics, logs, and reproducible evidence capture.
- Controlled local simulation before any discussion of real hardware or production networks.

## What We Do Not Claim

- No certified flight readiness.
- No production OT security or safety certification.
- No real UAV, PLC, plant network, radio, or hardware validation in the public previews.
- No complete coverage of MAVLink, Modbus, or all cyber-physical attack paths.
- No cryptographic authentication claim for the Modbus TCP PoC.
- No replacement for autopilot hardening, PLC/SCADA hardening, key management, network segmentation, access control, or OT risk governance.

## Commercial / Lab Pilots

RustShield Security is open to assessment, laboratory pilot, and partner-integration discussions with UAV integrators, drone security labs, robotics security teams, OT/ICS security teams, and critical-infrastructure inspection groups.

Contact:

rustshield.security@proton.me
