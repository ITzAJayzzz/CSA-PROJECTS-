# CSA-PREFINALS-PROJECTS-
CSA Projects of Borcelas and Gula

Drive link for Glusterfs and Raid:

[GLUSTERFS](https://drive.google.com/drive/folders/1MlRYA3VccvpqJ98DtAsB3d7qYz-uOLX6)

[RAID](https://drive.google.com/drive/folders/1ycnfG0wUvor9HfvdHkd_utSgKVNhLywT)

---
---

## Disk Scheduling Algorithm Simulation

This program, `sched.py`, demonstrates how various operating system disk scheduling algorithms manage I/O requests to minimize total head movement.

---

## Algorithms Implemented

The script provides a comparative analysis of the following five strategies:

* [cite_start]**FCFS (First-Come, First-Served):** Services requests in the exact order they arrive in the queue[cite: 1].
* [cite_start]**STF (Shortest Time First):** A greedy approach that selects the request closest to the current head position[cite: 2].
* [cite_start]**SCAN (Elevator Algorithm):** The disk arm moves toward track 0, servicing all requests in that path, before reversing direction[cite: 2].
* [cite_start]**C-SCAN (Circular SCAN):** The arm moves toward track 0, then performs a full jump to the opposite boundary (track 300) to service remaining requests[cite: 2, 3].
* [cite_start]**C-LOOK (Circular LOOK):** A version of C-SCAN that only travels to the furthest requested tracks instead of the absolute disk boundaries[cite: 2, 3].

---

## How to Run

1. Ensure Python 3 is installed on your system.
2. Navigate to the directory containing the file.
3. Execute the script via the terminal:
   
   python sched.py

---

## Input Configuration

The simulation uses the following parameters as defined in the source code:

* [cite_start]**Initial Head Position:** 75 [cite: 3]
* [cite_start]**Request Queue:** [75, 25, 290, 215, 50, 75, 120, 85, 245, 98] [cite: 3]

---

## Technical Concepts

* [cite_start]**Absolute Distance Calculation:** Used to determine seek time[cite: 1].
* [cite_start]**List Manipulation:** Utilizes sorting and filtering to organize track requests[cite: 2].
* [cite_start]**Simulation Logic:** Models the mechanical behavior of a disk drive head in a software environment[cite: 2].
