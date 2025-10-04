# Priorities

## Definitions

### P1 (Urgent/Critical)

An issue that makes the service completely unavailable, resulting in significant business impacts. It requires immediate attention and mitigation, and the support engineer needs to assemble the incident response team.

**Examples:**

- A server is down.
- A critical defect that makes the product unavailable in production for all or a major part of the users.
- A customer reports a critical vulnerability in the product and is able to show a PoC (proof of concept) or clear evidence of exploitation.

### P2 (High)

An issue that impacts major functionality of the product or a subset of users, making the service partially unavailable or results in significant degradation in performance.

**Examples:**

- Consistent and significant delays in API responses are observed and the problem is ongoing.
- A defect in the product impacted a specific high-value customer's use case. The customer's business is completely blocked due to the defect and there is no workaround.
- A customer reports a potential vulnerability in the product, but they don't show a PoC or clear evidence of exploitation.

### P3 (Normal)

This is the default priority.

**Examples:**

- A defect in the product that doesn't completely block the customer's business operations or one that has a workaround.
- A customer asked the support engineer to investigate a defect or past outage, but it is not ongoing.
- A problem found in a non-production environment.
- A customer asks how to implement a desired use case.

## Priority Decision Tree

### Step 1: Service Availability Check

**Question:** Is the service completely down or unavailable for ALL users?

- **YES** → P1 (Critical system outage)
- **NO** → Go to Step 2

### Step 2: Impact and Workaround Assessment  

**Question:** Are ≥50% of users affected AND no workaround exists?

- **YES** → P1 (Major impact, no mitigation)
- **NO** → Go to Step 3

### Step 3: Business Impact Evaluation
**Question:** Does this issue meet ANY of these criteria?

- Blocks high-value customer's critical business function
- Violates SLA commitments with financial penalties
- Affects revenue-generating functionality
- Security vulnerability with proof of concept
- **YES** → P2 (High business impact)
- **NO** → Go to Step 4

### Step 4: Default Assignment

**All other issues** → P3 (Normal priority)

### Special Cases:

- **When uncertain:** Default to P3 and explain your uncertainty
- **Customer demands P1:** Validate using this tree; explain if incorrect
- **Multiple criteria met:** Choose the highest priority that applies

**Priority Justification Template:**

"I recommend [Priority] because [specific criterion from decision tree]. This means [expected response time/team involvement]."
