# android-ai-glasses-runtime
Android-based runtime prototype for AI/AR glasses, supporting phone-glass pairing, split-computing orchestration, device event routing, and multiple AI provider abstraction.

## Problem
AI glasses have limited battery, thermal budget, and compute capacity.
Therefore, the phone runtime must coordinate pairing, event routing, split computing, and AI provider selection.

## Architecture
Glass Simulator → Pairing Manager → Event Dispatcher → Split Compute Router → AI Provider

## Key Design Decisions
- StateFlow for runtime state updates
- Coroutine for asynchronous event processing
- AIProvider interface for multiple model support
- Router-based split compute decision
- Mock-first design for testability
