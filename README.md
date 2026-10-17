# RISC-V Transformer (Attention Mechanism) in Assembly

Project developed for the Introduction to Computer Architecture (IAC) course at Instituto Superior Técnico.

## Overview
This project implements the forward pass of a simplified Transformer model (the architecture behind modern LLMs) entirely from scratch in RISC-V Assembly language. 

The program reads a vocabulary, an input sequence, and weight matrices (W_Q, W_K, W_V, and Embeddings) from text files. It then calculates the Query, Key, and Value matrices to compute attention scores and predict the next token in the sequence.

*(Note: An initial logic circuit representation of this architecture was also designed using Logisim for the first part of the course).*

## Key Features
- **Low-Level Matrix Mathematics:** Implemented matrix multiplication, vector dot products, and argmax functions directly manipulating CPU registers and memory.
- **Robust Error Handling:** Includes manual overflow detection for integer multiplication and addition during dot product calculations.
- **Self-Attention Mechanism:** Implements the core Q, K, and V matrix multiplications and score computations required for Transformer attention.
- **File I/O in Assembly:** Uses system calls (`ecall`) to open, read, and parse text files into memory buffers.

## Technologies
- RISC-V Assembly
- Logisim (for initial hardware logic design)
- Computer Architecture
