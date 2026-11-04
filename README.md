# Thermal Test Intelligence Center (TTIC)
### Semiconductor Test Analytics & Engineering Visualization

**Python | Streamlit | Engineering Analytics | Interactive Visualization | Test Comparison | Automated Reporting**

**Project Status:** Engineering Pilot — Validation in Progress

---

## Project Overview

The **Thermal Test Intelligence Center (TTIC)** is a Python-based engineering analytics application designed to simplify the analysis, visualization, comparison, and reporting of thermal test data.

The application provides engineers with a centralized workspace to explore measurement channels, investigate thermal behavior, compare test runs, and generate structured engineering reports.

TTIC transforms raw engineering test logs into meaningful analytical insights through interactive visualizations, engineering calculations, event analysis, and repeatable reporting workflows.

The application is designed for local execution, allowing engineers to analyze test files without uploading data to a cloud service.

> **Portfolio Note:** This repository showcases the application's design, capabilities, documentation, and engineering workflows. Source code, executable files, and engineering datasets are intentionally excluded.

---

## Application Preview

The TTIC application provides a centralized interface for engineering test analysis, visualization, comparison, and reporting.

![TTIC Application Overview](Screenshots/TTIC%20Home%20Page.png)

---

## The Engineering Challenge

Engineering test environments frequently generate large volumes of measurement data across multiple channels and test runs.

Traditional analysis workflows can involve several challenges:

- **Fragmented data:** Logger exports vary in structure, duration, and measurement channels.
- **Time-consuming analysis:** Engineers manually investigate thermal transitions, heating/cooling behavior, and stability.
- **Complex comparisons:** Different test durations and operating conditions make comparisons difficult.
- **Repeated reporting:** Charts, calculations, and reports often need to be recreated.
- **Limited traceability:** Analysis settings, assumptions, and engineering observations may not be consistently documented.

These challenges create opportunities to improve analytical efficiency, consistency, and engineering review processes.

---

## The Solution

TTIC provides an integrated engineering analytics workflow:

**Import → Visualize → Analyze → Investigate → Compare → Report**

The application combines six functional modules within a browser-based interface.

### 1. Test Setup

Supports engineering test preparation and data-quality review.

Key capabilities include:

- Import CSV and Excel logger files.
- Identify timestamps and measurement channels.
- Review observation counts and test duration.
- Inspect timestamp quality and missing measurements.
- Record test metadata, operating conditions, and engineering observations.

### 2. Interactive Visualization

Enables engineers to explore measurement behavior through configurable charts.

Capabilities include:

- Interactive multi-channel visualization.
- Primary and secondary Y-axis configuration.
- Channel selection and chart customization.
- Zooming into specific observation periods.
- Optional display smoothing.
- Exporting interactive charts and reusable configurations.

Engineering calculations use the selected raw measurement data rather than visually smoothed traces.

### 3. Engineering Analytics

Provides quantitative indicators for investigating thermal behavior.

Analytical capabilities include:

- Descriptive statistics.
- Minimum, maximum, and average measurements.
- Measurement variability.
- Heating and cooling rates.
- Interval-based rate calculations.
- Channel-level engineering metrics.

These measurements support engineering investigation and comparison.

### 4. Event Intelligence

Supports the investigation of thermal stability and command-response behavior.

Capabilities include:

- Stability-window screening.
- Identification of low-variation measurement periods.
- Detection of command-step events.
- Manual event-time selection.
- Response-time calculations.
- t10, t50, and t90 measurements.
- 10–90% transition-time analysis.

**Important:** Automated screening provides engineering indicators, not certified equilibrium determinations or automatic product acceptance decisions.

### 5. Reports & Export

Supports repeatable engineering documentation.

Reporting capabilities include:

- Excel engineering reports.
- PDF engineering summaries.
- Measurement statistics and supporting tables.
- Analytical results and chart evidence.
- Analysis settings and test metadata.
- Engineering observations and review information.

The objective is to reduce repetitive report preparation and improve consistency across engineering reviews.

### 6. Test Comparison

Allows engineers to compare two thermal test runs.

Supported comparison approaches include:

| Comparison Mode | Description |
|---|---|
| Full Test | Compare complete test recordings |
| Common Duration | Compare tests over a shared elapsed-time duration |
| Independent Windows | Compare selected periods from different test runs |

Comparison capabilities include:

