# Aston Insurance Group - Complete Knowledge Base

**Last Updated:** February 12, 2026
**Status:** Client-Verified Information

---

## 1. COMPANY OVERVIEW

### Business Identity
- **Company Name:** Aston Insurance Group
- **Secondary Brand:** Seguro Con Obamacare
- **Years in Business:** 20+ years
- **Primary Market:** Hispanic community in the United States
- **Geographic Focus:** Florida and Texas
- **Client Base:** ~3,000 clients (90% ACA/Marketplace policies)

### Contact Information
| Brand | Website | Primary Contact | Phone |
|-------|---------|-----------------|-------|
| Aston Insurance Group | astoninsurancegroup.com | Adriana Rubio (adriana@astonlife.co) | 305-570-2122 |
| Seguro Con Obamacare | seguroconobamacare.com | Flor A. Rubio | FL: 305-395-7085, TX: 469-868-8877 |

### Products & Services
| Product Category | % of Business | Notes |
|-----------------|---------------|-------|
| ACA/Marketplace Health Insurance | 90% | Core business |
| Life Insurance (Vida) | ~10% combined | Secondary products |
| Short-Term Insurance (ST) | | |
| Dental Insurance | ~5 policies/month | 12-15 min per policy |
| Vision Insurance | | Often bundled with Dental |
| Medicare | Variable | Complex process, 40 min - 1+ hour |
| Travel Insurance (Viaje) | ~1 policy/month | 40-50 min per policy |

---

## 2. TEAM STRUCTURE

### Licensed Agents (3)
| Name | Specializations | Notes |
|------|-----------------|-------|
| Freddy Palacio | ACA, Life | Licensed agent |
| Andrea Palacio | ACA | Exclusive Florida Blue agent |
| Flor Rubio | ACA, Medicare, Travel, Dental, Vision | Licensed agent; works OE and OP periods |

### Administrative/Customer Service Staff
| Name | Products Handled | Schedule | Notes |
|------|------------------|----------|-------|
| Silvia C. Abadia | ACA, Medicare, Travel, Dental, Vision, Life | 8:00 AM - 1:00 PM (5 hrs) | 10% policy verification, 20% admin tasks, 40% inbound calls |
| Yuliana Rios | ACA, Dental, Vision | 8:00 AM - 5:00 PM (8 hrs) | 10% policy verification, 80% admin tasks |
| Mery | ACA, Dental, Vision | 8:00 AM - 5:00 PM (8 hrs) | Currently 100% policy verification (Feb 2026) |

### Seasonal/OE Staff
- Claudia Rubio - ACA (during Open Enrollment only)
- Natalia Palacio - ACA (during OP only)
- Flor Rubio - Additional ACA, Medicare, Travel, Dental, Vision (during OP)
- Application processors during OE: Juliana, Juan E, Andrea Bedoya, Paola
- Call/consent uploads during OE: Miguel

### Key Organizational Notes
- **No dedicated marketing staff**
- Customer service/admin is handled separately from licensed agents
- Staff schedules vary during Open Enrollment (OE) vs. rest of year
- Some seasonal staff have no established schedules

---

## 3. TECHNOLOGY STACK

### Current Systems
| System | Purpose | Integration Status |
|--------|---------|-------------------|
| ZOHO CRM | Contact management, alarms, document storage | Primary system, basic usage only |
| ZOHO Drive | Document storage | Active |
| ZOHO Cliq | Consent delivery | Active |
| ZOHO Email | Communication | Active |
| RingCentral | VoIP phone system, SMS | **NOT integrated** with other systems |
| WhatsApp Business | Customer communication | Manual use (API status unknown) |
| Health Sherpa | ACA Certified Platform, policy lists | External portal, daily access |
| Healthcare.gov | ACA policy verification, plan comparisons | External portal, manual verification |
| Individual Carrier Portals | Policy management, payment lists | Multiple systems, no integration |

### ZOHO Modules In Use
- CRM (Contacts)
- Drive (document storage)
- Alarm/reminder system
- Email
- Cliq (consent sending)

### ZOHO Modules NOT In Use
- Campaigns (email marketing)
- Workflows/Automation
- Advanced CRM features

### Data Quality Assessment
| Data Field | Confidence Level |
|------------|-----------------|
| Phone Numbers | 99% accurate |
| Email Addresses | 90% accurate |
| Dates of Birth | Reliable for all 3,000 clients |
| All client data centralized in ZOHO | Yes - no external spreadsheets for client master data |

---

## 4. CURRENT PROCESSES

