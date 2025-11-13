---
title: "Cornell Notes - Quantum Technology"
date: 2025-11-12 09:00:00 -0800
categories: [Notes, Quantum Computing]
tags: [quantum-computing, cornell-notes, ibm, quantum-volume, qubits]
permalink: /posts/ibm-quantum-technology/
---

**Course:** Introduction to Quantum Computing by IBM Quantum Learning

**Section:** Quantum Technology

---

## Cornell Notes

**What does IBM have right now?**
- IBM has the LARGEST fleet of quantum computers in the world!
- Each one has at least 127 qubits
- They all use something called superconducting transmon qubits
- IBM combines these powerful computers with Qiskit so people can actually USE quantum computers to solve real problems

**What are the different types of qubits?**
Three Types of Qubits:
1. **Superconducting Qubits** (IBM's type): Made from special materials on silicon. Need EXTREMELY cold temps (near absolute zero). Like ice that conducts electricity!
2. **Photonic Qubits:** Made from particles of light (photons)
3. **Trapped-Ion Qubits:** Information stored in charged atoms held in a trap

All three work, but superconducting is what IBM uses!

**What is IBM Quantum Platform?**
All-in-One Quantum Workspace - It's like a Swiss Army knife for quantum computing. All tools in one place:
- Home page: Get your API keys and see your jobs
- Documentation: Instructions and reference guides
- Learning: Courses and teaching materials
- Circuit Composer: Visual tool to build quantum circuits

**What is Qiskit Runtime?**
- A special container system that runs quantum programs
- Imagine a GPU for graphics - Qiskit Runtime is like a QPU (quantum processing unit) for quantum!
- It handles all the behind-the-scenes stuff (job scheduling, data transfer) so you can focus on YOUR code
- Makes quantum computing way faster and easier!

**What is Circuit Knitting?**
- A tool that takes HUGE quantum circuits (too big for current computers) and chops them into smaller circuits that current quantum computers CAN handle
- Classical computers help piece it all back together
- Like cutting a pizza into slices but still getting the whole pizza!

**What is Quantum Serverless?**
- A system that connects regular computers (classical) with quantum computers automatically
- It's like having a personal assistant that figures out what resources you need and gets them for you
- You just write the code!

**What is Quantum Volume?**
The Big Picture of Quantum Computer Quality - Quantum Volume is ONE NUMBER that tells you how good a quantum computer is.

It combines:
- Number of qubits (space)
- Error rate (time to explore)
- Circuit connectivity
- Other quality factors

Higher Quantum Volume = Better Computer! Counting qubits alone is misleading!

## The NYC Tourist Analogy for Quantum Volume

**The Analogy:** Imagine a tourist trying to explore New York City in a limited amount of time.

**Scenario 1: 1 Day vs. 3 Days**
- Tourist wants to see ALL of NYC (the "space")
- With 1 day? Not possible. Doesn't get enough volume.
- With 3 days? Can hit all the top spots. Gets the volume!
- **Lesson:** More TIME lets you explore more SPACE.
- **In Quantum Terms:** Lower ERROR RATE = more TIME to run calculations = explore bigger quantum space.

**Scenario 2: More Time, Same City**
- Tourist has 3 days but stays in NYC
- NYC is fully explored
- More time doesn't help - already saw everything!
- Tourist volume stays the same
- **Lesson:** Extra time without more space doesn't help.
- **In Quantum Terms:** Decreasing errors without adding more qubits doesn't improve Quantum Volume. You need BOTH!

**Scenario 3: Same Time, Bigger Area**
- Tourist has 3 days but now tries NYC AND Long Island
- Too much area for 3 days!
- Can't explore everything
- Tourist volume stays at "NYC level"
- **Lesson:** More space without more time doesn't help.
- **In Quantum Terms:** Adding qubits without lowering errors doesn't improve Quantum Volume. You need BOTH!

**The Key Insight:**
To get a BETTER quantum computer (higher Quantum Volume), you MUST:
- Increase the number of qubits (bigger space) AND
- Decrease the error rate (more time to explore)

Both need to improve together! It's not one or the other - it's BOTH!

## Performance Metrics Comparison

| Metric | What It Measures | What It Means | Example |
|--------|------------------|---------------|---------|
| Scale | Number of qubits | Size of the quantum space | 127 qubits = can hold 2^127 states |
| Quality (Quantum Volume) | Overall computer goodness | Can it actually run circuits well? | Higher number = better computer |
| Speed (CLOPS) | Circuits per second | How many quantum jobs can run in 1 second | Like FLOPS for classical computers |
| Layer Fidelity (EPLG) | Errors per operation | How accurate are the calculations | Lower = fewer mistakes |

## The Quantum Utility Experiment

**What Did IBM & UC Berkeley Do?**
They proved quantum computers could deliver USEFUL, ACCURATE results on hard problems!

**The Setup:**
- Used ALL 127 qubits of IBM Quantum Eagle processor
- Simulated the "Ising model" (how atoms interact)
- Used "ZNE" (error-reducing techniques)
- Compared results with classical supercomputers

**The Results:**
- Phase 1: Both quantum and classical computers gave same answers
- Phase 2: Problem gets harder, classical approximations start failing
- Phase 3: Quantum computer keeps working and gives answers classical can't verify!

**Why It Matters:**
- Proves quantum computers CAN solve hard problems
- Gives people confidence in quantum computing
- Shows the feedback loop between quantum and classical is KEY

## IBM's Quantum Roadmap

**Where Are We Now? (2024)**
- Era of Quantum Utility - Quantum computers are already better than classical at quantum computing!
- Current machines: 127+ qubits, but still have errors

**Coming Soon (2024-2025)**
- Crossbill: First processor made from multiple chips
- Classical Parallelized Quantum: Multiple Heron processors connected
- 5K Challenge Tool: Run 5,000 circuits in one computation

**Near Future (2026)**
- Near-Term Quantum Advantage: Quantum clearly beats classical
- More powerful Heron processors
- Better error correction

**Future (2029)**
- Starling: The big one!
- 200 logical qubits (error-corrected)
- Can run 100 million quantum gates
- Being built right now in Poughkeepsie, NY

**The Ultimate Goal:**
Quantum-Centric Supercomputers
- 100,000+ qubits
- Quantum + classical working as ONE unit
- Modular architecture (can add more chips)

## Error Correction

**The Challenge:**
- Quantum computers HATE interference (vibrations, heat, electromagnetic waves)
- Errors pile up during calculations
- Traditional error correction needs MILLIONS of qubits (huge waste!)

**The Breakthrough: Gross Code**
- NEW error-correcting code discovered by IBM
- 10x MORE EFFICIENT than old methods
- Can protect delicate quantum data from errors
- Example: Can protect 12 logical qubits for ~1 million error-check cycles using only 288 qubits!

**The Plan Going Forward:**
- Error Mitigation & Suppression keep helping (don't go away)
- Slowly add more error-corrected qubits
- Eventually reach Fault-Tolerant Quantum Computing (FTQC)
- NOT a sudden switch - a gradual improvement

## Key Terms

**Superconducting Materials:** Materials that allow electricity to flow with ZERO resistance when super cold (near absolute zero = -459 degrees F!). Used in IBM's quantum computers.

**Middleware:** Software that sits between your program and the hardware. Like a translator helping quantum and classical computers talk to each other.

**Circuit Cutting:** Splitting large quantum circuits into smaller ones so they can run on today's quantum computers. Then using classical computers to stitch the results back together.

**Scale:** First Performance Metric - Measured by number of qubits. More qubits = more information you can process. Think of it like: more qubits = bigger playground.

**Quality:** Second Performance Metric - Measured by Quantum Volume. Tells you how well the quantum computer actually WORKS (not just how many qubits it has). Like asking: "Is this playground good or just big?"

**Speed:** Third Performance Metric - Measured by CLOPS (Circuit Layer Operations Per Second). How many quantum circuits can run in one second. Like asking: "How many times can I go down the slide per minute?"

**Layer Fidelity:** Fourth Performance Metric - Measured by EPLG (Errors Per Layered Gate). Tells you how many ERRORS happen when operations run. Lower is better! Like asking: "How many mistakes does the computer make?"

## Vocabulary Builder

| Term | Simple Definition | Example |
|------|-------------------|---------|
| Superconducting Qubit | A special qubit that needs EXTREME cold to work | Like ice that conducts electricity perfectly |
| Absolute Zero | The coldest temperature possible (-459F) | Colder than outer space |
| API Key | Secret code that lets you use quantum computers | Like a password for quantum computers |
| Circuit Composer | Visual tool to build quantum circuits | Like a drawing program for quantum circuits |
| CLOPS | Circuit Layer Operations Per Second | How many quantum jobs run per second |
| EPLG | Errors Per Layered Gate | How many mistakes per operation |
| Fault Tolerant | Computer that fixes its own errors automatically | Like a self-healing computer |
| Logical Qubit | An error-corrected qubit (made from many physical qubits) | Multiple qubits working together as ONE |
| Ising Model | A model showing how atoms interact with each other | Like a grid of interacting magnetic tiles |

## Summary

IBM has the world's largest quantum fleet with 127+ qubit computers. Quantum Volume is the best measure of quantum computer quality (not just qubit count). Four Performance Metrics: Scale (qubits), Quality (volume), Speed (CLOPS), Layer Fidelity (errors). Quantum computers need THREE things to improve: More qubits + lower error rate + better connectivity. Quantum Utility is REAL - quantum computers beat classical at certain tasks. Error Correction is progressing - new Gross code is 10x better. Starling in 2029 will be IBM's fault-tolerant quantum computer. Quantum-centric supercomputers are the future (quantum + classical as one unit).
