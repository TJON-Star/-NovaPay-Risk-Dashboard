# NovaPay Technologies - GRC Risk Dashboard

> *20 fintech risks. 4 critical. Built in Power BI from a real GRC risk register.*

![Dashboard Preview](The%20Full%20Dashboard%20Overview.jpeg)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]()
[![Made with Power BI](https://img.shields.io/badge/Tool-Power%20BI-orange)]()
[![Framework: ISO 27001](https://img.shields.io/badge/Framework-ISO%2027001-blue)]()
[![Framework: PCI-DSS](https://img.shields.io/badge/Framework-PCI--DSS%20v4.0-red)]()
[![Framework: NDPR](https://img.shields.io/badge/Framework-NDPR-green)]()

---

## 👤 Author
**Taiwo Johnson** | GRC & Cybersecurity Risk Analyst
Tools: Power BI · DAX · ISO 27001:2022 · PCI-DSS v4.0 · NDPR

---

## 📋 Executive Summary

NovaPay Technologies processes payments across multiple African markets and is subject to ISO 27001:2022, PCI-DSS v4.0, and NDPR compliance obligations. This dashboard was built to give security and compliance leadership a single view of the organisation's risk posture - translating a live GRC risk register into executive-ready visuals.

The assessment identified **20 fintech risks** across 4 domains. Of those:
- **4 risks** are rated Critical and require immediate remediation
- **10 risks** are currently Open and assigned to control owners
- **6 risks** are In Treatment with documented remediation plans

The dashboard is designed to support both operational risk management and board-level reporting. It enables control owners to track treatment status, helps leadership prioritise resource allocation, and provides audit-ready evidence of ongoing risk management activity.

---

## 🔭 Scope

This assessment and dashboard cover the following:

| In Scope | Out of Scope |
|---|---|
| Information security risks across NovaPay's payment processing environment | Physical security of third-party data centre facilities |
| Risks mapped to ISO 27001:2022, PCI-DSS v4.0, and NDPR obligations | Full 93-control ISO 27001 Annex A assessment |
| 20 identified risks across 4 risk domains | Penetration testing findings or technical vulnerability details |
| Control ownership, treatment status, and residual risk tracking | Financial quantification of risk exposure |
| Governance, operational, compliance, and technology risk categories | Third-party vendor risk assessments |

---

## 📐 Assumptions

The following assumptions underpin the risk assessment and dashboard:

1. Risk ratings reflect the organisation's control environment at the time of assessment - they are not static and should be reviewed quarterly
2. Likelihood and impact scores are based on professional judgement informed by industry threat intelligence and the organisation's operational context - they are not derived from actuarial or quantitative loss modelling
3. Control effectiveness ratings reflect documented controls - controls that exist in policy but are not consistently operated are treated as partially effective
4. The 20 risks documented represent significant and prioritised risks - this is not an exhaustive inventory of all possible risks
5. Residual risk scores assume current controls are operating as documented - any control failure would increase residual risk
6. The dashboard reflects a point-in-time assessment - the risk landscape changes as the organisation grows, adds vendors, or enters new markets

---

## 📊 Risk Rating Criteria

All risks are scored using a **5×5 likelihood and impact matrix**, producing a risk score between 1 and 25.

### Likelihood Scale
| Score | Rating | Definition |
|---|---|---|
| 1 | Rare | May occur only in exceptional circumstances - less than once in 5 years |
| 2 | Unlikely | Could occur at some point - once in 3-5 years |
| 3 | Possible | Might occur at some point - once in 1-3 years |
| 4 | Likely | Will probably occur in most circumstances - once per year |
| 5 | Almost Certain | Expected to occur in most circumstances - multiple times per year |

### Impact Scale
| Score | Rating | Definition |
|---|---|---|
| 1 | Negligible | Minimal disruption - no regulatory notification required, no customer impact |
| 2 | Minor | Limited disruption - internal management only, minor reputational effect |
| 3 | Moderate | Significant disruption - regulatory notification may be required, moderate financial impact |
| 4 | Major | Serious disruption - regulatory breach, significant financial loss, customer impact |
| 5 | Critical | Catastrophic - regulatory sanction, major data breach, potential business failure |

### Risk Rating Matrix
| Risk Score | Rating | Treatment Requirement |
|---|---|---|
| 20-25 | 🔴 Critical | Immediate remediation required - escalate to CISO and board |
| 12-19 | 🟠 High | Treatment plan required within 30 days - assign control owner |
| 6-11 | 🟡 Medium | Treatment plan required within 90 days - monitor monthly |
| 1-5 | 🟢 Low | Accept or monitor - review quarterly |

### How Critical Risks Were Scored

The 4 critical risks in this dashboard all scored 20 or above on the 5×5 matrix. Each scoring decision is explained below:

| Risk | Likelihood | Impact | Score | Rationale |
|---|---|---|---|---|
| Unauthorised access to cardholder data environment | 4 - Likely | 5 - Critical | 20 | MFA gaps on privileged accounts make exploitation likely; PAN exposure triggers PCI-DSS breach notification and potential card brand fines |
| Unpatched critical vulnerabilities in payment processing systems | 4 - Likely | 5 - Critical | 20 | Exploit code publicly available for known CVEs; successful exploitation enables data exfiltration from live payment systems |
| Third-party API integration without security assessment | 4 - Likely | 5 - Critical | 20 | Unassessed integrations represent unquantified attack surface; supply chain compromise via third-party is a leading fintech attack vector |
| Absence of logging and monitoring across cloud environment | 5 - Almost Certain | 4 - Major | 20 | No monitoring means breaches cannot be detected - regulatory notification timelines cannot be met without detection capability |

---

## 📊 Risk Categories Covered

| Category | Description |
|---|---|
| 🔴 Critical Risks | High-likelihood, high-impact risks requiring immediate action |
| 🟠 Open Risks | Active risks assigned to control owners and under treatment |
| 📋 Compliance Risk | Exposure across ISO 27001, PCI-DSS v4.0, and NDPR domains |
| 🔗 Operational Risk | Process and control failures across business units |

---

## 🖼️ Dashboard Visuals

| File | Description |
|---|---|
| `The Full Dashboard Overview.jpeg` | Full GRC risk monitoring view |
| `Critical filter active.jpeg` | Breakdown of risks requiring immediate remediation |
| `Open status filter active.jpeg` | Active risks filtered by open status |
| `Image Breakdown.jpeg` | Risk breakdown by category and severity |
| `Image map.jpeg` | Risk map across business domains |

---

## 📁 Risk Register

The risk register provides detailed entries for each identified risk, including **category, likelihood, impact, and control owner**.

- Power BI File → `NovaPay_Risk_Dashboard.pbix`

---

## 🚀 How to Use

1. Download `NovaPay_Risk_Dashboard.pbix` and open in **Power BI Desktop**
2. Explore interactive charts and risk metrics
3. Browse the `.jpeg` files for dashboard screenshot previews
4. Review the risk register within Power BI for detailed entries

---

## 🛠️ Tech Stack

- **Tools:** Power BI, Excel, GitHub
- **Languages:** DAX
- **Frameworks:** ISO 27001:2022, PCI-DSS v4.0, NDPR

---

## 🎓 Lessons Learned

**1. Risk scoring without agreed criteria creates inconsistency**
Early versions of the risk register had inconsistent scoring because likelihood and impact were not formally defined. Establishing the 5×5 criteria matrix first - before scoring any risks - produced more defensible and consistent results.

**2. Ownership without accountability is decoration**
Assigning a control owner to a risk only works if the owner understands their responsibility and has the authority to act. Risks without empowered owners do not get treated - they get reviewed and re-listed.

**3. Dashboard design affects decision quality**
The visual hierarchy of the dashboard matters as much as the data. Placing critical risks at the top of the view and using consistent colour coding (red/amber/green) reduced the time senior stakeholders needed to orient themselves and reach decisions.

**4. PCI-DSS and ISO 27001 have significant overlap - map them together**
Treating PCI-DSS and ISO 27001 as separate compliance programs created duplication. Mapping controls to both frameworks simultaneously reduced the total number of controls needed and made evidence collection more efficient.

**5. Treatment status needs a clear definition**
Without a defined definition of "In Treatment" vs "Open," control owners reported risks as in treatment when remediation had not meaningfully started. Clear status definitions (Open, In Treatment, Resolved, Accepted) with documented evidence requirements resolved this.

---

## ⚠️ Limitations

1. **Point-in-time assessment** - The risk register reflects the control environment at the time of assessment. It does not update automatically as controls change or new threats emerge.
2. **Qualitative scoring only** - Risk scores are based on professional judgement, not quantitative loss modelling (e.g., FAIR methodology). Financial exposure figures are not included.
3. **20 risks assessed** - This dashboard does not claim to be an exhaustive risk inventory. Additional risks may exist that were not surfaced during the assessment period.
4. **Control effectiveness not independently verified** - Control ratings reflect documented and self-reported controls. Independent testing (penetration testing, internal audit) may surface gaps not visible in this assessment.
5. **No automated data refresh** - The Power BI dashboard requires manual data updates. Risk status does not refresh in real time.
6. **Vendor risks excluded** - Third-party and supply chain risks are not assessed in this dashboard. A separate vendor risk assessment would be required to address that exposure.

---

## 🏭 How This Project Would Change in Production

This portfolio project demonstrates the methodology and visual output of a GRC risk dashboard. In a production environment at a regulated fintech, the following changes would be essential:

| Portfolio Version | Production Version |
|---|---|
| Static Excel risk register manually updated | Risk register integrated with GRC platform (ServiceNow GRC, Vanta, or Drata) with real-time updates |
| Manual Power BI refresh | Automated data pipeline - risk register changes trigger dashboard refresh |
| 20 risks across 4 domains | Full risk inventory across all business units - typically 80-200+ risks at a regulated fintech |
| Qualitative scoring only | Hybrid qualitative and quantitative scoring - high-rated risks quantified using FAIR methodology |
| Single analyst assessment | Risk assessment conducted collaboratively with risk owners, validated by internal audit |
| No access controls on dashboard | Role-based access - executives see summary view, risk owners see their own risks, auditors see evidence |
| No audit trail | Full change log - every risk update, status change, and treatment action is timestamped and attributed |
| GitHub-hosted static file | Embedded in ISMS documentation system with version control and approval workflow |
| Manual regulatory mapping | Controls automatically mapped to ISO 27001, PCI-DSS, and NDPR - compliance gaps surfaced automatically |
| Reviewed annually | Reviewed quarterly minimum - triggered immediately by significant incidents, new products, or regulatory changes |

---

## 🗺️ v2.0 Roadmap

- [ ] Automate risk scoring
- [ ] Add predictive analytics
- [ ] Expand compliance frameworks support
- [ ] Integrate quantitative risk scoring (FAIR methodology)
- [ ] Add vendor risk module

---

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.