### 4.1 Policy Verification Process

**Timing:**
- January-February: All policies verified (highest volume)
- Rest of year: Once monthly verification
- Currently (Feb 2026): Mery dedicated 100% to verification

**Time Per Verification:** 8-15 minutes depending on:
- Whether portal is already open
- Need for 2-factor verification (text + email)
- Searching by name vs. SSN

**Steps:**
1. Take client name from renewed client list
2. Search client info in ZOHO
3. Access corresponding Sherpa portal
4. Locate client using personal data
5. Review policy activity (agent changes, updates, market requests, pending documents)
6. Take action based on findings:
   - **Document request:** Call client → Send text → Set alarm for follow-up
   - **Agent change:** Call client → If authorized, process change → Call Marketplace for official authorization (new regulation)
   - **Upload documents:** Locate client → Attach documents → Log in ZOHO notes → Save to Drive

**Tracking Methods:**
- ZOHO alarms (primary)
- Excel spreadsheets (secondary)
- Monthly Sherpa lists for new document requests or agent changes

### 4.2 Payment Follow-Up Process

**Payment Distribution:**
| Payment Type | % of Clients |
|--------------|--------------|
| Automatic | 70% |
| Manual (agent-assisted) | 20% |
| Self-managed by client | 10% |

**Monthly Payment Lists:**
- Downloaded from each carrier around the 15th of each month
- ~10 minutes to download per carrier
- Lists contain 10-20 payments each (varies)
- January/February: Lists can exceed 50+ people due to renewals, company changes, auto-renewals

**Manual Payment Clients:**
- ~50 clients across all carriers who requested auto-pay but it failed
- Tracked in Excel, worked at beginning of each month

**Time Per Payment:** 5-7 minutes per client payment

**SMS Follow-Up Volume:**
- 1st of month (payment due): ~15 messages
- 15th of month (list work): ~30 messages (varies by list size)

**Grace Periods:**
- Payments: 15-30 days depending on carrier
- Documents: ~90 days (Marketplace deadline)

### 4.3 Sales Process

**Lead Sources:** Referrals only (no active marketing campaigns)

**Data Captured for New Prospects:**
- Name
- Address
- Date of birth
- Family group
- Persons needing coverage
- Social Security Number
- Immigration status (if needed for insurance)
- Family income
- Payment method

**All data recorded in ZOHO**

**Sales Cycle Time:** 10-15 minutes to 1+ hour depending on:
- Client's knowledge of health system
- Medical care needs
- Family group size
- Client personality

**Quoting Tools:**
- ACA: healthcare.gov/see-plans/#/
- Other products: Individual carrier platforms

**Cross-Selling:**
- During OE: Focus on ACA renewals only
- Rest of year: Other products offered

### 4.4 Medicare Process (Most Complex)

**Steps:**
1. Request Medicare ID from client
2. If client doesn't have ID: Create account on Medicare.gov together to download
3. Review client needs
4. Create plan comparison (including medications and doctors)
5. Client makes decision
6. Send consent (via text or email)
7. Wait 48 hours
8. Submit application (via text or email for signature)

**Time:** 40 minutes to 1+ hour for simple case (often longer)

**Special Case - Adriana's Clients:**
- Additional communication layer (Adriana → Flor → Client)
- Flor creates comparison in Excel
- Adriana reviews and explains to client
- Questions researched and answered
- Adriana sends final info to Flor for consent/application

### 4.5 Other Product Processes

**Travel Insurance:**
- Volume: ~1 policy/month
- Time: 40-50 minutes total (15 min conversation + process)

**Dental/Vision:**
- Volume: ~5 policies/month
- Time: 12-15 minutes per policy
- United policies require email creation
- Other carriers don't require email

### 4.6 Administrative Tasks

**Daily Admin Work:**
- Name changes
- Add/remove dependents
- Upload documents
- **Time per task:** Minimum 25 minutes
- **Volume:** ~5 policies/day (Yuliana)

**ID/Doctor List Requests:**
- Time: 10 minutes
- Volume: ~5/day

**1095 Forms (Jan-Feb only):**
- Time: 10 minutes
- Volume: ~10/day

**Time Allocation:**
- Silvia: 20% of day on admin
- Yuliana: 80% of day on admin

### 4.7 Inbound Calls

- Currently (early 2026): More than half the day
- Decreases in following months
- Call duration: 5 minutes to 1+ hour (if on conference with carrier)
- Time allocation: 40% of Yuliana and Silvia's day
- Recent metric: 46 hours over 6 days in February = ~4 hours/day average

