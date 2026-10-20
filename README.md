# EKA V6 SYSTEMS LLC
### Adaptive Edge AI · FPGA Research · Auditable Decision Intelligence

**Research and development portfolio | October 2026**

EKA V6 SYSTEMS LLC is developing experimental adaptive, event-driven computing technology and offline AI software. Our work explores resource-constrained FPGA processing, reproducible verification, and human-governed AI workflows.

> **Research status:** The technical milestones below are project-reported results. Public source artifacts and independently verified hardware benchmarks have not yet been published. Simulation results are not equivalent to measured physical hardware performance.

## Featured research: EKA AI Brain V6

An experimental FPGA-oriented adaptive event processing architecture, developed with Verilog and tested using open-source digital design tools.

**Reported engineering milestones**

| Area | Project-reported milestone | Evidence to publish after review |
|---|---|---|
| RTL simulation | Top-level V6 optimized testbench passed | Redacted simulation log and testbench summary |
| Stress testing | Up to 10 million simulated samples; no threshold-range violations reported | Test configuration, seed, tool versions and results |
| Accuracy testing | 500,000-sample run reported zero count/event/range errors | Oracle specification and aggregate report |
| Verification | Phase 7 verification: 13/13 test cases reported passing | Reproducible verification summary |
| Timing | Synthesis/timing reports generated for iCE40UP5K target | Constraints and labeled estimated Fmax report |
| Hardware | UPduino 3.1 / Lattice iCE40UP5K development target | Board test report and instrumented measurements when available |

**Toolchain:** Verilog · Icarus Verilog · Yosys · Lattice iCE40UP5K · UPduino 3.1 · Python

### Engineering questions
- How can adaptive event detection reduce unnecessary processing on resource-limited devices?
- How do threshold policies behave under quiet, noisy, and bursty workloads?
- How can we make RTL verification and benchmark claims independently reproducible?

## EKA AI-V6: Offline assistant prototype

A separate experimental desktop application exploring local AI interactions and offline document access.

**Prototype stack:** Python · HTML · SQLite · Ollama · local models (Gemma 3 4B, Llama 3.2 3B)

**Development directions:** searchable offline library, private local chat, secure mobile access, and user-controlled data handling. These are prototype goals, not claims of production readiness or App Store availability.

## Research direction: Auditable Decision Intelligence

We are exploring a schema-driven decision workflow that can organize objectives, options, constraints, evidence, assumptions, risks, and bias checks into reviewable Decision Packages.

A proposed demonstration would compare synthetic ground-vehicle computing alternatives, preserve evidence provenance and human approvals, and show how updated assumptions change a recommendation. **This is a proposed research direction, not an implemented or validated product capability.**

## Development roadmap

1. Publish sanitized, reproducible RTL verification reports and tool versions.
2. Record physical FPGA power, timing, and functional measurements using documented methods.
3. Build a decision-schema prototype with deterministic scoring, provenance, and human review.
4. Validate privacy/security for local AI and mobile connectivity.
5. Prepare research collaborations and technical demonstrations.

## Intellectual property and responsible disclosure

This repository is a **public portfolio only**. It does not contain proprietary RTL, confidential datasets, unpublished invention details, credentials, or unrestricted rights to EKA V6 technology. No patent, government endorsement, award, certification, or performance guarantee is implied.

**Organization:** EKA V6 SYSTEMS LLC  
**Portfolio owner:** Mangal Singh  
**Contact:** Add a dedicated public business contact address after reviewing privacy settings.

---
*Evidence-first engineering. Reproducible research. Human-controlled AI.*
