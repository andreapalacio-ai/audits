# Aston Insurance Group
## Operations & Process Analysis Report

**Analysis Date:** February 12, 2026
**Status:** Based on Client-Verified Information
**Analyst:** Operations Growth Analyst

---

## Section 1: Business Understanding Summary

Aston Insurance Group is a well-established 20+ year insurance brokerage serving the Hispanic community across Florida and Texas, operating under two brands: the primary Aston Insurance Group (full product suite) and Seguro Con Obamacare (ACA-focused). The business maintains approximately 3,000 clients, with 90% holding ACA/Marketplace health insurance policies. The remaining 10% comprises life insurance, Medicare, dental, vision, travel, and short-term products. The operation runs with a lean team of 3 licensed agents (Freddy Palacio, Andrea Palacio, and Flor Rubio) supported by 3 administrative staff (Silvia, Yuliana, and Mery), with seasonal expansion during Open Enrollment periods. Revenue is heavily concentrated in ACA renewals, with cross-selling of ancillary products occurring only during off-peak periods.

The day-to-day operation is characterized by high manual effort and reactive workflows. Customer acquisition flows almost exclusively through referrals with zero active marketing—no email campaigns, no outbound sales calls, and no systematic lead generation. The customer service function consumes the majority of staff time: policy verification alone currently requires one full-time employee (Mery at 100%), while inbound calls average 4 hours daily across the team. Administrative tasks like dependent changes, document uploads, and ID requests absorb 80% of Yuliana's workday. Communication happens primarily in Spanish via RingCentral (phone/SMS) and WhatsApp Business, with all client data centralized in ZOHO CRM—though the platform is severely underutilized, with no workflows, no automations, and no email marketing modules active.

The technology ecosystem reveals significant integration gaps that multiply manual work. ZOHO CRM operates as an isolated contact database rather than an automation hub. RingCentral handles all phone and SMS communication but has no integration with ZOHO, meaning call logs and SMS history exist separately from client records. The team accesses multiple external portals daily—Health Sherpa for ACA policy management, Healthcare.gov for verification and quoting, and individual carrier portals for payment lists—all requiring manual data transfer. Despite these inefficiencies, the business maintains strong retention rates (85-95% depending on staff member) and has high-quality client data (99% phone accuracy, 90% email accuracy, reliable DOB for all 3,000 clients), creating a solid foundation for automation initiatives.

---

## Section 2: Information Gaps

### Strategic & Financial
- Budget constraints and investment capacity for automation tools
- Specific 12-month success metrics (revenue targets, time savings goals)
- Monthly client acquisition targets
- Revenue breakdown by product line
- Cost per acquisition (current referral-only model)
- Lifetime value per client by product type

### Technology & Infrastructure
- WhatsApp Business configuration (API-connected or manual?)
- ZOHO subscription tier (which features are available?)
- RingCentral plan details (API access available?)
- Health Sherpa API capabilities (if any)
- Number of carrier portals accessed and login credentials management

### Process Timing & Volume
- Exact number of carriers requiring monthly payment list downloads
- Volume of document requests per month (outside Jan-Feb peak)
- Average policies per client (cross-sell penetration rate)
- Lead-to-client conversion rate
- Time spent on carrier conference calls (included in 4-hour call average?)

### Compliance & Legal
- Current consent language used during client intake
- How/where client consent is stored (if at all)
- HIPAA compliance procedures for document handling
- State-specific insurance communication regulations

### Workflow Documentation
- Escalation procedures when client doesn't respond to follow-ups
- Decision criteria for prioritizing which clients to contact first
- Quality control process for policy verification
- Handoff procedures between admin staff and licensed agents

---

## Section 3: Follow-Up Questions

### A. Strategic Priorities

1. What is your target number of new clients per month for 2026?

2. If automation freed up 20 hours/week of staff time, would you redirect that time to outbound sales, improving service quality, or reducing headcount?

3. What budget range are you considering for automation tools and implementation (monthly or one-time)?

4. Are there specific revenue targets for cross-selling (life, dental, Medicare) that would define success?

### B. Technology Clarification

5. Can you confirm your ZOHO subscription tier? (Free, Standard, Professional, Enterprise?)

6. For WhatsApp Business: Is it the free app on a phone, or do you have WhatsApp Business API access through a provider?

7. Does your RingCentral plan include API access for integration with other systems?

8. How many different carrier portals do your staff log into daily? Can you list them?

### C. Process Details

9. When a client doesn't respond to document request follow-ups after the initial call and text, what is the escalation sequence? How many attempts before the case is flagged as at-risk?

10. For the ~50 manual payment clients tracked in Excel: What information is tracked (name, amount due, carrier, due date, attempt history)?

11. During policy verification, how do you prioritize which clients to check first? Is there a risk-scoring system?

12. What happens when a policy lapses due to non-payment despite follow-up attempts? Is there a win-back process?

### D. Compliance Requirements

13. During client intake, do you currently read or document any consent language regarding communication preferences (calls, texts, emails)?

14. Where is client consent stored if it is captured?

15. Are there any carrier-specific rules about how/when you can contact clients about their policies?

