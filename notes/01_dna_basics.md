
# Day 1: The Molecular Operating System

**Date:** 2026-05-24
**Topic:** Central Dogma & Sequencing Strategies

---

## 1. Core Architecture (Nucleic Acids)
Life runs on two main types of data storage:
*   **DNA (Deoxyribonucleic Acid):** The **Hard Drive**. Permanent, stable storage of genetic instructions. Kept in the nucleus.
*   **RNA (Ribonucleic Acid):** The **RAM / Flash Drive**. Temporary, volatile copies used to execute tasks.

---

## 2. The Central Dogma (Data Flow)
The flow of genetic information is strictly one-way (mostly):
1.  **Replication:** DNA $\to$ DNA. (Copying the hard drive before cell division).
2.  **Transcription:** DNA $\to$ RNA. (Creating a working copy of a specific file).
3.  **Translation:** RNA $\to$ Protein. (Compiling the code into a functional machine).

```text
[DNA] --Replication--> [DNA]
  |
  +--Transcription--> [RNA] --Translation--> [Protein]
```

*Key Term:* A group of 3 RNA letters is called a **Codon**. One Codon = One Amino Acid.

---

## 3. How We "Hack" the System (Sequencing)
We can't read the DNA strand directly like a barcode. We have to break it down.

### Strategy A: Expression Profiling (The "Snapshot")
*   **Goal:** See what the cell is doing *right now*.
*   **Method:** Capture all the RNA currently floating around. If a gene is being used, it will have RNA present.

### Strategy B: Whole Genome Sequencing (Shotgun Method)
*   **Goal:** Read the entire source code.
*   **Workflow:**
    1.  **Extraction:** Pull DNA out of the cell.
    2.  **Fragmentation:** Shred the long DNA strands into millions of tiny random pieces.
    3.  **Amplification:** Insert pieces into bacteria to clone them (make millions of copies for reading).
    4.  **Assembly:** Use algorithms to find overlapping ends and stitch the puzzle back together.

---

## 4. Connection to Coding
Understanding the biology tells us how to structure our data:

*   **DNA is a String:** In Python, a gene is `seq = "ATCG..."`.
*   **Transcription is String Manipulation:** Replacing 'T' with 'U'.
*   **Translation is a Hash Map:** Looking up 3-letter keys (`AUG`) to get values (`Methionine`).
*   **Assembly is Pattern Matching:** We write code to find where `string_A` overlaps with `string_B`.
```
