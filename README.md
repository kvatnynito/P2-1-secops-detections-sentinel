# P2-1: Security Operations & Detection Engineering

## Overview

This repo is planned to document hands-on Security Operations (SecOps) and detection engineering work using Microsoft Sentinel.

It is intended to focus on detection rules, incident investigations, log analysis, and automation workflows used to identify and respond to suspicious activity in a simulated enterprise environment.

This project is part of Portfolio 2 and is planned as the next phase after completion of Portfolio 1, which focuses on lab infrastructure, telemetry pipelines, and investigation workflows built in Proxmox.

---

## Status

**Current state:** Planned  
**Execution state:** Not yet started  
**Prerequisite:** Portfolio 1 completion

This repo is being prepared in advance so that the project scope, folder structure, and expected deliverables are already defined before hands-on work begins.

---

## Planned Objectives

This project is intended to demonstrate practical SecOps and SIEM skills, including:

- writing custom detection rules
- building Microsoft Sentinel KQL queries
- performing incident investigations
- ingesting and analyzing Windows, Linux, and Sysmon logs
- documenting detection logic and investigation findings
- using automation or scripts to support detections and triage

---

## Planned Repository Structure

- `docs/` — reports, playbooks, investigation notes, diagrams, templates
- `scripts/` — Python, PowerShell, or Bash utilities used for enrichment or automation
- `lab/` — sample logs, test datasets, or supporting lab notes
- `.github/` — issue or pull request templates (optional)

---

## Planned Lab Setup

### Host Platform
This project is planned to use the Proxmox-based lab environment built in Portfolio 1.

### Planned Lab Systems
Potential systems for testing and log generation may include:

- Windows Server 2019
- Ubuntu 22.04
- Kali Linux

### Planned Network Components
- pfSense
- segmented lab networking carried over from Portfolio 1

### Planned Cloud Components
- Microsoft Sentinel
- Log Analytics Workspace
- Microsoft Defender for Cloud
- Azure AD / Entra ID

This environment is intended to combine the local Proxmox homelab with Azure trial or free-tier resources where possible.

---

## Planned Workflow

Once execution begins, the intended workflow for this repo is:

### 1. Generate test activity
Examples may include:

- failed login attempts
- suspicious PowerShell execution
- Sysmon event generation
- Linux authentication events
- network scans such as Nmap

### 2. Ingest or connect logs into Sentinel
Planned log sources may include:

- Windows Event Logs
- Sysmon logs
- Linux authentication logs
- custom or sample log sources

### 3. Build and test detection rules
Planned activities include:

- writing KQL-based analytics rules
- mapping detections to MITRE ATT&CK
- tuning alert logic
- validating expected alert behavior

### 4. Investigate triggered incidents
Planned activities include:

- confirming alerts fire as expected
- reviewing incidents in Sentinel
- documenting triage steps, findings, and conclusions
- saving investigation artifacts in the repo

---

## Planned Deliverables

This repo is expected to eventually include:

- KQL detection rules
- incident reports documenting triage and findings
- sample log data for reproducible testing
- diagrams showing log ingestion and detection flow
- screenshots of alerts, incidents, and investigation timelines
- enrichment or helper scripts used during analysis

---

## Planned Skill Areas

This project is intended to help build experience in:

- SIEM operations
- detection engineering
- KQL query writing
- log analysis across Windows, Linux, and Sysmon
- MITRE ATT&CK-aligned alerting
- incident triage and documentation
- cloud-native SecOps tooling in Azure

---

## Planned Next Steps

When work begins on this repo, the initial implementation focus will likely be:

- establish Sentinel workspace and basic data sources
- prepare sample logs or test event generation
- create first custom detections
- validate alert and incident workflow
- document repeatable investigation steps

Future expansion may include:

- additional detection rules for brute force, malware, and lateral movement
- Logic Apps / SOAR workflow integration
- enrichment scripts using sources such as VirusTotal or AbuseIPDB
- expanded log sources such as Apache or DNS logs
- threat-hunting workbooks or dashboards

---

## License

MIT — see `LICENSE`.
