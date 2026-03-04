# Aston Insurance Group: Operations Flowchart

**Prepared by:** Systems Architect
**Date:** February 12, 2026

---

## Company Operations & Automation Opportunity Map

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'fontSize': '14px'}}}%%
flowchart TB
    %% Style Definitions
    classDef critical fill:#FF6B6B,stroke:#CC0000,stroke-width:3px,color:#000
    classDef highROI fill:#4ECDC4,stroke:#00A896,stroke-width:3px,color:#000
    classDef mediumPriority fill:#FFE66D,stroke:#F4A800,stroke-width:2px,color:#000
    classDef standard fill:#95B8D1,stroke:#4A7C9B,stroke-width:2px,color:#000
    classDef automated fill:#DDA0DD,stroke:#8B008B,stroke-width:2px,color:#000
    classDef database fill:#B8B8B8,stroke:#666666,stroke-width:2px,color:#000
    classDef startend fill:#98D8AA,stroke:#2E7D32,stroke-width:2px,color:#000

    %% ============================================
    %% CLIENT ACQUISITION SUBGRAPH
    %% ============================================
    subgraph ACQUISITION["📞 CLIENT ACQUISITION"]
        direction TB
        START((("Client<br/>Contact")))
        REFERRAL["Referral Source<br/>📊 100% of leads<br/>⏱️ No active marketing"]
        INBOUND["Inbound Call<br/>📊 500+ calls/mo<br/>⏱️ 4 hrs/day team"]
        WHATSAPP["WhatsApp Inquiry<br/>📊 Volume unknown<br/>⚠️ API status TBD"]
        LEAD_CAPTURE["Manual Lead Entry<br/>📊 20-50 leads/mo<br/>⏱️ 5-10 min each"]

        START --> REFERRAL
        REFERRAL --> INBOUND
        REFERRAL --> WHATSAPP
        INBOUND --> LEAD_CAPTURE
        WHATSAPP --> LEAD_CAPTURE
    end

    %% ============================================
    %% CRM & DATA SUBGRAPH
    %% ============================================
    subgraph CRM["💾 CRM & DATA SYSTEMS"]
        direction TB
        ZOHO[("ZOHO CRM<br/>📊 3,000 clients<br/>📧 90% email accuracy<br/>📱 99% phone accuracy")]
        RINGCENTRAL[("RingCentral<br/>📞 Phone/SMS<br/>⚠️ NOT integrated")]
        EXCEL[("Excel Tracking<br/>📊 ~50 manual pay clients<br/>💰 $2,340/yr cost")]
        HEALTH_SHERPA[("Health Sherpa<br/>📊 ACA Platform<br/>⏱️ Daily access")]
        CARRIER_PORTALS[("Carrier Portals<br/>📊 Multiple logins<br/>⏱️ Monthly payment lists")]
    end

    %% ============================================
    %% ONBOARDING SUBGRAPH
    %% ============================================
    subgraph ONBOARDING["📋 CLIENT ONBOARDING"]
        direction TB
        INTAKE_CALL["Intake Call<br/>📊 20-50/mo<br/>⏱️ 10-60+ min"]
        NEEDS_ASSESS{{"Needs<br/>Assessment"}}
        ACA_PATH["ACA/Marketplace<br/>📊 90% of clients"]
        OTHER_PATH["Medicare/Life/Other<br/>📊 10% of clients"]
        HEALTHCARE_GOV["Healthcare.gov<br/>Plan Comparison<br/>⏱️ 20-45 min"]
        CONSENT_SEND["Send Consent<br/>via Cliq/Email<br/>⚠️ No SMS consent captured"]
        DOC_COLLECTION["Document Collection<br/>📊 Variable<br/>⏱️ 30-60 min/case"]
        APP_SUBMIT["Application<br/>Submission<br/>⏱️ 15-30 min"]

        INTAKE_CALL --> NEEDS_ASSESS
        NEEDS_ASSESS -->|"ACA"| ACA_PATH
        NEEDS_ASSESS -->|"Other"| OTHER_PATH
        ACA_PATH --> HEALTHCARE_GOV
        OTHER_PATH --> HEALTHCARE_GOV
        HEALTHCARE_GOV --> CONSENT_SEND
        CONSENT_SEND --> DOC_COLLECTION
        DOC_COLLECTION --> APP_SUBMIT
    end

    %% ============================================
    %% POLICY SERVICING SUBGRAPH
    %% ============================================
    subgraph SERVICING["🔧 POLICY SERVICING"]
        direction TB
        POLICY_VERIFY["Policy Verification<br/>📊 3,000 peak / 300 normal<br/>⏱️ 8-15 min each<br/>👤 Mery 100% FTE<br/>💰 $34,580/yr SAVINGS"]
        VERIFY_DECISION{{"Document<br/>Request?"}}
        DOC_REQUEST["Document Request<br/>Follow-up<br/>⏱️ 30-60 min/case"]
        PAYMENT_CHECK["Payment Status<br/>Check<br/>📊 Monthly carrier lists"]
        PAYMENT_DECISION{{"Payment<br/>Issue?"}}
        PAYMENT_FOLLOWUP["Payment Follow-up<br/>📊 45-80 clients/mo<br/>⏱️ 5-7 min each<br/>💰 $6,240/yr SAVINGS"]
        ADMIN_TASKS["Admin Tasks<br/>📊 100 tasks/mo<br/>⏱️ 25 min each<br/>👤 Yuliana 80%"]
        ID_REQUESTS["ID/Doctor List<br/>Requests<br/>📊 100/mo<br/>⏱️ 10 min each"]

        POLICY_VERIFY --> VERIFY_DECISION
        VERIFY_DECISION -->|"Yes"| DOC_REQUEST
        VERIFY_DECISION -->|"No"| PAYMENT_CHECK
        DOC_REQUEST --> PAYMENT_CHECK
        PAYMENT_CHECK --> PAYMENT_DECISION
        PAYMENT_DECISION -->|"Yes"| PAYMENT_FOLLOWUP
        PAYMENT_DECISION -->|"No"| ADMIN_TASKS
        PAYMENT_FOLLOWUP --> ADMIN_TASKS
        ADMIN_TASKS --> ID_REQUESTS
    end

    %% ============================================
    %% RENEWAL & RETENTION SUBGRAPH
    %% ============================================
    subgraph RETENTION["🔄 RENEWAL & RETENTION"]
        direction TB
        OE_PREP["Open Enrollment<br/>Preparation<br/>📅 Oct-Dec annually"]
        RENEWAL_CONTACT["Renewal Contact<br/>📊 3,000 clients<br/>⚠️ Not systematic"]
        RETENTION_CHECK{{"Client<br/>Renewing?"}}
        RENEWAL_COMPLETE["Renewal<br/>Complete<br/>📊 85-95% retention"]
        WINBACK["Win-back<br/>Process<br/>⚠️ Not defined"]

        OE_PREP --> RENEWAL_CONTACT
        RENEWAL_CONTACT --> RETENTION_CHECK
        RETENTION_CHECK -->|"Yes"| RENEWAL_COMPLETE
        RETENTION_CHECK -->|"No"| WINBACK
    end

    %% ============================================
    %% MISSING PROCESSES SUBGRAPH
    %% ============================================
    subgraph MISSING["❌ MISSING PROCESSES - HIGH ROI"]
        direction TB
        BIRTHDAY["Birthday Outreach<br/>⚠️ NOT DONE<br/>💰 Quick Win"]
        MEDICARE_TRIGGER["Medicare Age Trigger<br/>⚠️ NOT DONE<br/>💰 Revenue Opportunity"]
        EMAIL_MARKETING["Email Marketing<br/>⚠️ ZERO campaigns<br/>💰 $15,600/yr opportunity"]
        CROSSSELL["Cross-sell Campaigns<br/>⚠️ NOT systematic<br/>💰 Reduce 90% ACA concentration"]
        OUTBOUND_SALES["Outbound Sales<br/>⚠️ NOT DONE<br/>💰 After time freed"]
    end

    %% ============================================
    %% CONNECTIONS BETWEEN SUBGRAPHS
    %% ============================================
    LEAD_CAPTURE --> ZOHO
    ZOHO --> INTAKE_CALL
    APP_SUBMIT --> ZOHO
    APP_SUBMIT --> HEALTH_SHERPA
    POLICY_VERIFY --> HEALTH_SHERPA
    POLICY_VERIFY --> ZOHO
    PAYMENT_CHECK --> CARRIER_PORTALS
    PAYMENT_FOLLOWUP --> RINGCENTRAL
    PAYMENT_FOLLOWUP --> EXCEL
    ID_REQUESTS --> ZOHO
    RENEWAL_COMPLETE --> ZOHO
    ZOHO -.->|"Trigger<br/>Opportunity"| BIRTHDAY
    ZOHO -.->|"DOB Data<br/>Available"| MEDICARE_TRIGGER
    ZOHO -.->|"3,000 clients<br/>No campaigns"| EMAIL_MARKETING
    ZOHO -.->|"Product data<br/>exists"| CROSSSELL
    CROSSSELL -.->|"After automation<br/>frees time"| OUTBOUND_SALES

    %% ============================================
    %% END STATE
    %% ============================================
    RENEWAL_COMPLETE --> ENDSTATE((("Active<br/>Policy")))
    WINBACK --> ENDSTATE

    %% ============================================
    %% APPLY STYLES
    %% ============================================
    %% Critical (RED) - Compliance/Risk Issues
    class CONSENT_SEND,POLICY_VERIFY critical

    %% High ROI (GREEN) - Top Savings Opportunities
    class BIRTHDAY,MEDICARE_TRIGGER,EMAIL_MARKETING,PAYMENT_FOLLOWUP highROI

    %% Medium Priority (ORANGE)
    class DOC_REQUEST,ADMIN_TASKS,CROSSSELL,RENEWAL_CONTACT mediumPriority

    %% Standard (BLUE)
    class REFERRAL,INBOUND,WHATSAPP,LEAD_CAPTURE,INTAKE_CALL,HEALTHCARE_GOV,DOC_COLLECTION,APP_SUBMIT,PAYMENT_CHECK,ID_REQUESTS,OE_PREP,WINBACK,OUTBOUND_SALES standard

    %% Database (GRAY)
    class ZOHO,RINGCENTRAL,EXCEL,HEALTH_SHERPA,CARRIER_PORTALS database

    %% Start/End (GREEN)
    class START,ENDSTATE startend
