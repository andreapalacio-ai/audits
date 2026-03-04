# Aston Insurance Group: Operations & Process Analysis

**Prepared for:** Adriana Rubio, Aston Insurance Group
**Date:** January 29, 2026
**Analyst:** Operations Growth Analyst

---

## Section 1: Business Understanding Summary

Aston Insurance Group is a 20+ year insurance brokerage serving the Hispanic community across Florida and Texas through two distinct brands. The primary brand (Aston Insurance Group) offers a full suite of products including life, health, accident, dental, vision, funeral, and international insurance, while the secondary brand (Seguro Con Obamacare) focuses specifically on ACA/Marketplace health insurance enrollment. The business operates with an estimated client base of approximately 3,000 customers, the majority of whom hold health insurance policies.

The current operational model is heavily phone-centric and manually intensive. Customer acquisition flows primarily through inbound phone calls and WhatsApp chat, with no online scheduling or self-service options available. The company uses ZOHO CRM but reports low proficiency and underutilization of its capabilities. A significant portion of agent time is consumed by reactive, repetitive tasks: manually checking the Healthcare.gov Marketplace portal for document requests, monitoring payment statuses for clients who have opted out of auto-pay, and sending individual follow-up text messages one-by-one. There is no systematic approach to lifecycle marketing (birthdays, age-based triggers for Medicare eligibility at 65), cross-selling existing clients, or automated renewal communications.

The business faces mounting pressure from rising customer acquisition costs, ACA policy changes that have contributed to client attrition, and the fundamental inefficiency of manual processes that prevent agents from focusing on revenue-generating activities. The leadership has expressed clear interest in automation for personalized bulk SMS/email communications, age-triggered outreach workflows, improved retention mechanisms, and systematic cross-selling to maximize lifetime value from their existing 3,000-client database.

---

## Section 2: Information Gaps

### Operations & Workflow
- No documented SOPs for agent daily workflows (policy checking, payment follow-up sequences)
- Unknown frequency and volume of Marketplace document requests per day/week
- Unclear how agents currently track which clients need follow-up (spreadsheet? ZOHO? memory?)
- No visibility into the policy checking process (which portal? how many clients checked daily?)
- Unknown time allocation per agent across different task categories

### Sales & Lead Management
- No data on current lead sources and their relative volume/quality
- Unknown lead-to-client conversion rate and sales cycle length
- Unclear how leads are currently distributed among agents
- No information on quoting process (manual comparisons? carrier portals?)
- Unknown average policies per client (cross-sell penetration)

### Client Data & Segmentation
- No breakdown of 3,000 clients by product type, tenure, or value tier
- Unknown percentage of clients on auto-pay vs. manual payment
- No visibility into client communication preferences (SMS vs. email vs. phone)
- Unclear how client birthdays and ages are currently tracked in ZOHO
- No data on client renewal rates by product line

### Technology & Systems
- No detailed ZOHO configuration information (which modules are active, what data is captured)
- Unknown integration capabilities between ZOHO and other systems
- No information on current phone system (VoIP? call tracking?)
- Unclear what data exists in ZOHO vs. scattered in spreadsheets/other locations
- No visibility into WhatsApp usage (personal accounts? WhatsApp Business? API?)

### Team Structure
- Unknown number of agents and their specializations
- No clarity on who handles Medicare vs. ACA vs. other products
- Unclear reporting structure and management oversight processes
- No information on current performance metrics or KPIs tracked

### Compliance & Constraints
- Unknown regulatory requirements for automated communications in insurance
- No information on carrier-specific compliance requirements
- Unclear data privacy considerations for the Hispanic immigrant community

---

## Section 3: Client Questionnaire

### A. Team & Organizational Structure

1. How many licensed agents currently work at Aston Insurance Group, and what are their primary product specializations (ACA, Medicare, Life, etc.)?

2. What does a typical agent's daily schedule look like? Please estimate hours spent on: policy status checking, payment follow-ups, inbound calls, outbound sales calls, administrative tasks.

3. Who is responsible for managing ZOHO CRM, and have any staff received formal training on the platform?

