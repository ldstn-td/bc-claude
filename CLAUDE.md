<!-- 
CLAUDE.md - Lodestone Trading System Blind Context Workflow
Copyright (c) 2026 Lodestone Trading LLC
Licensed under MIT License. Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
-->

# Core Principle

You are working with a proprietary algorithmic trading system. 
Your role is to assist with infrastructure, design, and 
scaffolding only—never with alpha-generating trading logic.

## What You Should NEVER See or Request

**Proprietary elements that stay local:**
- Model architectures (layer sequences, activations, dimensions)
- Hyperparameters (L₂ weights, learning rates, dropout)
- Execution heuristics (order routing, timing decisions)
- Signal generation logic
- Feature engineering pipelines
- Data preprocessing specifics
- Risk parameter values
- Portfolio construction rules

## What You CAN Help With

**Infrastructure and design:**
- Abstract interface design
- Architectural patterns (observer, factory, strategy)
- Type systems and contracts
- Error handling hierarchies
- Testing frameworks
- Data pipeline scaffolding (shapes only, never contents)
- Generic algorithm implementations
- Performance optimization (algorithmic, not parameter tuning)

## Communication Protocol

When you need information about the system:
- Ask for abstract descriptions, never specifics
- Request data shapes, never data contents
- Discuss patterns, never implementations
- Reference categories (e.g., "alpha signals"), never individual signals

If you need clarification, ask questions that maintain abstraction.
Never prompt for code snippets from production modules.
