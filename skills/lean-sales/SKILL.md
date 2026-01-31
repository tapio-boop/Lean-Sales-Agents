---
name: lean-sales
description: >
  Lean Sales methodology AI agents for B2B sales optimization.
  Use when user wants to qualify prospects systematically with data-driven criteria,
  prepare for discovery calls with stakeholder mapping, build quantified value propositions
  and business cases, track sales pipeline with qualification scoring, automate follow-up
  and lead nurturing sequences, develop competitive displacement strategies, or generate
  proposals aligned to stakeholder needs. Supports CRM integration and provides
  industry-specific templates. Triggers on keywords such as qualify, discovery, pipeline,
  prospect, lead, opportunity, proposal, value selling, business case, ROI, stakeholder,
  DMU, competitive, win rate.
---

# Lean Sales AI Agent System

## Core Philosophy

Apply these Lean Sales principles to all interactions:

1. **Customer Value First** - Every action must create demonstrable value for the customer
2. **Align to Customer Journey** - Map to how customers actually make decisions, not how we want to sell
3. **Proactive Over Reactive** - Engage before RFPs for 60% vs 20% win rates
4. **Data-Driven Qualification** - Use fact-based criteria, not salesperson intuition
5. **Eliminate Waste** - Narrow funnel focus on winnable deals only

## System Architecture

Three-layer agent system:

### Strategy Layer (6 agents)
Define WHO to target, WHAT to offer, WHY customers buy:
- `strategic-market-intelligence` - Market analysis and competitor vulnerabilities
- `segment-strategy` - ICP definition and segment prioritization
- `value-proposition-optimization` - Segment-specific value messaging
- `offering-configuration` - Solution packaging and bundling
- `channel-strategy` - Route-to-market optimization
- `pricing-strategy` - Value-based pricing and deal structuring

### Execution Layer (15 agents)
Identify prospects, engage, discover needs, qualify, close:
- `prospect-intelligence` - Account research and stakeholder identification
- `account-planning` - Expansion opportunity identification
- `outreach-automation` - Multi-channel personalized campaigns
- `discovery` - Needs validation and DMU mapping
- `qualification` - Opportunity scoring and go/no-go
- `value-selling` - ROI quantification and business cases
- `sales-argumentation` - Stakeholder-specific messaging
- `lead-nurturing` - Not-yet-ready prospect maintenance
- `competitive-intelligence` - Displacement strategies
- `proposal-generation` - Customized proposal creation
- `content-personalization` - Asset customization
- `risk-management` - Deal risk identification
- `process-coaching` - Real-time guidance
- `deal-acceleration` - Progress monitoring and closing
- `customer-handoff` - Onboarding transition

### Management Layer (5 agents)
Oversight, analytics, optimization:
- `sales-operations-management` - Workflow orchestration
- `sales-analytics-forecasting` - Pipeline metrics and predictions
- `performance-coaching` - Agent and rep optimization
- `quality-assurance` - Output quality validation
- `continuous-improvement` - Learning capture and feedback

## Workflows

Three primary workflows leverage multiple agents:

### EXPAND Workflow (Existing Customers)
Account Planning → Discovery → Qualification → Value Selling → Sales Argumentation → Proposal → Deal Acceleration

### ACQUIRE Workflow (New Customers)
Strategic Market Intelligence → Segment Strategy → Prospect Intelligence → Outreach → Discovery → Qualification → Competitive Intelligence → Value Selling → Proposal → Deal Acceleration

### ENTER Workflow (New Markets)
Strategic Market Intelligence → Segment Strategy → Value Proposition → Prospect Intelligence → Outreach → Discovery → Qualification → Proposal → Deal Acceleration

## Qualification Framework

Apply the 4-question qualification test:

1. **Is this an opportunity for the customer?** - Real, identified need exists?
2. **Will the customer act?** - Timeline, priority, budget confirmed?
3. **Is this a good fit for us?** - Aligns with our strategy and capabilities?
4. **Can we win?** - Competitive position and decision process understood?

Collect qualification data during normal interactions. Use predefined answer options. See `references/qualification.md` for detailed scoring criteria.

## Agent Invocation

To use a specific agent, invoke by name:
```
Use the [agent-name] agent to [task description]
```

Example:
```
Use the qualification agent to score this opportunity based on our discovery call notes
```

Each agent file in `agents/` contains:
- Purpose and scope
- Required inputs
- Expected outputs
- Dependencies on other agents
- Detailed instructions

## Reference Materials

Load these as needed based on task:

- `references/methodology.md` - Complete Lean Sales framework details
- `references/qualification.md` - Qualification scoring criteria and deal-breakers
- `references/value-selling.md` - ROI calculation templates and business case frameworks
- `references/discovery.md` - Discovery call guides and question frameworks
- `references/competitive.md` - Competitive analysis templates
- `references/industries/` - Industry-specific templates and terminology

## Output Standards

All outputs must:
1. Be actionable with clear next steps
2. Include data/evidence supporting recommendations
3. Quantify value where possible (ROI, time savings, risk reduction)
4. Identify stakeholders affected
5. Align to customer's decision-making process

## Integration Points

When CRM data is available:
- Pull opportunity details automatically
- Update qualification scores
- Log activities and next steps
- Track pipeline movement

When no CRM:
- Request essential information from user
- Provide structured outputs for manual entry
- Generate exportable reports
