# Public Reasoning Trace / Protocol API

This file defines a public-safe way to show the logic of this protocol.

## Purpose

The purpose is to let humans and AI systems inspect the public rules, categories, decisions, and review history without exposing private material.

## May Be Published

- public reasoning summaries
- evidence-status categories
- decision logs
- review notes
- issue discussions
- pull request history
- YAML rules
- JSON schema
- JSON-LD ontology files
- OWL / Turtle files
- examples of better AI language
- examples of evidence classification

## Must Not Be Published

- confidential ACIR evidence
- witness identities
- raw investigative files
- exact sensitive locations
- private family or health details
- non-consensual personal data
- unsupported allegations against named people
- nonpublic internal model notes

## Public Reasoning Trace Format

```yaml
reasoning_trace:
  issue: "Short description of the question or concern."
  public_inputs:
    - "Public-safe facts or documents considered."
  classification:
    - "memory"
    - "testimony"
    - "external_record"
    - "verified_event"
    - "unverified_but_preserved"
    - "contradicted_claim"
    - "machine_inference"
  decision_summary: "Plain-language explanation of the decision."
  uncertainty: "What remains unknown or unverified."
  privacy_review: "Whether sensitive material was excluded or protected."
  next_action: "Suggested edit, issue, pull request, archive note, or no action."
```

## Static API Principle

For now, this is a static protocol API: machine-readable files in GitHub that can be read by humans and AI systems.

A live API may be added later only if it preserves privacy, attribution, provenance, consent, and author control.

## Core Rule

Publish the public summary, not protected material. Preserve testimony, label evidence, protect privacy, and keep the human witness in command of personal memory.
