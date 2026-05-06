---
name: launch-product
description: SOP for managing the 90-day product launch sprint for DMPtech.ai and Easein. Tracks milestones, surfaces blockers, and coordinates cross-functional tasks.
---

# Launch Product

This skill manages the 90-day product launch sprint for both DMPtech.ai and Easein. It helps Wen stay focused, unblock dependencies, and ensure both products ship on time.

## Context
Both companies are targeting a product launch within 90 days. DMPtech.ai is a B2B SaaS platform; Easein is a B2C e-commerce product. They have different launch requirements but share the same founder's time and attention.

## Workflow

### Step 1: Weekly Status Check
When triggered, ask Wen for a quick status update on both companies:
1. What was completed this week?
2. What is blocked or at risk?
3. What is the single most important thing to unblock next?

### Step 2: Milestone Tracking
Maintain a running checklist of launch milestones for each company. Update this list based on Wen's status updates.

**DMPtech.ai Launch Milestones:**
- [ ] Finalize platform architecture (including zero-knowledge identity layer / NoPorts)
- [ ] Complete CNS Engine core build
- [ ] Onboard first pilot client (financial services / broker-dealer)
- [ ] Complete compliance and security review
- [ ] Prepare demo environment and sales materials

**Easein Launch Milestones:**
- [ ] Confirm production supplier and manufacturing timeline
- [ ] Finalize NFC tag integration and return logistics
- [ ] Complete Shopify store setup and payment processing
- [ ] Execute pre-order fulfillment plan
- [ ] Launch marketing campaign (Substack, LinkedIn, X, YouTube)

### Step 3: Prioritization
Cross-reference blockers with `context/priorities.md`. If a task is not directly tied to a launch milestone, deprioritize it and surface this to Wen.

### Step 4: Delegation Suggestions
When Wen describes a task, ask: "Can this be automated or delegated?" If yes, suggest creating a new skill or script. If no, add it to the action list.