### E. Seasonal Operations

16. During Open Enrollment, what is the approximate daily call volume per staff member?

17. How far in advance do you begin contacting clients about renewals before OE begins?

18. What triggers the decision to bring on seasonal staff vs. working overtime with core team?

---

## Section 4: Preliminary Process Map

### 4.1 Core Business Processes

| Process | Owner | Frequency | Time/Instance | Monthly Volume | Monthly Hours | Dependencies | Automation Potential |
|---------|-------|-----------|---------------|----------------|---------------|--------------|---------------------|
| **Policy Verification** | Mery (100%) | Daily (Jan-Feb), Monthly (rest) | 8-15 min | ~3,000 (peak) / ~300 (normal) | 160 hrs (peak) / 40 hrs | ZOHO, Health Sherpa, Healthcare.gov | 🔴 HIGH - RPA candidate |
| **Payment Follow-Up** | Silvia, Yuliana | Monthly (1st & 15th) | 5-7 min | ~45-80 clients | 4-9 hrs | Carrier portals, RingCentral, Excel | 🔴 HIGH - Bulk SMS + ZOHO workflow |
| **Inbound Call Handling** | Silvia, Yuliana | Daily | 5 min - 1+ hr | ~500+ calls | 80+ hrs | RingCentral | 🟡 MEDIUM - Call routing, IVR |
| **Admin Tasks (changes, docs)** | Yuliana (80%) | Daily | 25 min | ~100 tasks | 42 hrs | ZOHO, Carrier portals | 🟡 MEDIUM - Template automation |
| **ID/Doctor List Requests** | Admin team | Daily | 10 min | ~100 requests | 17 hrs | ZOHO | 🟢 LOW - Self-service portal |
| **1095 Form Processing** | Admin team | Jan-Feb only | 10 min | ~200 forms | 33 hrs | ZOHO | 🟢 LOW - Batch processing |
| **New Client Intake** | Licensed agents | As needed | 10-60+ min | ~20-50 (est.) | 10-50 hrs | ZOHO, Healthcare.gov | 🟡 MEDIUM - Digital forms |
| **Medicare Enrollment** | Flor Rubio | As needed | 40 min - 2+ hrs | ~5-10 (est.) | 10-20 hrs | Medicare.gov, Excel, ZOHO | 🟡 MEDIUM - Workflow automation |
| **Dental/Vision Sales** | Admin team | As needed | 12-15 min | ~5 policies | 1-1.5 hrs | Carrier portals | 🟢 LOW - Low volume |
| **Travel Insurance** | Flor Rubio | Rare | 40-50 min | ~1 policy | <1 hr | Carrier portal | 🟢 LOW - Low volume |

### 4.2 Missing Processes (Not Currently Executed)

| Process | Current State | Impact of Gap | Automation Potential |
|---------|---------------|---------------|---------------------|
| **Birthday Outreach** | Not done | Lost engagement opportunity | 🔴 HIGH - Simple ZOHO workflow |
| **Medicare Age Trigger (65)** | Not done | Lost revenue opportunity | 🔴 HIGH - Simple ZOHO workflow |
| **Email Marketing** | Zero activity | No nurturing, no cross-sell | 🔴 HIGH - ZOHO Campaigns |
| **Outbound Sales Calls** | Not done | No proactive growth | 🟡 MEDIUM - After time freed |
| **Renewal Reminder Campaign** | Not systematic | Reactive renewals only | 🔴 HIGH - ZOHO workflow |
| **Client Satisfaction Surveys** | Not done | No feedback loop | 🟢 LOW - After basics |
| **Referral Program** | Informal only | Untapped growth channel | 🟡 MEDIUM - After infrastructure |

### 4.3 Process Dependencies Map

