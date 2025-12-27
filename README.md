# Quantum Error Correction Resilient Against Atom Loss

A research project investigating quantum error correction (QEC) strategies specifically designed for neutral-atom quantum processors to mitigate atom loss errors.

## Table of Contents

- [About the Project](#about-the-project)
- [Research Objectives](#research-objectives)
- [Methodology](#methodology)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Project Timeline](#project-timeline)
- [Expected Results](#expected-results)
- [Author](#author)
- [License](#license)
- [References](#references)

## About the Project

Neutral-atom quantum processors, based on optically trapped atoms and Rydberg interactions, combine long coherence times with flexible, reconfigurable connectivity and have shown promise for tasks such as optimization and quantum simulation. However, practical implementations suffer from atom loss (qubit loss) arising from finite trap lifetimes and technical noise, which directly reduces the effective code distance of error-correcting encodings and undermines long-duration quantum computation.

This project focuses on developing and evaluating quantum error-correction strategies that are specifically resilient to atom loss in neutral-atom arrays. Building on recent approaches — including:

- **Teleportation-based loss-detection** and unitary (LDU) replacement schemes
- **Gauge-stabilizer constructions** for deterministic supercheck outcomes
- **Belief-propagation plus ordered-statistics decoding (BP+OSD)** techniques for qLDPC codes

The goal is to identify combinations of code structure, loss-aware encoding/repair, and decoding that maximize logical fidelity in the presence of realistic loss channels.

## Research Objectives

This project aims to assess and compare the performance of modifications to existing QEC strategies under qubit loss (QL) errors. Specifically, the project seeks to:

1. **Review existing QEC protocols** for mitigating QL errors to identify strategies that can be applied to neutral atom qubits
2. **Implement relevant QEC protocols** for a comparative analysis of their performance under QL errors
3. **Construct a more robust QEC protocol** based on the advantageous features identified in the comparative analysis

## Methodology

Quantum error correction involves protecting logical qubit information from quantum errors by encoding it among multiple physical qubits. QEC protocols generally consist of the following elements:

### Encoding Procedures
Mapping logical qubits into entangled states of multiple physical qubits to create redundancy that allows error detection and correction. Examples include:
- Surface codes
- Color codes
- Low-density parity-check (LDPC) codes

### Decoding Procedures (Error Detection & Correction)
Measuring syndromes to identify errors and applying corrective operations to restore the logical qubit state. Examples include:
- Minimum-weight perfect matching (MWPM)
- Belief propagation (BP)
- Machine learning-based decoders

This study will focus on modifying and assessing these elements of relevant QEC strategies with mathematical models and computational simulations to propose a QEC protocol suitable for neutral atom arrays under atom loss.

## Project Structure

```
QEC-for-neutral-atom-arrays/
├── Decoders/              # Error decoding implementations
├── Encoders/              # Error encoding implementations
│   └── Test.ipynb         # Testing notebook for encoders
├── Project Docs/          # Project documentation
│   ├── Dissertation/      # Final dissertation documents
│   ├── Literature Review/ # Literature review documents
│   ├── Progress Report/   # Progress report documents
│   └── Project Plan/      # Initial project plan
├── LICENSE
├── README.md
└── VERSIONING.md
```

## Getting Started

### Prerequisites

This project uses computational simulations and requires:
- Python (version TBD based on implementation)
- Jupyter Notebook for running test implementations
- High-performance computing resources (available at UCL)
- Quantum simulation libraries (to be specified during implementation)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/QEC-for-neutral-atom-arrays.git

# Navigate to the project directory
cd QEC-for-neutral-atom-arrays

# Install dependencies (to be updated)
# pip install -r requirements.txt
```

## Project Timeline

The project is divided into three main phases:

### Phase 1: Literature Review (November 2025 - January 2026)
Learning key concepts relevant to QEC, neutral atom quantum computing, and qubit loss errors. Conducting a comprehensive review focusing on:
- QEC constraints specific to neutral atom arrays
- State-of-the-art QEC protocols for QL-mitigation
- Key factors for measuring QL-mitigation performance

### Phase 2: Comparative Analysis (February - April 2026)
Implementation and comparative analysis of relevant QEC protocols:
- Implementing selected QEC protocols using suitable programming languages and simulation tools
- Simulating performance under various QL error models relevant to neutral atom arrays
- Analyzing results to identify strengths and weaknesses of each protocol

### Phase 3: Algorithm Development and Analysis (May - End of Project)
Investigating modifications to improve QL-mitigation performance:
- Developing enhanced QEC methods
- Synthesizing results
- Preparing final project deliverables and presentation

## Expected Results

This study is expected to yield the following outcomes:

- Improved understanding of the performance of existing QEC protocols under qubit loss errors in neutral atom arrays
- Identification of key factors that influence the effectiveness of QEC protocols in mitigating qubit loss
- Development of a more robust QEC protocol tailored for neutral atom quantum computers that effectively mitigates qubit loss errors
- Comprehensive comparative analysis of various QEC protocols, providing insights into their strengths and weaknesses in the context of qubit loss

## Risk Assessment

This study employs a computational approach, minimizing physical risks. Potential challenges include:

- **Computational Resource Limitations**: Mitigated by utilizing high-performance computing resources at UCL and optimizing code for efficiency
- **Algorithm Complexity**: Addressed by breaking down algorithms into manageable components and seeking expert guidance
- **Time Management**: Managed through detailed scheduling and milestone tracking

## Author

**Adeniyi Osinowo**  
Department of Physics and Astronomy  
University College London  
Gower Street, London, WC1E 6BT, UK

## License

See [LICENSE](LICENSE) file for details.

## References

Key references for this project include:
- Perrin et al. (2025) - Teleportation-based loss-detection and unitary replacement schemes
- Auger et al. (2017) - Gauge-stabilizer constructions
- Roffe (2020) - Belief-propagation plus ordered-statistics decoding techniques for qLDPC codes

For a complete list of references, see the project documentation in [Project Docs](Project%20Docs/).

