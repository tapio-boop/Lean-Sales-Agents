---
name: follow-up
description: Generate follow-up actions, emails, and nurturing sequences
usage: /lean-sales:follow-up [type] [context]
---

# Follow-Up Command

Generate appropriate follow-up actions based on sales stage and interaction type.

## Follow-Up Types

### Post-Meeting Follow-Up (`/lean-sales:follow-up meeting`)

1. **Input Meeting Context**
   - Meeting type (discovery, demo, negotiation, etc.)
   - Key attendees and their roles
   - Main discussion points
   - Commitments made
   - Next steps agreed

2. **Generate Follow-Up Package**

   #### Thank You Email
   - Personalized acknowledgment
   - Key points recap (their words, not ours)
   - Value reinforcement tied to their priorities
   - Clear next steps with dates

   #### Internal Action Items
   - Tasks with owners and deadlines
   - Materials to prepare
   - Stakeholders to brief
   - CRM updates needed

   #### Customer-Facing Materials
   - Summary document recommendations
   - Case studies to share
   - ROI materials to prepare

### Lead Nurturing Sequence (`/lean-sales:follow-up nurture`)

1. **Assess Lead Context**
   - Current qualification status
   - Engagement history
   - Identified interests/pain points
   - Reason for nurture (not ready, timing, etc.)

2. **Generate Nurture Sequence**

   #### 90-Day Nurture Plan
   | Day | Action | Content/Message | Goal |
   |-----|--------|-----------------|------|
   | 1 | Email | Thank you + value resource | Maintain connection |
   | 7 | Content | Industry insight article | Establish expertise |
   | 21 | Email | Case study relevant to needs | Build credibility |
   | 35 | Invite | Webinar/event invitation | Re-engage |
   | 50 | Content | Research/benchmark report | Provide value |
   | 65 | Email | Check-in on initiatives | Gauge readiness |
   | 80 | Content | New capability announcement | Create urgency |
   | 90 | Call | Re-qualification attempt | Convert or extend |

   #### Trigger-Based Actions
   - Email engagement signals
   - Website visit indicators
   - Content download triggers
   - Social engagement opportunities

### Proposal Follow-Up (`/lean-sales:follow-up proposal`)

1. **Input Proposal Context**
   - Proposal sent date
   - Key stakeholders
   - Main value propositions
   - Known concerns/objections
   - Decision timeline

2. **Generate Follow-Up Strategy**

   #### Immediate Actions (24-48 hours)
   - Confirmation of receipt
   - Offer to walk through
   - Stakeholder-specific summaries

   #### Week 1 Strategy
   - Check-in cadence
   - Value reinforcement touchpoints
   - Competitive defense preparation

   #### Stall Recovery Tactics
   - Re-engagement approaches
   - New value angles
   - Executive sponsor engagement
   - Timeline compression techniques

### Win-Back Campaign (`/lean-sales:follow-up winback`)

1. **Input Lost Opportunity Context**
   - Original opportunity details
   - Reason for loss
   - Competitive outcome
   - Relationship status
   - Time since loss

2. **Generate Win-Back Plan**

   #### Re-Engagement Strategy
   - Timing recommendations
   - Approach angle
   - New value propositions
   - Relationship rebuilding steps

## Output Format

All follow-ups include:
- Ready-to-send email drafts
- Calendar/task items with dates
- CRM update recommendations
- Success metrics to track

## Dependencies

- Uses: `lead-nurturing` agent, `outreach-automation` agent
- References: `references/discovery.md` for context
- May trigger: `content-personalization` for materials

## Examples

User: `/lean-sales:follow-up meeting` - Creates post-meeting follow-up
User: `/lean-sales:follow-up nurture` - Generates nurturing sequence
User: `/lean-sales:follow-up proposal Acme Corp` - Creates proposal follow-up plan