```
┌─────────────────────────────────────────────────────────────────────┐
│                        CLIENT LIFECYCLE                              │
├─────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ACQUISITION          ONBOARDING           SERVICING        RENEWAL  │
│  ───────────          ──────────           ─────────        ───────  │
│                                                                      │
│  Referral ──┬──► Intake Call ──► ZOHO Entry ──► Policy Verification │
│             │         │              │                │              │
│  (No other  │         ▼              ▼                ▼              │
│   sources)  │    Healthcare.gov  Documents ──► Health Sherpa        │
│             │    Plan Comparison    to Drive         │               │
│             │         │              │                ▼              │
│             │         ▼              │         Payment Follow-up     │
│             │    Consent Sent       │         (if needed)            │
│             │    (Cliq/Email)       │                │               │
│             │         │              │                ▼              │
│             │         ▼              │         Admin Requests        │
│             │    Application ◄──────┘         (ID, docs, changes)   │
│             │         │                              │               │
│             │         ▼                              ▼               │
│             │    Carrier Portal              Inbound Calls           │
│             │    Submission                  (RingCentral)           │
│             │         │                              │               │
│             │         ▼                              │               │
│             └──► Active Policy ◄─────────────────────┘               │
│                       │                                              │
│                       ▼                                              │
│               [NO SYSTEMATIC                                         │
│                CROSS-SELL OR                                         │
│                BIRTHDAY/AGE                                          │
│                TRIGGERS]                                             │
│                       │                                              │
│                       ▼                                              │
│               OE Renewal Contact ──► Repeat Cycle                    │
│                                                                      │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Section 5: Initial Observations

### 🟢 Quick Wins (Implement Within 30 Days)

| Opportunity | Effort | Impact | Prerequisites | Est. Time Savings |
|-------------|--------|--------|---------------|-------------------|
| **1. Birthday SMS/Email Automation** | Low | High (engagement) | ZOHO workflow setup | Goodwill, not time |
| **2. Medicare Age Trigger (approaching 65)** | Low | High (revenue) | ZOHO workflow + task assignment | New revenue stream |
| **3. Bulk SMS for Payment Reminders** | Low | High | Consent capture process first | 3-5 hrs/month |
| **4. Renewal Reminder Workflow** | Low | Medium | ZOHO workflow | Proactive vs. reactive |
| **5. Document Request Follow-up Automation** | Medium | High | ZOHO workflow + SMS integration | 5-10 hrs/month |

**Recommended First Action:** Implement birthday and Medicare age triggers in ZOHO—these require no consent changes, use existing data, and demonstrate immediate value with minimal effort.

### 🟡 Medium-Term Opportunities (60-90 Days)

| Opportunity | Effort | Impact | Blocker to Resolve |
|-------------|--------|--------|-------------------|
| **RingCentral-ZOHO Integration** | Medium | High | Verify API access on both platforms |
| **Email Drip Campaigns (Cross-Sell)** | Medium | High | Build templates, segment clients by product |
| **Payment Tracking Dashboard** | Medium | Medium | Replace Excel with ZOHO reports |
| **Client Self-Service Portal** | Medium | Medium | Evaluate ZOHO Portal or alternatives |
| **Standardized SMS Templates** | Low | Medium | Create library, train staff |

### 🔴 Red Flags Requiring Immediate Attention

| Issue | Risk Level | Recommended Action |
|-------|------------|-------------------|
| **No SMS marketing consent captured** | HIGH (Legal) | Add consent checkbox to intake process immediately; cannot do bulk SMS marketing without it |
| **Policy verification consuming 1 FTE** | HIGH (Operational) | Investigate RPA for Health Sherpa/Healthcare.gov; this is unsustainable |
| **Zero marketing activity** | MEDIUM (Growth) | Client base is static; referral-only model limits growth ceiling |
| **RingCentral not integrated** | MEDIUM (Efficiency) | All call context lost; agents can't see call history in CRM |
| **WhatsApp API status unknown** | MEDIUM (Scalability) | If manual-only, cannot automate WhatsApp communications |
| **Mery's 85% retention vs. 95% for others** | MEDIUM (Quality) | Investigate cause—different client segment? Training gap? |

### 📊 Estimated Time Recovery Potential

| Process | Current Monthly Hours | Post-Automation Est. | Savings |
|---------|----------------------|---------------------|---------|
| Payment Follow-Up | 4-9 hrs | 1-2 hrs | 3-7 hrs |
| Birthday/Age Triggers | 0 (not done) | 0 (automated) | Revenue gain |
| Document Request Tracking | 10+ hrs (Excel) | 2-3 hrs | 7+ hrs |
| Policy Verification (with RPA) | 160 hrs (peak) | 40-80 hrs | 80-120 hrs |
| **Total Potential Monthly Savings** | | | **90-134 hrs** |

### 🎯 Recommended Implementation Sequence

**Phase 1 (Days 1-30): Foundation**
1. Add SMS consent capture to intake process
2. Implement birthday automation in ZOHO
3. Implement Medicare age trigger (65) in ZOHO
4. Create standardized SMS templates for payment reminders

**Phase 2 (Days 31-60): Integration**
5. Integrate RingCentral with ZOHO (if API available)
6. Replace payment Excel tracking with ZOHO reports
7. Build email templates for cross-sell campaigns
8. Launch first email nurture sequence to existing clients

**Phase 3 (Days 61-90): Optimization**
9. Evaluate RPA options for policy verification
10. Implement document request workflow automation
11. Create client segmentation for targeted campaigns
12. Establish KPI dashboard for ongoing monitoring

---

## Appendix: Key Metrics Summary

| Metric | Current Value | Target (Suggested) |
|--------|---------------|-------------------|
| Client Base | ~3,000 | Track growth monthly |
| ACA Concentration | 90% | Reduce to 80% via cross-sell |
| Retention Rate | 85-95% | Standardize to 95%+ |
| Email Marketing | 0 campaigns | 2-4 campaigns/month |
| Outbound Sales Calls | 0 | TBD after time freed |
| SMS Consent Captured | 0% | 100% of new clients |
| Phone Data Accuracy | 99% | Maintain |
| Email Data Accuracy | 90% | Improve to 95% |
| Policy Verification FTE | 1.0 | Reduce to 0.25-0.5 |

---

*This analysis is based on client-verified information from the completed questionnaire. Implementation recommendations should be validated against budget constraints and timeline expectations in follow-up discussions.*
