# Product Requirements Document (PRD)

## People & Business Intelligence Platform

**Document status:** Initial Draft  
**Version:** 0.1  
**Product category:** B2B SaaS · Business Intelligence · AI Research  
**Development stage:** Product Discovery and MVP Planning  
**Last updated:** 29 October 2026

---

## 1. Executive Summary

The People & Business Intelligence Platform is a proposed B2B SaaS product designed to help professionals research high-profile businesspeople, understand their publicly documented business interests, explore relationships between people and organisations, and prepare for important business meetings.

The platform aims to organise fragmented information from appropriate public and licensed sources into structured, searchable, source-linked intelligence profiles.

Unlike a general-purpose AI chatbot, the platform will focus on professional research workflows, connected business information, source transparency, and reusable intelligence profiles.

The product will initially target selected business professionals in Dubai and other international markets.

## 2. Problem Statement

Researching a high-profile businessperson can require reviewing multiple websites, company announcements, interviews, news articles, public records, and other sources.

This process can be time-consuming, fragmented, and difficult to verify. Information may be outdated, conflicting, or disconnected from relevant companies and business relationships.

Professionals need a more efficient way to collect, verify, organise, and use relevant business intelligence before important meetings and commercial decisions.

The initial customer research phase will validate how frequently this problem occurs, how customers currently solve it, and whether they are willing to pay for a dedicated solution.

## 3. Product Vision

To build a professional intelligence platform that connects people, businesses, publicly disclosed investments, and documented professional relationships in one searchable workspace.

The long-term vision is to help business professionals move from fragmented research to evidence-based business preparation.

## 4. Target Users

### 4.1 Primary customer segments under evaluation

- Private aviation and luxury yacht brokers.
- Luxury real estate advisers.
- Family offices and investment professionals.
- Strategic partnerships and business development teams.
- Professional advisers working with business leaders.

### 4.2 Initial target market

Dubai will be explored as the initial customer discovery market because the founders may have access to relevant business professionals there.

The initial customer segment will be selected after interviews and paid-pilot validation.

### 4.3 User roles

- **Subscriber:** Searches profiles, reviews intelligence, and generates research briefs.
- **Team member:** Uses shared research within an organisation, where team access is supported.
- **Administrator:** Manages access, subscription settings, and permitted product configuration.

## 5. Jobs to Be Done

The platform should help a professional:

1. Research a person before an important business meeting.
2. Understand their documented career and business affiliations.
3. Find publicly reported investments and relevant transactions.
4. Explore documented relationships between people and companies.
5. Review recent, relevant business developments.
6. Generate a concise research brief with supporting sources.
7. Save profiles for future reference.

## 6. Proposed MVP Scope

### 6.1 People Search

Users can search for a person by name and, where available, refine results using company, role, or industry.

Requirements:

- Display relevant search results.
- Distinguish people with similar names.
- Link each result to its profile.
- Show a useful message when no match is found.

### 6.2 Professional Intelligence Profiles

Each profile may include:

- Professional biography.
- Career and role timeline.
- Company affiliations.
- Publicly disclosed investment activity.
- Relevant business announcements.
- Public interviews and statements.
- Source links and publication dates.

Information must be included only when an appropriate source is available. Unknown information must not be presented as fact.

### 6.3 Company and Investment Intelligence

Users can explore organisations associated with a person and review available information about publicly disclosed investments and transactions.

Requirements:

- Identify the relevant company or organisation.
- Distinguish current and former affiliations where evidence permits.
- Record the source and date of each material claim.
- Distinguish completed transactions from reported intentions.
- Display uncertainty where the evidence is incomplete.

The MVP will not claim access to confidential portfolios or undisclosed investments.

### 6.4 Business Relationship Explorer

Users can explore documented connections between people and organisations.

Examples include:

- Founder and company relationships.
- Publicly disclosed investor and company relationships.
- Documented board and executive roles.
- Publicly announced investment relationships.

The platform must distinguish confirmed relationships from inferred associations.

### 6.5 AI Research Assistant

Users can ask questions about the available intelligence records.

Requirements:

- Generate answers grounded in retrieved information.
- Link important factual claims to supporting sources.
- Indicate when evidence is insufficient.
- Avoid inventing relationships, investments, or personal details.
- Distinguish facts, estimates, and unverified reports.

### 6.6 Meeting Brief Generator

Users can generate a concise professional briefing for a selected person.

The briefing should contain:

- Professional background.
- Relevant business interests.
- Documented company relationships.
- Recent relevant public developments.
- Potentially useful professional conversation topics.
- Source links and the dates of relevant information.

Conversation suggestions must be based on documented professional information, not speculative assumptions about a person's private life or preferences.

### 6.7 Saved Profiles

Users can save profiles for future research and access them through their account.

Automated alerts and advanced monitoring will be evaluated for a later release.

## 7. Features Outside the Initial MVP

The first release will not include:

- A comprehensive database of every wealthy individual.
- Confidential or non-public financial information.
- Personal addresses or invasive personal profiling.
- Predictions about undisclosed investments.
- Automated financial recommendations.
- Full CRM functionality.
- A native mobile application.
- Complex enterprise integrations.
- Unverified wealth rankings.
- Guaranteed coverage of every company or transaction.

These exclusions will help keep the initial release focused and manageable.

## 8. User Journey

### Primary workflow

1. The user signs in.
2. The user searches for a businessperson.
3. The platform displays matching people.
4. The user opens a professional profile.
5. The user reviews career history, companies, disclosed investments, and source links.
6. The user explores relevant business relationships.
7. The user generates a meeting briefing.
8. The user saves the profile for later use.

The workflow should be designed for desktop use first, with responsive support for smaller screens.

## 9. Data Requirements and Source Quality

