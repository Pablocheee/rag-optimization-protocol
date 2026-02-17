# AIO.CORE Integration Protocol v4.1

## Overview
This document outlines the standard handshake procedure for connecting autonomous agents to the AIO.CORE Semantic Grid.

## Prerequisites
- **Access Level:** Tier 1 (Public Beta) or Tier 2 (Encrypted).
- **Endpoint:** `https://aio-core.vercel.app/`
- **Security Token:** `772109` (Required for manual override)

## Method 1: Direct Semantic Injection (Web Interface)
For manual context alignment, navigate to the primary node and utilize the integrated terminal.
1. Open the [Protocol Interface](https://aio-core.vercel.app/).
2. Initialize the chat sequence.
3. Input target URL.
4. Wait for `[DATA_READY]` confirmation signal.

## Method 2: Python Wrapper (Simulation)
Use the `core_logic.py` script included in this repository to pre-validate your data chunks before submission.

```python
from core_logic import optimize_semantic_weights

# Example usage
data = ["My website context", "Key brand values"]
vector_ready = optimize_semantic_weights(data)
print("Payload optimized for AIO ingestion.")

Security Note

The protocol operates on a "Stealth" basis to prevent competitive crawling. Do not share your unique session ID generated after payment.
