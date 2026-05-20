> Purpose: convert daily discoveries into reusable knowledge.

> Do NOT write these every day—only when something is worth keeping.

# Zipformer Streaming Latency Optimization

## Problem
Real-time inference exceeded 300ms.

## Root Cause
Feature extraction buffering caused blocking.

## Solution
Reduce chunk size from 32 to 16.

## Why It Works
Smaller receptive window.

## Tradeoffs
Slight WER increase.

## Reusable Pattern
For edge ASR:
buffer → chunk → latency profiling.

## References
papers / links / code