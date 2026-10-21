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
| Verification | Separately claimed corrected Phase 7 suite remains unverified | Corrected source, contract, and original test evidence required |
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

# EKA AI Brain V6 — Engineering Milestone Update

**Date:** October 21, 2026
**Organization:** EKA V6 SYSTEMS LLC
**Project:** Experimental adaptive event-processing architecture for resource-constrained FPGA systems
**Target platform:** Lattice iCE40UP5K / UPduino 3.1

## Project overview

EKA AI Brain V6 is a research-stage, Verilog-based event-processing project exploring change detection, adaptive thresholds, and auditable telemetry on resource-constrained FPGA hardware. Separate experimental configurations must be evaluated against their own source, workload, and implementation records.

This update summarizes saved engineering results. **RTL simulation, implementation-tool estimates, and physical-board measurements are separate evidence categories.** No new physical performance result is announced in this update.

## Engineering milestones

| Area | Documented result | Evidence category |
|---|---|---|
| V6 optimized functional tests | Saved top-level test log reports `ALL V6-OPT TOP LEVEL TESTS PASSED` | RTL simulation |
| Extended V6 stress test | 10,000,000 simulated samples; zero threshold-range violations | RTL simulation |
| Phase 9 metrics workload | 30,000,000 admitted simulated inputs; 21,980,390 detected events; zero instrumented threshold-range errors; matching Verilator and Icarus results recorded | RTL simulation |
| Phase 6C.1 dense healthy workload | 631 of 631 labeled events detected; zero input drops; 238 event records delivered in that test | RTL simulation; workload-specific |
| Phase 7 FPGA implementation | 758 of 5,280 logic cells; nominal 12 MHz target passed; final estimated Fmax 34.28 MHz | Historical synthesis and place-and-route |
| Phase 8 timing estimate | Estimated Fmax 31.54 MHz for its saved build | Historical place-and-route estimate |
| Phase 9 FPGA implementation | iCE40UP5K SG48 build; 757 of 5,280 logic cells; nominal 12 MHz timing target passed | Synthesis and place-and-route |
| Phase 9 timing estimate | Routed estimated maximum frequency approximately 33.07 MHz | Implementation-tool estimate; not measured board frequency |
| Historical V6 timing recheck | A separate saved implementation produced a 14.97 ns path estimate, corresponding to 66.78 MHz | Historical timing-tool estimate; different build and method |
| Engineering preservation | Original engineering artifacts preserved with a checksum inventory | Documentation and reproducibility |

The Phase 9 figures describe the verified metrics configuration, not proof that a separately claimed corrected adaptive architecture has been integrated. The separate Phase 7 correction package and its claimed 13-case suite remain unverified in the available engineering review.

The 631/631 recall result applies only to the documented healthy workload; it is not a general field-accuracy or fault-tolerance claim. Label detection, input drops, and transmitted record counts are different measures. Separate fault-injection tests exposed limitations under some outage conditions. Zero threshold-range errors means that particular instrumented check passed; it does not establish the absence of every possible design defect.

The timing estimates describe different implementation records and tools and should not be presented as a before/after performance comparison or as demonstrated operating frequencies.

## Inputs and clock cycles are different measures

| Measure | Meaning | Status in this update |
|---|---|---|
| Admitted simulated inputs | Samples accepted by the Phase 9 RTL simulation workload | 30,000,000 |
| Simulated FPGA clock cycles | Clock edges advanced by the simulator, including startup, workload, drain, stalls if any, and telemetry | No separately established end-to-end total is asserted here; the admitted-input counter is not that total |
| Physically measured clock cycles | Cycles independently counted or captured from the running physical FPGA, using a stated observation boundary | Not independently established for the 30-million-input run |

Nominal 12 MHz is a build/configuration target. The 34.28, 31.54, 33.07, and 66.78 MHz values are tool estimates for separate builds, not measured physical clocks or evidence of a speedup.

## Current verification boundary

Saved records establish RTL simulation results and successful synthesis and routing for documented configurations. They do not yet independently establish:

- A repeatable physical UPduino run with independently captured and validated 30-million-input counters.
- Measured physical throughput, clock frequency, or end-to-end latency matching a simulation estimate.
- Measured dynamic-power or energy savings against a controlled baseline.
- Independent third-party validation or production readiness.

A board connection, programming verification, or completion LED alone does not establish the numerical result of a hardware workload.

## Next verification milestone

The next target is a repeatable physical UPduino 3.1 test that **admits 30,000,000 input samples**. Total elapsed FPGA clock cycles—including startup, stalls if any, pipeline drain, and telemetry—will be counted or measured separately; they must not be assumed equal to admitted inputs.

The acceptance record will identify exact RTL and bitstream hashes, board identity, clock configuration and measured timing method, workload definition, raw independently captured output, counter values, error-check meaning, and repeated-run results. The current Phase 9 simulation reference is 30,000,000 admitted inputs, 21,980,390 events, and zero threshold-range errors. Hardware acceptance also requires a valid telemetry frame and its integrity checks.

Power and energy claims require a separate documented measurement boundary, calibrated or characterized instrumentation, matched workload, idle and active observations, and an appropriate baseline. They will be reported only after those experiments are completed.

## Publication and intellectual property

This high-level update excludes the complete engineering archive, proprietary RTL and patterns, bitstreams, private datasets, and raw test artifacts. Additional source or evidence publication requires project-owner review. Publication of aggregate metrics is not a release of rights to the underlying technology.

**Organization:** EKA V6 SYSTEMS LLC
**Portfolio:** https://singhbagnalia.github.io/eka-v6-portfolio/
**GitHub:** https://github.com/singhbagnalia
**Tagline:** *Building adaptive, auditable computing systems.*
