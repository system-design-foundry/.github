# What Is System Design Foundry?

Application developers build software for users. Systems software engineers build the foundations other software relies on. **System Design Foundry builds foundations and tools for those systems builders.**

System Design Foundry is an open-source effort exploring a simple idea: **foundational software becomes more useful when more of its meaning is represented explicitly.**

That means putting semantics on systems.

Software often begins with rich knowledge about what something means: types, ownership, constraints, relationships, intent, provenance, capabilities, effects, structure, and expected behavior. As software moves through parsers, compilers, generators, binary formats, protocols, and other transformations, much of that information is traditionally discarded or buried inside implementation details.

SDF explores what becomes possible when more of that meaning survives.

## Why start with languages and compilers?

Programming languages are a natural proving ground for this idea because compilers already have to reason explicitly about meaning.

A compiler must understand considerably more than syntax. It deals with types, control flow, ownership, effects, diagnostics, source relationships, target capabilities, transformations, and the rules governing how one representation becomes another.

That makes compiler infrastructure a useful place to develop and test richer semantic models.

SDF therefore begins heavily in the language and compiler space, with work around parsing, typed syntax trees, semantic intermediate representations, diagnostics, provenance, lowering, code generation, and language tooling.

But compilers are the starting point, not the boundary.

## Beyond programming languages

The same principles apply to many other forms of foundational software.

Binary structures, for example, contain meaning that is frequently represented only through specification documents and handwritten parsing code. SDF's binary-definition work explores describing that structure explicitly across static formats, streaming data, and protocols.

Similar ideas can potentially apply to executable formats, storage formats, network protocols, runtimes, distributed systems, embedded systems, resource models, and other areas where software has important semantics that are difficult to preserve or expose.

The goal is not to force every system into one universal representation. It is to build reusable approaches for describing the meaning that matters in each domain and carrying that information far enough that other tools can use it.

## Semantics and AI

This becomes increasingly important as AI becomes part of software engineering.

AI can infer meaning from source code, documentation, binary layouts, logs, and other artifacts. But inference is not the same thing as having the system explicitly describe what something means.

When semantics are represented directly, deterministic software and AI can work from the same structured knowledge.

That can make it easier to analyze systems, generate implementations, validate transformations, explain behavior, compare alternatives, preserve provenance, identify unsupported capabilities, and reason about changes without repeatedly reconstructing intent from lower-level artifacts.

SDF is therefore interested not simply in using AI to write software, but in building software whose semantic structure makes it easier for **people, deterministic tools, and AI to reason about the same system together**.

## What SDF builds

System Design Foundry develops libraries, languages, models, generators, and tools for systems builders.

Its current work is concentrated around language construction, compiler infrastructure, semantic representation, binary and protocol definition, source provenance, diagnostics, transformation, and multi-target generation.

Some projects may become broadly useful infrastructure. Others may remain experiments. Some ideas may fail entirely and still produce useful information about where an approach does or does not work.

That experimentation is intentional.

The long-term goal is not a single compiler, programming language, binary parser, or framework.

It is to explore how **explicit semantics can make foundational software easier to build, transform, analyze, and reason about—by both people and machines.**
