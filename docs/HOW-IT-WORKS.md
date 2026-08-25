# How Codebase Inspection Works

The visuals on this page are static SVGs, so they render directly on GitHub on phones and desktop browsers. Each one is generated from a model specific to this skill.

## System architecture

![Detailed system map for Codebase Inspection](../assets/system-map.svg)

### Components

- **1. Repository tree:** participates in confirm repository scope and exclusions.
- **2. Language detector:** participates in enumerate tracked source files.
- **3. pygount counters:** participates in classify languages and generated code.
- **4. Ratio calculator:** participates in count code comments and blanks.
- **5. Inspection report:** participates in calculate composition ratios.

## Actor and data sequence

![Actor and data sequence for Codebase Inspection](../assets/operation-sequence.svg)

### 1. Confirm repository scope and exclusions

**Primary surface:** `Repository tree`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 2. Enumerate tracked source files

**Primary surface:** `Language detector`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 3. Classify languages and generated code

**Primary surface:** `pygount counters`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 4. Count code comments and blanks

**Primary surface:** `Ratio calculator`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 5. Calculate composition ratios

**Primary surface:** `Inspection report`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.
### 6. Report measurements without modification

**Primary surface:** `Repository tree`

Record the concrete input, the operation performed, and the evidence produced at this stage. Continue only when the output is sufficient for the next stage; otherwise preserve the blocker and stop.

## Example output shape

![Illustrative output for Codebase Inspection](../assets/example-output.svg)

The example is a visual contract: a real run may look different, but it should expose comparable state, provenance, and verification information. It is not presented as evidence of a live external action.

## Decision and stop conditions

![Decision guide for Codebase Inspection](../assets/decision-guide.svg)

The workflow stops when the target is ambiguous, the relevant surface is unavailable or unauthorized, or the final artifact cannot be checked. A logged-in session or successful tool call is not by itself proof that the requested outcome is complete.

## Verification checklist

- Confirm every component shown in the system map exists in the target environment.
- Trace the actor sequence using actual tool output or artifact state.
- Compare the result with the example-output information contract.
- Re-read or reopen the final artifact instead of trusting an attempt message.
- Report omitted stages, unsupported capabilities, and remaining human decisions.
