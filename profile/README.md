# MedTranscribeAi

_Transcribe care. Optimize billing. Get paid faster._ 🩺✨

![MedTranscribeAi icon](../docs/assets/iOSiconMedTranscribe.png)

> **MedTranscribeAi** is an AI assistant for clinicians and providers that turns spoken encounters into structured **SOAP notes** with **ICD‑10** suggestions — and (as we roll out) checks payer rules in real time to **reduce denials**, prevent audits, and improve cash flow.

---

## TL;DR — Why this matters

Healthcare teams lose hours to typing, hunting codes, fixing denials, and chasing audits. We’re building one flow from **note → code → claim** that’s:

-   **Fast**: Dictate once; get a ready-to-review SOAP note in 5 minutes. ⏱️
-   **Accurate**: ICD‑10 suggestions aligned with the note’s content. 🎯
-   **Up‑to‑date**: Models trained on updated **CMS NCD/LCD** + commercial payer rules to prevent denials **before** claims go out. ✅
-   **Future‑proof**: EHR integrations, claims optimization, and compliance insights — all in one place. 🔄

---

## Quick links

-   📘 **User Documentation (start here)**

    -   Phase 1 – Real‑time Transcription & ICD‑10: [`docs/phases/phase-1-transcription.md`](../docs/phases/phase-1-transcription.md)
    -   Phase 2 – EHR Integration & Scheduling: [`docs/phases/phase-2-ehr-integration.md`](../docs/phases/phase-2-ehr-integration.md)
    -   Phase 3 – Real‑time Claims Optimization: [`docs/phases/phase-3-claims-optimization.md`](../docs/phases/phase-3-claims-optimization.md)
    -   Phase 4 – Fraud/Waste/Abuse & Compliance: [`docs/phases/phase-4-fraud-waste-abuse.md`](../docs/phases/phase-4-fraud-waste-abuse.md)

-   🧭 **Product Requirements Document (PRD)**: [`docs/PRD.md`](../docs/PRD.md)

-   💼 **Monetization**: [`docs/monetization.md`](../docs/monetization.md)

-   ⚖️ **Legal & Regulatory**: [`docs/legal-compliance.md`](../docs/legal-compliance.md)

-   🆚 **Comparative Analysis**: [`docs/comparative-analysis.md`](../docs/comparative-analysis.md)

---

## What problems we solve (today → tomorrow)

### 1) Documentation drag ✍️

**Problem:** Providers spend nights and weekends finishing notes.
**Solution:** **Phase 1** converts your speech into a structured **SOAP note** (Subjective, Objective, Assessment, Plan) — with **ICD‑10** suggestions — in minutes.

**Power feature: Transcription Preferences** 🎛️
Every clinician writes differently. Our **Transcription Preferences** let you “teach” the model how to write _your_ notes:

-   Define prompts for **Chief Complaint, HPI, Medications, Allergies, PMH, PSH, Family/Social History, ROS, Objective, Assessment, Plan** — and any sub‑sections you use.
-   Choose **narrative vs. bulleted** styles, required elements, phrasing, and headers.
-   Save per‑provider or per‑group presets.

_Example prompt ideas (you’ll set these in the app UI):_

```text
Chief Complaint → "Start with CC: and quote the patient’s words."
HPI → "Narrative paragraph covering onset, location, duration, severity, context, modifying factors, associated symptoms."
Medications → "Bulleted list; include drug, dose, route, frequency; mark nonadherence if documented."
ROS → "System-by-system bullets; use 'denies …' for pertinent negatives."
Plan → "Numbered steps; include orders, counseling, follow-up interval."
```

---

### 2) Copy‑paste chaos 🔁

**Problem:** External dictation tools create notes you still have to paste into the EHR.
**Solution:** **Phase 2** integrates with leading **EHRs** (e.g., Athenahealth, Epic). Pull today’s schedule into the app → pick a patient → dictate → **note & codes post back automatically**.

---

### 3) Denials whack‑a‑mole 💸

**Problem:** Denial trends are found **after** rejections — weeks later.
**Solution:** **Phase 3** adds a policy-trained engine (CMS **NCD/LCD** + commercial payers) to check documentation and codes **as you chart**, suggesting what to add or adjust — so claims pass the first time.

-   **Real‑time rule checks:** Frequency limits, required modifiers, prerequisite therapies, medical necessity language.
-   **Continuously updated:** Our models ingest **new CMS and payer updates** regularly, so manual coders aren’t left chasing rule changes.
-   **Outcome focus:** Target higher clean-claim rates and fewer resubmits.

---

### 4) Audit anxiety & compliance risk 🛡️

**Problem:** Fraud/Waste/Abuse patterns are caught retroactively.
**Solution:** **Phase 4** provides **real-time** compliance nudges for providers and a **dashboard** for compliance teams to spot outliers early — reducing clawbacks and protecting reputation.

---

## How it works (high level)

1. **Record** in the iOS app (during or after the encounter).
2. **Transcribe & structure** into SOAP; review/edit as needed.
3. **Suggest codes** aligned with the documentation.
4. _(Phase 2+)_ **Sync** to the EHR automatically.
5. _(Phase 3+)_ **Policy check** claim logic in real time; add missing elements.
6. _(Phase 4+)_ **Monitor** patterns for compliance and quality.

---

## Who it’s for

-   **Clinicians** who want to finish notes during clinic hours, not after.
-   **Billers/Coders** who prefer preventing denials to cleaning them up.
-   **Practice leaders** who want fewer write‑offs, faster cash, and lower audit risk.

---

## What’s shipping now vs. next

-   **Now (Phase 1)** ✅

    -   Real‑time transcription → SOAP
    -   ICD‑10 suggestions
    -   **Transcription Preferences** and model tuning to customize note style

-   **Next up** 🛣️

    -   **Phase 2:** EHR schedule sync & automatic note posting
    -   **Phase 3:** Real‑time claims optimization (CMS LCD/NCD + payer rules)
    -   **Phase 4:** FWA analytics, compliance dashboard, and in‑workflow nudges

See the full roadmap inside the **PRD** → [`docs/PRD.md`](../docs/PRD.md)

---

## Security & compliance 🔒

-   HIPAA‑ready design with encryption in transit & at rest.
-   Business Associate Agreement (BAA) during onboarding.
-   Minimal PHI on device; processing in secure cloud.
-   Audit logs currently online in production.

For details, see: [`docs/legal-compliance.md`](../docs/legal-compliance.md)

---

## Get involved

-   💬 **Questions / pilots:** [dev@medtranscribe.ai](mailto:dev@medtranscribe.ai)
-   ⭐ **Star this repo** to follow progress
-   🧩 **Contribute:** Open an issue with ideas, edge cases, or integration requests
-   📄 **PRD & specs:** [`docs/PRD.md`](../docs/PRD.md)

---

## Credits & status

Built by a team obsessed with saving clinicians time and helping practices get paid for the care they deliver. If you’re a provider, biller, or compliance lead who wants to shape this, we’d love to hear from you. 🙌

---

### Appendix: Repo map (suggested)

```
.
├─ README.md                      # ← You are here (org entry point)
├─ docs/
│  ├─ PRD.md
│  └─ phases/
│     └─ phase-1-transcription.md
│     └─ phase-2-ehr-integration.md
│     └─ phase-3-claims-optimization.md
│     └─ phase-4-fraud-waste-abuse.md
│  ├─ comparative-analysis.md
│  ├─ monetization.md
│  ├─ legal-compliance.md
│  ├─ bug-bounty.md
│  ├─ release-notes.md
│  └─ assets/
│     └─ iOSiconMedTranscribe.png
└─ ...
```
