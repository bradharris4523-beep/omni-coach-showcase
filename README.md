# Omni Coach

### AI-Powered Competitive Gaming Intelligence

**Replay Analysis · AI Mentoring · Performance Tracking**

Omni Coach is an independently developed AI-assisted competitive gaming platform designed to help players better understand their gameplay, investigate decisions, and identify opportunities for improvement.

The project brings together game telemetry, machine learning, conversational AI, and performance analytics within a unified coaching experience.

**Status:** Active development | Private source code | Counter-Strike 2 flagship implementation

---

## Overview

Competitive players generate substantial amounts of gameplay data, but translating that data into actionable improvements is challenging.

Omni Coach explores a more connected approach to game improvement through three core systems:

- **Match Analysis:** Transform recorded gameplay into structured telemetry, model-driven analysis, and coaching explanations.
- **AI Mentor:** Provide contextual, conversational coaching through persistent sessions and configurable mentoring styles.
- **Performance Tracker:** Organize match histories and aggregated performance data to help players evaluate their progress.

Rather than treating gameplay analysis and coaching as separate experiences, Omni Coach is designed to connect them into a continuous improvement workflow.

## System Architecture

The platform integrates a web application, Python backend, asynchronous processing infrastructure, game-specific parsers, model inference, and AI-generated explanations.

**Simplified processing flow:**

Gameplay Replay → Secure Upload → Analysis Queue → Replay Parsing → Model Processing → Explanation Generation → Coaching Report

A separate tracking pipeline handles match ingestion, historical records, and performance aggregation.

Major architectural components include:

- Astro and React frontend
- Python and FastAPI application services
- PostgreSQL-backed asynchronous job processing
- Game-specific replay parsing and telemetry transformation
- Custom PyTorch model and training infrastructure
- Language-model integration for coaching explanations
- Persistent conversational mentoring
- Match tracking and analytics services
- Containerized service architecture and cloud deployment configuration

The private implementation is organized around separating computational analysis, external AI services, background processing, and user-facing experiences.

## Core Product Systems

### 01 — Match Analysis

The analysis system is designed to transform gameplay recordings into structured information players can review.

Implemented components include replay submission, job scheduling, parsing, telemetry processing, model integration, and report-generation paths.

Its asynchronous architecture helps separate computationally intensive analysis from ordinary web requests.

### 02 — AI Mentor

A conversational coaching system built around contextual discussion and ongoing player interactions.

Implemented capabilities include:

- Streaming AI-generated responses
- Persistent conversation history
- Session management
- Configurable coaching personas
- Context construction from previous messages
- Integration with application access controls

The goal is to move beyond isolated feedback and support follow-up discussion about decisions, performance, and improvement.

### 03 — Performance Tracker

A game-performance analysis system designed to connect match records with longer-term player development.

The implementation includes match ingestion, parsing, historical aggregation, cached profile data, and performance visualization.

This allows gameplay history and coaching to be explored as complementary parts of the same experience.

## Machine Learning & AI Engineering

Omni Coach includes a custom neural-network research and engineering subsystem built using PyTorch.

The inspected implementation contains:

- Game and map context representations
- Sparse mixture-of-experts adaptation
- Spatial feature processing
- Attention-based and temporal components
- Multiple prediction outputs
- Multi-objective training infrastructure
- Gradient-based feature attribution
- Specialist explanation routing
- Model-oriented alternative-action exploration

These systems reflect independent architectural and integration work using established machine-learning frameworks.

**Validation note:** Model architecture and training code are implemented, but predictive accuracy, cross-game generalization, and coaching effectiveness have not yet been established through independently verified evaluation results.

## Engineering Highlights

### Asynchronous Processing

Analysis jobs are handled through background processing infrastructure, including transactional work claiming, progress handling, heartbeats, and recovery mechanisms.

### Computational Workload Management

The analysis architecture incorporates chunking and batching strategies while separating inference workloads from latency-sensitive external AI requests.

### Gameplay Data Integration

Game-specific replay processing is connected to downstream analytical models and user-facing explanations.

### Custom Product Experience

The frontend combines interactive gameplay demonstrations, responsive design, custom Blender-generated assets, and scroll-controlled visual storytelling.

### Integrated AI Workflows

Language-model services are incorporated into a broader application architecture involving structured data, model outputs, routing, and conversational interfaces.

## Technology Stack

**Frontend:** Astro, React, TypeScript, JavaScript, CSS, Zustand

**Backend:** Python, FastAPI, Pydantic, SQLAlchemy, PostgreSQL

**Machine Learning:** PyTorch, NumPy, Polars, Captum

**Replay Processing:** Game-specific parsers, telemetry transformation, asynchronous processing

**AI Integration:** Language-model APIs, specialist routing, retrieval integration

**Infrastructure:** Docker, GitHub Actions, AWS-related services, S3-compatible storage

**Testing:** Vitest, Testing Library, backend unit and integration testing infrastructure

**Visual Production:** Blender, Python rendering workflows, custom web animation

## Development & Validation Status

Omni Coach remains an active software development project.

The repository contains substantial frontend, backend, machine-learning, replay-processing, tracking, and infrastructure implementations.

Selected frontend tests and builds have passed during development. Broader end-to-end production operation, predictive model quality, reliability under real workloads, and deployment health require further verification.

Additional game-specific code is under development and should not be interpreted as confirmed released support.

## Current Development Priorities

- End-to-end verification of the Counter-Strike 2 replay analysis workflow
- Evaluation and calibration of model predictions
- More extensive integration and reliability testing
- Continued refinement of coaching explanations
- Performance measurement and operational validation
- Improvements to user experience, accessibility, and visual presentation
- Progressive validation of additional game integrations

## Project Demonstrations

Screenshots, architecture visualizations, and selected demonstrations will be added as they are reviewed and prepared for public release.

The project is presented as a technical engineering showcase rather than an open-source software distribution.


## Product Gallery

Screenshots from an earlier Omni Coach application experience.

<table>
<tr>
<td width="50%">
<img src="2d%20Map%20display" width="100%">
<br><b>2D Tactical Replay</b>
</td>
<td width="50%">
<img src="Post%20Match%20Metrics" width="100%">
<br><b>Post-Match Analytics</b>
</td>
</tr>
<tr>
<td>
<img src="Post%20Match%20Coaching%20report" width="100%">
<br><b>AI Coaching Report</b>
</td>
<td>
<img src="Live%20tracker" width="100%">
<br><b>Performance Tracker</b>
</td>
</tr>
<tr>
<td>
<img src="Omni%20Mentor" width="100%">
<br><b>AI Mentor</b>
</td>
<td>
<img src="Dashboard" width="100%">
<br><b>Command Center</b>
</td>
</tr>
<tr>
<td colspan="2">
<img src="Upload%20spot" width="100%">
<br><b>Replay Upload Experience</b>
</td>
</tr>
</table>


## Source Code & Intellectual Property

Omni Coach is an independently developed proprietary software project.

The application source code, model weights, internal infrastructure, and sensitive implementation details are maintained in private repositories.

This public repository documents selected technical capabilities, development approaches, and product concepts without distributing the underlying commercial implementation.

---

**Bradley Harris**  
Independent Software Developer  
Boise State University

*Building intelligent systems, ambitious software products, and practical applications of artificial intelligence.*
