# Awesome-Managed-Cloud-Detection-Response

## Top Managed Cloud Detection & Response Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on 24/7 Cloud MDR, Cloud-Native Threat Hunting & Self-Hosted CDR Tooling*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Managed Cloud Detection & Response**. These services and tools enable organizations to detect, investigate, and respond to threats targeting cloud infrastructure—control plane abuse, identity compromise, workload attacks, and data exfiltration—combining cloud-native visibility with human expertise to contain incidents before they spread.



**Examples** include CrowdStrike Falcon Complete Cloud Security, Wiz MDR (via partners), Arctic Wolf Cloud Detection, Expel Cloud MDR, Palo Alto Unit 42 Managed Cloud, Rapid7 Cloud MDR, eSentire Cloud Security, Sophos Cloud MDR, Red Canary Cloud Defense, and Secureworks Taegis Cloud (the category leaders).



**Open-source emphasis**: Managed Cloud Detection & Response is a domain where the **"managed" component is fundamentally a human service**—24/7 monitoring by expert analysts who investigate cloud threats on your behalf. No open-source project replicates that service. What open-source *does* provide is **cloud detection and response tooling that organizations can run themselves**: **Dredge** is the strongest active project—a Python CLI for cloud incident response and threat hunting across AWS, Kubernetes, GitHub, and GCP, with CloudTrail hunting across all regions, IAM/EC2/S3 containment actions, and forensics collection . **OpenCDR** provides an open-source, event-driven **Cloud Detection & Response data plane for AWS**, ingesting CloudTrail and GuardDuty events and delivering alerts to Slack, Discord, Email, Security Hub, Jira, or any webhook—with optional automated incident response . The critical caveat: **open-source gives you the tools, not the team**—managed cloud MDR is a service delivered by human analysts, and organizations without dedicated cloud security staff should evaluate MDR providers rather than attempting to self-manage with open-source tools alone.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon Complete Cloud Security](https://www.crowdstrike.com/)**  

  The **first fully managed cloud workload protection solution**, combining Falcon Cloud Security runtime protection with Falcon OverWatch managed threat hunting and the Falcon Complete MDR team . Features: **24/7 follow-the-sun coverage** with cloud defense, DFIR, and threat intelligence experts; **surgical remediation** averaging under 60 minutes to restore systems to pre-intrusion state without reimaging; **multi-cloud visibility** across AWS, Azure, and GCP without agents; and a **Breach Prevention Warranty** . **Best for organizations wanting fully managed cloud detection and response** with a financial guarantee—but it is a premium enterprise service.



- **[Wiz MDR (via partners)](https://www.wiz.io/)**  

  Wiz itself provides deep, graph-based cloud visibility; its **MDR offering is delivered through partners** like mnemonic (in the Wiz Integration Network) and Red Canary . Wiz surfaces cloud risks, vulnerabilities, identities, and runtime threats; partners operationalize these findings with 24/7 expert monitoring, prioritization, and guided remediation . **Best for organizations already using Wiz** wanting to add managed response through a partner ecosystem.



- **[Arctic Wolf Cloud Detection](https://arcticwolf.com/)**  

  MDR with **24x7 monitoring across networks, endpoints, identities, and cloud environments** . Integrates with Wiz via GraphQL APIs to ingest Issues, Detections, Cloud Config Findings, Exposed Resources, and Vulnerabilities—correlating cloud signals with endpoint, identity, email, and network telemetry for human-led investigation and prioritization . **Best for organizations wanting cloud detection integrated into broader MDR** with a Concierge Security Team.



- **[Expel Cloud MDR](https://expel.com/)**  

  MDR with cloud detection and response coverage across AWS, Azure, Google Cloud, and **Oracle Cloud Infrastructure (OCI)** . Features: **cloud-specific detections** tailored to each provider's service architecture and identity model (IAM policy abuse, anomalous API calls, compute misuse, data exfiltration); **AI-powered alert enrichment** linking user activity across the stack; **threat hunting in the cloud control plane**; and resilience recommendations . Expel also integrates with **Google SecOps** for customers using Google's cloud-native security platform . **Best for organizations wanting multi-cloud MDR** with deep cloud expertise—Expel has been securing cloud since its founding .



- **[Palo Alto Unit 42 Managed Cloud](https://www.paloaltonetworks.com/)**  

  Unit 42's Managed Detection and Response service, delivered as managed services with Cortex XDR/XSIAM as the underlying platform . Covers endpoints, network, cloud, and identity; Unit 42 experts provide 24/7 monitoring, proactive threat hunting, detailed threat reports, and continuous security posture improvement . **Best for Palo Alto Cortex customers** wanting Unit 42's frontline expertise managing their cloud and broader environment .



- **[Rapid7 Cloud MDR](https://www.rapid7.com/)**  

  Rapid7 MXDR extends SOC coverage into **AWS environments**, with triage, investigation, and response for critical **GuardDuty alerts** directly within the MDR service . Correlates AWS telemetry with global threat intelligence, monitors cloud identities and permissions for anomalous behavior, and provides AI-assisted triage with risk-aware context . **Best for AWS-centric organizations** wanting MDR integrated with Rapid7's CNAPP capabilities.



- **[eSentire Cloud Security](https://www.esentire.com/)**  

  eSentire's Atlas platform provides **Controlled Autonomy SecOps**, correlating signals across endpoints, network, identity, email, cloud, and SaaS with agentic AI operatives and human experts 24/7 . Features: **autonomous penetration testing** to preempt exposures; **response actions** including TCP disruption, host isolation, and user suspension; **200+ threat protections added daily**; and 95% tier-3 analyst validation alignment . **Best for organizations wanting an offense-informed MDR** that tests defenses proactively.



- **[Sophos Cloud MDR](https://www.sophos.com/)**  

  Fully managed MDR with an **Agentic SOC** providing 24/7 monitoring, threat hunting, and response across cloud infrastructure and workloads . **52% of cases resolved end-to-end by AI in an average of 89 seconds**, with human analysts overseeing AI and validating outcomes . Response modes include **Authorize** (Sophos handles containment), **Collaborate** (joint response), and **Notify Only** . **Best for Sophos customers** wanting cloud MDR with transparent AI/human collaboration.



- **[Red Canary Cloud Defense](https://redcanary.com/)**  

  MDR for cloud workloads, identities, SaaS applications, networks, and endpoints . Integrates with Wiz to investigate, enrich, and validate cloud security insights with **24x7 expert investigation**, correlating cloud threat data with endpoints, identities, and other domains . Provides validated, fully scoped threat detections with tailored response and remediation guidance . **Best for organizations wanting cloud MDR with deep cross-domain correlation**—nearly 1,000 organizations rely on Red Canary for MDR .



- **[Secureworks Taegis Cloud MDR](https://www.secureworks.com/)**  

  Taegis ManagedXDR with cloud coverage across AWS, Azure, GCP, and identity providers . Features: **24x7 threat monitoring, detection, investigation, and unlimited response**; 350+ integrations; 1-year data retention; **1 minute median time to detect, 5 minutes to remediate**; and **<90 second access to security analysts** via the Taegis console . Tiers include MDR, MDR Plus, and MDR Enhanced with additional investigation context and governance . **Best for organizations wanting a mature, open XDR-based MDR** with fast analyst access .



## Open-Source GitHub Projects



### Cloud Incident Response & Hunting CLIs (Dredge)



- **[Dredge](https://pypi.org/project/dredge-ir/)**  

  The **most capable open-source cloud incident-response and threat-hunting toolkit** available (Python library + CLI, `pip install dredge-ir`) . Supports **AWS, Kubernetes, GitHub, and GCP** (in progress) . **Killer feature**: **CloudTrail hunting across every enabled AWS region concurrently**—`LookupEvents` is a regional API, so a normal search only sees one region; Dredge fans out to all regions and merges results into one time-sorted timeline . Features: **AWS forensics** (S3 log collection, snapshots, flow logs); **AWS containment** (IAM, EC2, RDS, ECS, S3, Lambda, KMS); **Kubernetes hunt and containment** (RBAC, pods, nodes, NetworkPolicy); **GitHub audit-log hunting and containment**; and **baseline-deviation hunts** (e.g., flag events from IPs outside an allowlist) . **Best for incident responders and cloud security engineers** wanting scriptable, fast cloud IR—but it is a toolkit, not a managed service.



### Cloud Detection & Response Platforms (OpenCDR)



- **[OpenCDR](https://github.com/dbnz-io/opencdr)**  

  An **open-source, event-driven Cloud Detection & Response data plane for AWS** . One deployment protects one AWS account: ingests **CloudTrail and GuardDuty events**, evaluates configurable rules, correlates activity, and delivers alerts to **Slack, Discord, Email, AWS Security Hub, Jira, or any HTTPS webhook**—with **optional automated incident response** . Deploys via Serverless Framework (Node.js/Python); requires CloudTrail enabled for EventBridge event delivery . **Critical caveat**: automated response rules load with `response_module` stripped by default—you must explicitly review and arm them with `--with-response-modules` before they can take destructive action . **Best for AWS-centric organizations** wanting a self-hosted CDR foundation—but it is per-account infrastructure requiring deployment and rule tuning.



### Additional Strong Open-Source Options



- **Wazuh** — Open-source SIEM/XDR platform (GPLv2) with cloud workload agents and log analysis; can ingest cloud audit logs (CloudTrail, Azure Activity Logs, GCP Audit Logs) for detection . **Best for organizations wanting a unified SIEM foundation** that includes cloud telemetry—but it is not cloud-native CDR and requires significant tuning.

- **Prowler** — Open-source cloud security posture management (CSPM) tool for AWS, Azure, and GCP; **not a detection and response platform**, but useful for identifying misconfigurations and compliance gaps that CDR tools can then monitor . **Best for posture assessment** as a complement to CDR.



**Frameworks for building custom systems**: For **cloud incident response and hunting across AWS/K8s/GitHub**, Dredge provides the most capable open-source toolkit . For **event-driven cloud detection and response on AWS**, OpenCDR provides a deployable data plane . **No open-source project provides managed cloud detection and response**—that is a human service. Organizations requiring 24/7 cloud MDR should evaluate CrowdStrike Falcon Complete Cloud Security, Expel, Red Canary, Arctic Wolf, or other MDR providers rather than attempting to self-manage with open-source tools alone.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Managed cloud detection and response platforms handling cloud telemetry must comply with organizational security policies and privacy regulations; **self-hosted CDR tools require skilled operators**—Dredge and OpenCDR are powerful but demand cloud security expertise to configure and interpret.

- **Open-source cannot replicate managed cloud detection and response**—managed cloud MDR is a service delivered by human analysts 24/7 (CrowdStrike OverWatch, Expel SOC, Red Canary experts) . Open-source provides **tools (Dredge, OpenCDR)** but not the human expertise and continuous monitoring that define managed CDR. **OpenCDR's automated response is disabled by default** for good reason—arming it without review can cause destructive actions . Organizations without dedicated cloud security staff should evaluate MDR providers.

- Verify license terms for commercial use; Dredge is a PyPI package (check license) , and OpenCDR is open-source (check repository).



---



**Made for cloud security architects, incident responders, and organizations choosing their managed cloud detection and response strategy.**  

Let's make cloud detection and response more open at the tooling layer, but with clear eyes about the human expertise and 24/7 monitoring that managed services uniquely provide.
