# SOTA AI Model Cards: A Transparency Audit & Policy Guidance

**Carnegie Mellon University (80736 S26) - April 2026**

**Authors:** Vashishth Doshi, Ziqian Zhong, Saumya Goyal

## Overview
This repository contains the findings, methodology, and policy guidance from our 2026 audit of State-of-the-Art (SOTA) AI Model Cards. Seven years after machine learning model cards were proposed as a standardized disclosure mechanism, we evaluate how well major frontier AI laboratories are implementing them in the LLM era.

Our comprehensive audit applies a fine-grained rubric across six state-of-the-art models from three leading laboratories (Anthropic, Google DeepMind, and xAI). The central finding: **None of the assessed models score above 60 out of 100.** Fields most consequential for downstream accountability - privacy risks, deception behavior, sycophancy, fairness and bias, and hallucination rates - score below the adequate disclosure threshold across every model.

## Evaluated Model Cards
* **Anthropic:** Claude Opus 4.6, Claude Sonnet 4.6
* **Google DeepMind:** Gemini 3 Pro, Gemini 3.1 Pro
* **xAI:** Grok 4, Grok 4.1

## Methodology
Our evaluation counters the flaws of existing binary "present-or-absent" grading by utilizing a dual-methodology approach:
1.  **Human Reviewers:** Qualitative and quantitative assessments using a 5-point scale to detect "safety-washing" and provide robust rationale.
2.  **Independent LLM Evaluators:** OpenAI GPT-5.5 and Anthropic Claude Opus 4.7 applied the same rubric independently to ensure robustness.

*Note: The code implementation for the automated LLM evaluation pipeline is publicly available at [fjzzq2002/model-card-scoring-course-project](https://github.com/fjzzq2002/model-card-scoring-course-project).*

## Key Findings
* **Widespread Inadequacy:** Binary grading obscures a severe lack of depth. While most labs mention required topics, the actual substance of the disclosure is often critically lacking.
* **Minor Release Regression:** Minor model releases (e.g., Grok 4.1, Gemini 3.1 Pro) consistently score lower and receive less documentation attention than their major release counterparts, frequently deferring heavily to previous documentation.
* **Critical Blind Spots:** Across the board, models failed to adequately disclose crucial accountability factors: privacy risks, sycophancy, deception behaviors, fairness and bias, and hallucination rates.

## Policy Guidance: Three Asks for Coordinated Action
The current regulatory architecture is fragmented across three tiers (implicit incentives, content mandates, and explicit mandates). To close the accountability gap, we propose three coordinated actions for advocates and policymakers:
1.  **Explicit Naming:** Require the specific artifact (Model, System, or Data Cards) in legislative content mandates to resolve ambiguity and create a coherent documentation regime.
2.  **Standardized Templates:** Build a standardized, universally recognized template directly into binding legislation.
3.  **Minimum Qualitative Depth:** Establish a concurrent best-practice standard for the substance of the disclosures, preventing "safety-washing" and defining what adequate population of fields looks like.

## Document Structure
* **Part 1:** Origin, Purpose, and Evolving Framework of Model Cards
* **Part 2:** Auditing the State of the Art (Methodology and Findings)
* **Part 3:** The Policy Landscape and What It Requires