- Interactive test overlays.
- Separate statistical calculations.
- Heating and cooling rate comparisons.
- Stability screening comparisons.
- Command-response timing comparisons.
- Excel and PDF comparison reports.

Comparisons require engineering interpretation, particularly when test conditions, units, or operating environments differ.

---

## High-Level Application Architecture

TTIC follows a local engineering analytics workflow:

```text
Engineering Test Files
       |
       v
Data Import & Validation
       |
       v
Timestamp & Channel Processing
       |
       v
Interactive Visualization
       |
       v
Engineering Analytics
       |
       v
Event & Stability Analysis
       |
       v
Test Comparison
       |
       v
Excel / PDF Reporting
```

The application uses a Python-based analytical backend and a Streamlit browser interface.

Its core workflow is designed to process engineering data locally.

---

## Technology Stack

| Technology | Application |
|---|---|
| Python | Application development and engineering analytics |
| Streamlit | Interactive browser-based interface |
| Pandas | Data processing and analytical calculations |
| Interactive charting | Multi-channel and dual-axis visualizations |
| Excel | Structured engineering reporting |
| PDF | Engineering summaries and comparison reports |
| Windows | Target environment for portable pilot deployment |

---

## Application Workflows

The following documents demonstrate the application's main functional areas.

| Module | Documentation |
|---|---|
| Test Setup | [View Test Setup](application-workflows/TTIC_Setup.pdf) |
| Interactive Visualization | [View Visualization](application-workflows/TTIC_Visualization.pdf) |
| Engineering Analytics | [View Engineering Analytics](application-workflows/TTIC_EnggAnalytics.pdf) |
| Event Intelligence | [View Event Intelligence](application-workflows/TTIC_EventIntelligence.pdf) |
| Reports & Export | [View Report Generation](application-workflows/TTIC_Report_Generation.pdf) |
| Test Comparison | [View Test Comparison](application-workflows/TTIC_TestComparison.pdf) |

---

## Business and Engineering Value

TTIC is designed to deliver value across several areas.

**Engineering Productivity**

Reduces repetitive chart preparation, manual calculations, and report creation.

**Analytical Consistency**

Provides a repeatable workflow for calculating engineering indicators and comparing test runs.

**Improved Investigation**

Helps engineers explore thermal transitions, measurement variability, and command-response behavior.

**Reporting Standardization**

Supports structured Excel/PDF outputs with analysis settings and engineering observations.

**Knowledge Sharing**

Makes engineering results easier to review and communicate across teams.

These represent intended benefits. Quantified productivity improvements will require validation during engineering pilot testing.

---

## Windows Deployment Approach

TTIC is designed to support a portable Windows engineering pilot.

The intended deployment approach allows engineers to launch the application locally without separately installing Python.

The application uses a local browser interface.

**Deployment status:** The Windows packaging approach has been prepared. Executable build verification, engineering validation, and corporate IT approval remain part of the pilot process.

---

## Project Status and Next Steps

**Current Stage: Engineering Pilot**

The application prototype and supporting engineering workflows have been developed.

The next stage focuses on:

1. Validating engineering calculations against original test measurements.
2. Testing application functionality with representative engineering files.
3. Evaluating usability and reporting consistency.
4. Validating Windows executable packaging.
5. Collecting engineer feedback.
6. Resolving defects before considering wider deployment.

TTIC is not currently presented as a certified measurement system or a production-validated enterprise application.

---

## Documentation

The repository also contains supporting materials covering the complete solution and its intended engineering usage.

- **End-to-End Engineering Presentation:** [View Presentation](documentations/TTIC_End_to_End_Engineering.pdf)

- **Engineering Pilot User Guide:** [View User Guide](documentations/TTIC_Engineering_Pilot_User_Guide.pdf)

---

## Source Code and Data Availability

This is a documentation-focused portfolio repository.

The following are intentionally not publicly distributed:

- Application source code.
- Original engineering test datasets.
- Windows executable packages.
- Internal development dependencies.

The repository is intended to demonstrate the solution's design, analytical capabilities, engineering workflows, and project development approach.

---

## Project Summary

The Thermal Test Intelligence Center demonstrates the application of **Python development, interactive visualization, engineering analytics, data processing, and reporting automation** to a practical engineering problem.

The project illustrates how analytical methods and application development can be combined to create a repeatable, engineer-focused decision-support workflow.

**From raw thermal logs to engineering insight.**