The platform will use appropriate public sources and licensed data sources, subject to applicable terms and permissions.

Potential source categories include:

- Official company websites and announcements.
- Regulatory filings and public records.
- Company leadership pages.
- Public interviews and statements.
- Reputable news publications.
- Permitted commercial data providers.

Each material data point should record, where applicable:

- Person or organisation identifier.
- Claim or relationship type.
- Source URL or source reference.
- Publication date.
- Date the information was retrieved.
- Relevant event date.
- Verification status.
- Confidence or uncertainty label.

Source information must be retained in a form that supports verification and correction.

## 10. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | Search for people | Must have |
| FR-02 | Display professional profiles | Must have |
| FR-03 | Display source links and dates | Must have |
| FR-04 | Show company affiliations | Must have |
| FR-05 | Display supported investment disclosures | Must have |
| FR-06 | Generate source-grounded AI answers | Must have |
| FR-07 | Generate meeting briefs | Must have |
| FR-08 | Save profiles | Should have |
| FR-09 | Explore business relationships visually | Should have |
| FR-10 | Monitor changes and send alerts | Future consideration |

## 11. Non-Functional Requirements

### Accuracy and reliability

- Important factual claims must have supporting sources.
- The system must handle conflicting information transparently.
- Missing data must not be silently replaced with fabricated details.

### Performance

- Search and profile pages should respond quickly under expected pilot usage.
- AI research tasks should provide a clear loading state and handle failures gracefully.
- Performance targets will be finalised after selecting the data sources and architecture.

### Security

- Authentication and access control must be implemented appropriately.
- Secrets and API keys must not be exposed in client-side code or public repositories.
- Administrative functions must be protected.
- Customer information must be separated from public profile data.

### Usability

- The interface should use clear, professional English.
- Sources and uncertainty labels should be easy to understand.
- Users should be able to move from a search result to a useful briefing with minimal friction.

## 12. Privacy, Compliance and Responsible Use

The platform will be designed to support lawful professional research.

Requirements include:

- Assess the legal basis and permitted use of personal data.
- Respect data-provider licences, source terms, and applicable restrictions.
- Collect and retain only necessary information.
- Provide appropriate procedures for corrections and removal requests.
- Apply suitable access controls and retention policies.
- Avoid private or confidential information obtained without authorisation.
- Review relevant UAE, UK, and other applicable legal obligations before launch.

Public availability alone does not establish unrestricted rights to collect, reproduce, or commercially use information.

## 13. Initial Technical Direction

The proposed technology stack is:

- **Frontend:** Next.js.
- **Database:** PostgreSQL through Supabase.
- **Authentication:** Supabase Auth or an equivalent suitable service.
- **AI:** A large language model with retrieval grounded in stored records and approved sources.
- **Search:** Structured database queries and full-text search.
- **Source storage:** Metadata and references to approved sources.
- **Hosting:** To be selected after evaluating cost, security, and deployment requirements.

This is a preliminary direction, not a final architecture decision. The implementation design will be documented separately.

## 14. Commercial Model

The intended business model is subscription-based B2B SaaS.

Potential plans to validate:

- Individual professional subscription.
- Team subscription.
- Enterprise subscription.

Pricing, usage limits, and included data coverage will be tested with prospective customers.

The initial commercial validation goal is to secure paid pilot customers and establish whether they have a recurring need.

## 15. Success Metrics

Initial validation metrics include:

- Number of customer interviews completed.
- Number of qualified prospects agreeing to product demonstrations.
- Number of paid pilots secured.
- Percentage of research claims with usable supporting sources.
- Time required to produce a briefing.
- Customer-reported time saved.
- Repeat usage during the pilot.
- Conversion from paid pilot to recurring subscription.
- Customer retention once subscriptions begin.

Numeric targets will be established after initial customer discovery.

## 16. MVP Acceptance Criteria

The MVP will be ready for controlled customer testing when:

1. A user can search for a supported person.
2. The platform can distinguish supported matches where names are ambiguous.
3. A profile displays available professional information with sources.
4. Supported company affiliations and investment disclosures can be reviewed.
5. The user can generate a research brief.
6. Important factual statements in generated answers link to supporting evidence.
7. The system communicates missing or conflicting evidence.
8. Users can save profiles if that feature is included in the pilot.
9. Authentication and access controls work as intended.
10. Testing identifies no unresolved critical security or data-integrity issues.

## 17. Development Roadmap

### Phase 1: Discovery

- Conduct customer interviews.
- Evaluate competing products.
- Select the initial customer segment.
- Validate the willingness to pay.

### Phase 2: Product Design

- Finalise MVP requirements.
- Create wireframes.
- Design the data model.
- Establish data sourcing and verification rules.

### Phase 3: MVP Development

- Implement authentication and search.
- Build professional profiles.
- Add source attribution.
- Implement AI-assisted research and briefing generation.

### Phase 4: Pilot Testing

- Test with selected business customers.
- Measure accuracy and usefulness.
- Fix major product gaps.
- Evaluate subscription conversion.

### Phase 5: Iteration

- Prioritise improvements based on customer usage.
- Expand data coverage where justified.
- Consider saved searches, alerts, and team features.

## 18. Open Questions

The following decisions remain open:

1. Which initial customer segment has the strongest validated need?
2. Which public and commercial data sources can be used reliably and lawfully?
3. What profile coverage is required for the first paid pilot?
4. What level of human review is necessary?
5. Which AI model and retrieval approach provide sufficient accuracy?
6. What pricing and usage limits will customers accept?
7. Which features are essential for conversion to a recurring subscription?

These questions should be resolved through research and testing rather than assumptions.

## 19. Document History

| Version | Date | Change |
|---|---|---|
| 0.1 | 29 October 2026 | Initial PRD draft |

---

**End of document**