```

---

## Legend

| Color | Meaning | Action Required |
|-------|---------|-----------------|
| 🔴 **Red** | Critical Risk / Compliance Issue | Immediate attention required |
| 🟢 **Teal** | High ROI Opportunity | Prioritize for automation |
| 🟡 **Yellow** | Medium Priority | Include in Phase 2 |
| 🔵 **Blue** | Standard Process | Monitor and optimize |
| 🟣 **Purple** | Already Automated | Maintain |
| ⬜ **Gray** | Database/System | Integration opportunity |

---

## Key Metrics Summary

### Current State Pain Points
- **Policy Verification**: 1 FTE (Mery) = 160 hrs/month during peak
- **Payment Follow-up**: 4-9 hrs/month manual SMS
- **No Marketing**: 0 email campaigns, 0 outbound calls
- **SMS Consent Gap**: Cannot legally do bulk marketing SMS

### Automation ROI Summary
| Process | Annual Savings | Implementation Cost |
|---------|---------------|-------------------|
| Policy Verification RPA | $34,580 | $8,000-$10,000 |
| Payment Follow-up Automation | $6,240 | $2,500-$3,500 |
| Email Marketing Launch | $15,600 (revenue) | $3,000-$4,000 |
| ZOHO Workflow Automation | $10,920 | $3,000-$4,000 |
| **Total** | **$67,340+** | **$18,500-$24,500** |

### Payback Period: **2.8 - 3.7 months**

---

## Recommended Implementation Phases

### Phase 1 (Days 1-30): Foundation
1. ✅ Add SMS consent capture to intake
2. ✅ Implement birthday automation in ZOHO
3. ✅ Implement Medicare age trigger (65)
4. ✅ Create SMS templates for payment reminders

### Phase 2 (Days 31-60): Integration
5. 🔄 RingCentral-ZOHO integration
6. 🔄 Replace Excel tracking with ZOHO
7. 🔄 Build email templates
8. 🔄 Launch first email campaign

### Phase 3 (Days 61-90): Optimization
9. 🚀 Deploy RPA for policy verification
10. 🚀 Document request workflow automation
11. 🚀 Client segmentation for campaigns
12. 🚀 KPI dashboard implementation

---

*This flowchart represents the complete operational view of Aston Insurance Group with automation opportunities highlighted for executive review.*
