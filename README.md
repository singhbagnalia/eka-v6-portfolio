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

EKA AI Brain V6 — Engineering Milestone Update
Date: October 21, 2026
Organization: EKA V6 SYSTEMS LLC
Project: Experimental adaptive event-processing architecture for resource-constrained FPGA systems
Target platform: Lattice iCE40UP5K / UPduino 3.1

Project overview
EKA AI Brain V6 is a research-stage, Verilog-based adaptive event-processing system. Its architecture includes an optimized change detector, adaptive threshold logic, and telemetry mechanisms intended to support measurable, auditable processing of event streams on resource-constrained hardware.

This update summarizes results contained in the project's engineering records. Simulation results, implementation-tool estimates, and physical-board measurements are separate categories of evidence.

Engineering milestones
Area	Documented result	Evidence category
Top-level V6 functional tests	Test log reports ALL V6-OPT TOP LEVEL TESTS PASSED	RTL simulation
Extended V6 stress test	10,000,000 simulated samples; zero threshold-range violations	RTL simulation
Phase 9 metrics workload	30,000,000 simulated input samples; 21,980,390 detected events; zero threshold-range errors	RTL simulation
Phase 6C.1 dense workload	631/631 labeled events detected (100% recall); zero dropped frames in the specified healthy test	RTL simulation
Phase 7 FPGA implementation	iCE40UP5K SG48 build; 757 / 5,280 logic cells; 12 MHz timing target passed	Synthesis / place-and-route
Phase 7 timing estimate	Estimated Fmax: 31.54 MHz	Implementation-tool estimate
Separate V6 timing report	14.97 ns critical path; estimated 66.78 MHz	Timing-tool estimate for a different build
Engineering preservation	Consolidated archive with original engineering artifacts and checksum inventory	Documentation / reproducibility
Interpretation notes: The 30-million-input result is from simulation and does not establish 30 million physical FPGA clock cycles. The two timing figures describe different implementation reports and should not be presented as a direct before/after performance comparison. The dense-workload recall figure applies to the documented test conditions; separate fault-injection cases exposed limitations under some outage scenarios.

Current verification boundary
The engineering records demonstrate extensive RTL simulation and successful FPGA synthesis and routing for documented configurations. They do not yet independently establish:

A completed, instrumented 30,000,000-clock-cycle run on a physical UPduino 3.1 board.
Physical throughput matching the simulation workloads.
Measured dynamic-power or energy savings against a controlled baseline.
Independent third-party validation or production readiness.
Next verification milestone
The next target is a physical UPduino 3.1 test with 30,000,000 actual FPGA clock cycles. The proposed acceptance record will include the exact RTL/bitstream hashes, board and clock configuration, workload definition, start/end or completion evidence, output counters, error checks, and repeatability results. Input samples and FPGA clock cycles will be reported separately.

Publication and intellectual-property note
This public milestone report is a high-level summary. The complete engineering archive, detailed RTL, proprietary patterns, and full test data are not included in this public release. Publication of any additional source or artifacts should be reviewed by the project owner before committing to a public repository.

Organization: EKA V6 SYSTEMS LLC
Portfolio: https://singhbagnalia.github.io/eka-v6-portfolio/
GitHub: https://github.com/singhbagnalia
Tagline: Building adaptive, auditable computing systems.

