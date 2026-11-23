# TCS JFLAP ASSIGNMENT

**Student Name:** Sukanya Auti 
**Roll No / Class:** D12B-04
**Subject:** Theory of Computer Science (TCS)  
**Tool:** JFLAP (Java Formal Languages and Automata Package)  

---

## About JFLAP

**JFLAP** (Java Formal Languages and Automata Package) is an interactive educational software tool designed for experimenting with formal languages and automata theory. It provides a visual and interactive environment to design, simulate, and analyze foundational computational models studied in Computer Science.

### Key Capabilities:
- **Graphical Automata Design:** Construct and visually lay out state diagrams for finite automata, pushdown automata, and Turing machines.
- **Interactive Simulation:** Execute inputs using Single Step, Fast Run, and Multiple Run (batch testing) to evaluate acceptance and rejection behavior.
- **Formal Grammar Tools:** Define regular and context-free grammars, test derivations, eliminate ambiguity, and transform grammars into normal forms.
- **Parsing Algorithms:** Construct and visualize parsing tables for LL(1) top-down parsing and the Cocke–Younger–Kasami (CYK) dynamic programming algorithm.
- **Automated Conversions:** Step through equivalence algorithms, including Regular Expression to NFA/DFA, Grammar to DFA, CFG to CNF, and CFG to NPDA.

---

## Topics Covered

This assignment covers key theoretical and practical concepts across the Theory of Computer Science curriculum:

1. **Deterministic Finite Automata (DFA):**
   - Modulo arithmetic and counting conditions (even/odd parity, divisibility checks).
   - Substring tracking and pattern recognition (e.g., prefix, suffix, and exact occurrence constraints).

2. **Non-Deterministic Finite Automata (NFA):**
   - Non-deterministic branching and state guessing (e.g., tracking the $k$-th symbol from the end).
   - Union of pattern recognition paths.

3. **Regular Expressions (RE) & Regular Grammars:**
   - Formal specification of regular languages.
   - Right-linear grammars and equivalence conversions between Regular Expressions, Grammars, and Finite Automata.

4. **Finite State Machines with Output (Transducers):**
   - **Mealy Machines:** State-and-input dependent output generation (e.g., synchronous sequence detectors).
   - **Moore Machines:** State-associated output generation (e.g., residue modulo computation).

5. **Context-Free Grammars (CFG):**
   - Generating non-regular languages such as $\{a^n b^n \mid n \ge 1\}$.
   - Modeling structural properties like palindromes over alphabet $\{a, b\}$.

6. **Chomsky Normal Form (CNF):**
   - Transforming general context-free grammars into restricted production rules ($A \to BC$ or $A \to a$) for parsing and analysis.

7. **Pushdown Automata (PDA / NPDA):**
   - Stack-based computation for context-free language recognition.
   - Acceptance by final state and acceptance by empty store.
   - Top-down (LL-style) conversion between CFGs and NPDAs.

8. **Parsing Algorithms:**
   - **LL(1) Parsing:** Non-left-recursive grammar design, First and Follow sets calculation, and conflict-free parse table construction.
   - **CYK Parsing:** Triangular dynamic programming table generation for membership verification using grammars in Chomsky Normal Form.

---

## How to Open and Run

### 1. Prerequisites
- **Java Runtime Environment (JRE):** Java 8, 11, or newer installed on your machine.
- **JFLAP:** `JFLAP7.1.jar` executable.

To verify Java is installed, run:
```bash
java -version
```

### 2. Launching JFLAP
Open a terminal in the folder containing `JFLAP7.1.jar` and run:
```bash
java -jar JFLAP7.1.jar
```
*Alternatively, you can double-click `JFLAP7.1.jar` directly in File Explorer.*

### 3. Opening Assignment Files
1. In the JFLAP main menu, click **File** $\to$ **Open** (or press `Ctrl + O`).
2. Navigate to this directory and select any `.jff` file to load its diagram, grammar, or expression into the workspace.

### 4. Running and Testing Models

#### For Finite Automata & Pushdown Automata (DFA, NFA, PDA):
- **Batch Testing (Multiple Run):**
  1. Click **Input** $\to$ **Multiple Run**.
  2. Enter test strings into the input column.
  3. Click **Run Inputs** to see instant `Accept` or `Reject` verdicts.
- **Step-by-Step Visualization:**
  - Click **Input** $\to$ **Step with State** (or **Step by State**) to step through state transitions symbol-by-symbol with active stack/state inspection.
- **Fast Run:**
  - Click **Input** $\to$ **Fast Run** for quick single-string verification.

#### For Mealy & Moore Machines:
1. Click **Input** $\to$ **Multiple Run** (or **Fast Run**).
2. Enter an input sequence to view the generated synchronous output sequence alongside each transition.

#### For Grammars (CFG, LL(1), CYK):
- **Brute Force Parsing:**
  - Click **Input** $\to$ **Brute Force Parse** $\to$ enter a string to generate its derivation tree.
- **LL(1) Parse Table:**
  - Click **Input** $\to$ **Build LL(1) Parse Table** to inspect First/Follow sets and construct the LL(1) parsing matrix.
- **CYK Parsing:**
  - Click **Input** $\to$ **CYK Parse** $\to$ enter an input string to dynamically fill the triangular parsing table.

#### For Equivalence & Conversions:
- Use the **Convert** menu in JFLAP to step through automated conversions:
  - `Convert` $\to$ `Convert to NFA` / `Convert to DFA` (for Regular Expressions).
  - `Convert` $\to$ `Convert to FA` (for Regular Grammars).
  - `Convert` $\to$ `Transform to CNF` (for CFGs).
  - `Convert` $\to$ `Convert to PDA` (for CFGs).