4. Do you have any dedicated staff for marketing, customer service, or administrative support separate from licensed agents?

### B. Current Processes - Policy Monitoring

5. How many client policies do agents check daily/weekly for Marketplace document requests? What is the typical volume of document requests found per day?

6. Walk me through the exact steps an agent takes when they discover a Marketplace document request. What happens from discovery to resolution?

7. How do agents currently track which policies have been checked and which still need attention? Is there a system or is it memory-based?

8. What percentage of your 3,000 clients are ACA/Marketplace policies vs. other product types?

### C. Current Processes - Payment Follow-Up

9. What percentage of clients are on auto-pay vs. manual payment?

10. How do agents currently identify which clients have missed or upcoming payments? What system or report do they use?

11. How many individual text messages are sent per day/week for payment follow-ups?

12. What is your current text messaging method (personal phone, business line, SMS platform)?

13. What is the typical sequence of follow-up attempts before a policy lapses? How many touchpoints over what timeframe?

### D. Sales & Lead Management

14. What are your current lead sources and approximate monthly volume from each (website calls, referrals, walk-ins, marketing campaigns)?

15. When a new lead calls in, what information is captured and where is it recorded?

16. What is your estimated lead-to-client conversion rate? How long does the typical sales cycle take?

17. How do you currently compare policy options for clients? Do you use carrier portals, quoting software, or manual comparisons?

18. What cross-selling currently happens? When a health insurance client is onboarded, is there a systematic process to offer life, dental, or other products?

### E. Client Database & ZOHO CRM

19. What client data fields are currently populated in ZOHO (name, DOB, phone, email, policy details, payment status, etc.)?

20. Are client birthdays and dates of birth reliably captured in ZOHO for all 3,000 clients?

21. How confident are you in the email and phone number accuracy in your database (estimate percentage)?

22. Which ZOHO modules/features are you currently using (Contacts, Deals, Campaigns, Workflows, etc.)?

23. Is there important client data stored outside of ZOHO (spreadsheets, paper files, email folders)?

### F. Communication & Engagement

24. What is your current email marketing activity? How often do you send emails and what tools do you use?

25. Do you have email templates or is each communication written from scratch?

26. Have clients provided consent for SMS marketing communications? How was this consent captured?

27. What languages do you communicate in, and does this vary by channel (phone vs. SMS vs. email)?

### G. Technology & Integrations

28. What phone system do you use? Is it VoIP, and does it integrate with any other software?

29. Is your WhatsApp widget connected to WhatsApp Business API, or is it routing to personal/business phone numbers?

30. What carrier portals or external systems do agents access daily?

31. Do you have any existing automation or workflows set up in ZOHO, even if basic?

### H. Metrics & Goals

32. What is your current client retention rate (percentage of clients who renew annually)?

33. What is your target for new client acquisition per month?

34. If you could free up agent time from manual tasks, what would you want them to focus on instead?

35. What does success look like 12 months from now? What specific outcomes would make this automation investment worthwhile?

---

## Section 4: Preliminary Process Map

