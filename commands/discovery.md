---
name: discovery
description: Prepare for discovery calls and analyze discovery results
usage: /lean-sales:discovery [prepare|analyze] [context]
---

# Discovery Command

Prepare for discovery conversations or analyze discovery call results using Lean Sales methodology.

## Modes

### Prepare Mode (`/lean-sales:discovery prepare`)

1. **Gather Pre-Call Context**
   - Company/prospect information
   - Known stakeholders and roles
   - Industry and segment context
   - Existing relationship history
   - Competitive situation

2. **Generate Discovery Plan**

   Output includes:

   #### Call Objectives
   - Primary objective (what must be learned)
   - Secondary objectives (nice to have)
   - Relationship objectives (trust building)

   #### DMU Mapping Questions
   - Questions to identify decision makers
   - Questions to understand buying process
   - Questions to map influencers and blockers

   #### Needs Discovery Questions
   - Current state questions
   - Pain point exploration
   - Future state vision
   - Impact quantification

   #### Competitive Context Questions
   - Current solution landscape
   - Previous evaluation experiences
   - Vendor preferences and concerns

   #### Timeline & Budget Questions
   - Decision timeline drivers
   - Budget cycle alignment
   - Priority vs. other initiatives

3. **Provide Conversation Flow**
   - Opening framework (rapport building)
   - Transition phrases
   - Probing techniques
   - Closing and next steps structure

### Analyze Mode (`/lean-sales:discovery analyze`)

1. **Input Discovery Notes**
   - Accept call notes, transcript, or summary
   - Extract key information points

2. **Generate Analysis**

   Output includes:

   #### Needs Summary
   - Articulated needs (stated explicitly)
   - Latent needs (implied but not stated)
   - Underlying business drivers

   #### DMU Map
   | Role | Name | Influence | Support Level | Key Concerns |
   |------|------|-----------|---------------|--------------|

   #### Qualification Update
   - New information by qualification area
   - Updated qualification score
   - Deal-breaker assessment

   #### Competitive Insights
   - Competitors mentioned
   - Customer's perception of alternatives
   - Our positioning opportunities

   #### Value Themes Identified
   - Key value drivers for this customer
   - Quantifiable impact areas
   - Stakeholder-specific priorities

   #### Recommended Next Steps
   - Follow-up actions with owners
   - Information gaps to close
   - Stakeholders to engage next
   - Content/materials to send

## Dependencies

- Uses: `discovery` agent, `qualification` agent
- References: `references/discovery.md`, `references/qualification.md`
- May trigger: `value-selling` agent for business case development

## Examples

User: `/lean-sales:discovery prepare` - Prepares for upcoming discovery call
User: `/lean-sales:discovery analyze` - Analyzes notes from completed call
User: `/lean-sales:discovery prepare Acme Corp initial meeting` - Prepares with context
