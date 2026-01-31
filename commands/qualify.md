---
name: qualify
description: Qualify a prospect or opportunity using the Lean Sales qualification framework
usage: /lean-sales:qualify [opportunity name or description]
---

# Opportunity Qualification Command

Execute systematic qualification assessment using the Lean Sales 4-question framework.

## Process

1. **Gather Context**
   - Request opportunity details if not provided
   - Identify what qualification data is already known
   - Determine stage in sales process

2. **Apply Qualification Framework**

   Evaluate against four decision areas:

   ### FOR - Is this an opportunity for the customer?
   - Does a real, identified need exist?
   - Is the need acknowledged by key stakeholders?
   - What's the impact of not addressing this need?

   ### ACT - Will the customer take action?
   - Is there a defined timeline?
   - Is budget allocated or allocatable?
   - Is this a priority vs. other initiatives?
   - Who is driving the initiative internally?

   ### FIT - Is this a good fit for us?
   - Does it align with our ICP?
   - Can we deliver differentiated value?
   - Is the commercial model viable?
   - Does it fit our capacity and strategy?

   ### WIN - Can we win?
   - Do we understand the decision-making process?
   - Do we have access to key decision-makers?
   - What's our competitive position?
   - Are we first or last to the opportunity?

3. **Score and Recommend**
   - Assign scores (1-10) for each decision area
   - Calculate overall qualification score
   - Identify deal-breakers or red flags
   - Recommend: Pursue / Pursue with conditions / No-go

4. **Output Qualification Report**

   Format:
   ```
   ## Qualification Summary

   **Opportunity:** [Name]
   **Score:** [X/100]
   **Recommendation:** [Pursue/Conditional/No-go]

   ### Scores by Area
   - FOR (Customer Opportunity): X/25
   - ACT (Will Act): X/25
   - FIT (Strategic Fit): X/25
   - WIN (Win Probability): X/25

   ### Key Findings
   [Bullet points]

   ### Deal-Breakers Identified
   [List or "None"]

   ### Recommended Next Steps
   [Numbered action items]

   ### Information Gaps
   [Questions to answer before final decision]
   ```

## Dependencies

- Uses: `qualification` agent for scoring logic
- References: `references/qualification.md` for criteria details
- May trigger: `discovery` agent if information gaps identified

## Examples

User: `/lean-sales:qualify Acme Corp ERP modernization project`

User: `/lean-sales:qualify` (will prompt for opportunity details)