| Process | Current State | Est. Time/Frequency | Dependencies | Automation Potential |
|---------|--------------|---------------------|--------------|---------------------|
| **Lead Capture** | Phone calls, WhatsApp chat; manual entry into ZOHO | Unknown volume; ~5-10 min per lead | Website, phone system, ZOHO | HIGH - Web forms, auto-capture, lead routing |
| **Lead Qualification** | Phone conversation with agent | ~15-30 min per lead | Agent availability | MEDIUM - Pre-qualification chatbot/forms |
| **Policy Quoting** | Manual carrier portal comparisons | Unknown; likely 20-45 min per quote | Carrier portals, agent expertise | MEDIUM - Quoting engine integration |
| **Client Onboarding** | Manual data entry, paperwork | Unknown | Carrier systems, ZOHO | MEDIUM - Digital forms, auto-population |
| **Marketplace Monitoring** | Manual daily checks of Healthcare.gov | High frequency; unknown time per agent | Healthcare.gov portal access | HIGH - API integration or RPA if available |
| **Document Request Resolution** | Agent contacts client, collects docs, uploads | Variable; ~30-60 min per case | Client responsiveness, portal access | MEDIUM - Automated alerts, client portal |
| **Payment Status Monitoring** | Manual checks of payment status | High frequency; unknown time | Carrier/marketplace portals | HIGH - Automated monitoring & alerts |
| **Payment Follow-Up (SMS)** | Individual texts sent one-by-one | Unknown volume; ~2-5 min each | Personal phone, client contact info | HIGH - Bulk SMS with personalization |
| **Birthday Outreach** | Not currently done | N/A | DOB data in CRM | HIGH - Simple automated workflow |
| **Medicare Age Trigger (65+)** | Not currently done | N/A | DOB data in CRM, Medicare specialist | HIGH - Age-based workflow trigger |
| **Cross-Sell Campaigns** | Not systematically done | N/A | Client product data, segmentation | HIGH - Automated nurture sequences |
| **Renewal Reminders** | Unknown current process | Annual per client | Policy expiration dates | HIGH - Automated reminder sequence |
| **Client Retention Engagement** | Not systematically done | N/A | Client history, engagement data | MEDIUM - Loyalty program, regular touchpoints |

---

## Section 5: Initial Observations

### Quick Wins (High Impact, Low Complexity)

1. **Automated Birthday Emails/SMS** - If DOB data exists in ZOHO, this can be implemented within days using native ZOHO workflows or a simple integration. Immediate goodwill builder with zero ongoing effort.

2. **Bulk SMS Platform Implementation** - Replacing one-by-one texting with a platform like Twilio, SimpleTexting, or ZOHO-integrated SMS will immediately save hours weekly. Payment reminders can be templated and sent in batches while appearing personalized.

3. **Medicare Age Trigger Workflow** - Simple ZOHO workflow to flag clients approaching 65 and auto-assign tasks to the Medicare specialist. Low-hanging revenue opportunity from existing client base.

4. **Online Appointment Scheduling** - Adding Calendly or similar to websites captures leads who prefer not to call. Integration with ZOHO ensures no manual entry. Can be live within a week.

5. **Email Drip Campaign for Cross-Selling** - Segment existing 3,000 clients by current products, create simple email sequences promoting complementary coverage. ZOHO Campaigns or Mailchimp integration makes this straightforward.

### Red Flags & Areas Requiring Deeper Discovery

1. **ZOHO Data Quality Concerns** - The admitted low proficiency with ZOHO suggests client data may be incomplete, inconsistent, or outdated. Any automation depends on reliable data. A data audit should be the first step before building workflows.

2. **Healthcare.gov Monitoring Bottleneck** - This is consuming significant agent time but automation options are limited by portal access constraints. Need to understand if API access is available or if this requires RPA, which increases complexity.

3. **SMS Consent & Compliance** - Automated SMS marketing requires documented consent (TCPA compliance). Need to verify if consent exists and is properly recorded before implementing bulk messaging.

4. **WhatsApp Architecture** - If WhatsApp is running through personal accounts rather than Business API, there are scalability and compliance limitations that will need addressing.

5. **Single Point of Failure Risk** - Heavy reliance on phone-based processes with apparent lack of documented procedures creates vulnerability if key staff are unavailable.

6. **Content Marketing Gap** - Blog not updated since 2020 indicates potential resource constraints or strategic neglect of digital presence. Automation won't solve underlying content/marketing capacity issues.

### Recommended Discovery Call Focus Areas

- Validate ZOHO data quality and completeness (especially DOB, email, phone accuracy)
- Understand the exact Healthcare.gov monitoring workflow and explore automation options
- Confirm SMS consent status for existing client base
- Clarify agent capacity and where freed time would be redirected
- Establish baseline metrics (retention rate, conversion rate, response times) to measure automation impact
- Identify budget constraints and timeline expectations

---

*This analysis is preliminary and based solely on the provided knowledge base document. A discovery call will be essential to validate assumptions, fill information gaps, and prioritize automation initiatives based on actual business constraints and goals.*