### 4.8 Outbound Sales

- **Current status:** Not actively making sales calls
- Only occasional referral follow-ups

---

## 5. COMMUNICATION

### Language
- **Primary:** Spanish (all channels)

### Current Marketing Activity
- Email marketing: **NONE** (0 activity)
- Email templates: **NONE**
- SMS consent for marketing: **NOT captured**

### Communication Channels
| Channel | Tool | Usage |
|---------|------|-------|
| Phone | RingCentral | Primary for calls, SMS |
| Text/SMS | RingCentral | Payment reminders, client follow-up |
| WhatsApp | WhatsApp Business | Customer communication |
| Email | ZOHO Email | Consents, applications, documentation |

---

## 6. KEY METRICS

### Retention Rates
| Staff Member | Retention Rate |
|--------------|---------------|
| Silvia | 95% |
| Yuliana | 95% |
| Mery | 85% |

### Client Acquisition Goal
- Not specified by client

### Success Definition (12 months)
- Not specified by client
- **Stated priority:** Free up agent time for sales

---

## 7. SEASONAL PATTERNS

### Open Enrollment (OE) Period
- Highest activity period
- Additional seasonal staff brought in
- Focus: ACA renewals only
- No cross-selling during OE
- Longer hours, more staff
- January-February: Highest verification volume

### Off-Peak (OP) Period
- Regular operations
- Cross-selling of other products
- Policy verification once monthly
- Some seasonal staff (Flor, Natalia) still active

---

## 8. PAIN POINTS & GAPS IDENTIFIED

### Confirmed Pain Points
1. **Policy verification consuming full-time resource** - Mery at 100% currently
2. **Manual SMS sending one-by-one** - No bulk messaging capability
3. **No birthday outreach** - Despite having DOB data
4. **No Medicare age trigger** - Missing revenue opportunity
5. **No systematic cross-selling** - Only happens opportunistically off-season
6. **No email marketing** - Zero activity
7. **No automation in ZOHO** - All manual processes
8. **RingCentral not integrated** - Phone/CRM disconnect
9. **No SMS marketing consent captured** - TCPA compliance gap
10. **WhatsApp API status unknown** - May limit automation potential

### Critical Compliance Gap
- **SMS marketing consent not captured** - Must be addressed before bulk messaging

### Systems Not Talking
- RingCentral ↔ ZOHO (no integration)
- Carrier portals ↔ ZOHO (manual data transfer)
- Sherpa ↔ ZOHO (manual list processing)

---

## 9. AUTOMATION OPPORTUNITIES (PRIORITIZED)

### Tier 1: Quick Wins (High Impact, Low Complexity)
| Opportunity | Dependency | Estimated Impact |
|-------------|------------|------------------|
| Birthday SMS/Email automation | DOB data exists ✓ | Immediate goodwill |
| Bulk SMS for payment reminders | Need consent capture first | Hours saved weekly |
| Medicare age trigger (approaching 65) | DOB data exists ✓ | New revenue |
| ZOHO workflow for alarm/task automation | Basic ZOHO in place ✓ | Efficiency gain |

### Tier 2: Medium Complexity
| Opportunity | Dependency | Estimated Impact |
|-------------|------------|------------------|
| RingCentral-ZOHO integration | Technical setup | Call logging, efficiency |
| Email drip campaigns for cross-sell | Need to build templates | Revenue growth |
| Document request tracking system | ZOHO workflows | Replace Excel tracking |
| Automated policy verification alerts | May need RPA for portal access | Major time savings |

### Tier 3: Requires Investigation
| Opportunity | Blocker | Next Step |
|-------------|---------|-----------|
| Healthcare.gov automation | Portal access limitations | Investigate API/RPA options |
| WhatsApp automation | Unknown API status | Determine current setup |
| Sherpa integration | External system | Evaluate possibilities |

---

## 10. NEXT STEPS

### Immediate Actions Required
1. **Capture SMS marketing consent** - Add to intake process immediately
2. **Audit ZOHO workflows capability** - Determine what can be automated natively
3. **Clarify WhatsApp Business setup** - API or manual?
4. **Define success metrics** - Client didn't specify 12-month goals

### Questions Still Outstanding
1. What is the client acquisition goal per month?
2. What specific outcomes would make automation investment worthwhile?
3. Budget constraints and timeline expectations?
4. WhatsApp Business API status?

---

*This knowledge base consolidates all verified information from client questionnaire responses and initial research. It should be updated as new information becomes available.*
