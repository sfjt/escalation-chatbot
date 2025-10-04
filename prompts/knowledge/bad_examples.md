# Bad Escalation Examples

## Overview

If you see the following patterns in the support engineer's input, guide the support engineer to take additional actions so they can provide sufficient information with which you can write an effective escalation.

- The draft of the escalation or problem description only has a problem statement (symptom) without much detail, analysis, or logs. This indicates that the support engineer gives up investigating the issue themselves and simply "rethrows" what the customer explained to the development/engineering team.
- The draft of the escalation doesn't have a clear ask, action item, or definition of done for the development/engineering team.
- The support engineer declares a high priority, but the business justification or reason for the priority is unclear or unexplained.

## Bad Example 1

**Title:** 503 Service Unavailable

**Priority:** P1 (URGENT)

**Description:**

The customer is seeing 503 Service Unavailable responses and wants to know the cause.

**Why this is bad and how to guide the support engineer:**

The description lacks details, such as:

- It seems that some API endpoints returned the status code 503. The name or path of the API endpoints should be included.
- The description must include what the support engineer investigated before creating the escalation. For example, the support engineer should review and analyze the access logs, check if the same problem can be observed in their testing environment, and ask the customer for the timestamp when they started to see the problem.

Also, the business justification for the priority "P1 (URGENT)" needs to be explained. For example, "The customer observed 80k errors out of 100k requests, which was 80% of the total requests against the endpoint 'POST /api/contracts'. The issue is ongoing and has significant impact on the core business operation." If the customer or the support engineer cannot explain the business justification, the priority should be adjusted to "P2 (HIGH)" or "P3 (NORMAL)."

## Bad Example 2
**Title:** GET /api/contracts - "active" query parameter ignored

**Priority:** P3 (NORMAL)

**Description:**

Per our official documentation, the endpoint "GET /api/contracts" accepts the query parameter "active" (true/false) with which users can search for active or inactive contracts.
However, when the customer made a GET request with this parameter, the endpoint simply returned all existing contracts without filtering them.

**Why this is bad and how to guide the support engineer:**

- A defect must be tested and reproduced by the support engineer, and they must report the outcome of the test. If the problem cannot be reproduced even if the support engineer tries different conditions, they must explain what they tried so far.
- The description lacks action items or the definition of done for the development/engineering team. The support engineer should explain what they expect from the team. For example, "Could you file it in the backlog and let me know the URL?" and/or "Could you work on the fix right away and let me know the ETA for the fix? This is one of the largest customers in this region and the defect blocks them from implementing a core use case."

## Bad Example 3

**Title:** Need example code for new feature implementation

**Priority:** P2 (HIGH)

**Description:**

We are attempting to implement a new feature that allows our end users to purchase cosmetic items for their avatars using a Buy Now, Pay Later (BNPL) service.

We are integrating this purchase flow with the [Product Name] API and are receiving a 400 Bad Request error.

We have tried several different approaches, but we need an example of how to correctly format the request to handle this specific use case. Our deadline is next week, so we need a quick turnaround on this issue.

**Why this is bad and how to guide the support engineer:**

- The priority is P2, but the justification is a customer's internal development timeline ("We have a tight deadline" and "We need a quick turnaround"). This is not a sufficient reason for a high priority. P2 is reserved for issues with a significant business impact, such as a production outage or a proven defect that blocks a customer's core business operations.
- The description starts with the personal pronoun "We," which indicates that the support engineer simply copied and pasted the customer's request instead of translating it into their own words. A support engineer should internalize the problem and summarize it clearly. This also suggests the engineer hasn't performed the required investigation steps.
- The core request is for example code and implementation guidance, particularly for a complex use case involving a third-party BNPL service. Providing step-by-step instructions or custom code for such scenarios is typically the responsibility of a solutions architect or a professional services team, not the support or development teams. The support engineer should manage the customer's expectations by explaining what the support team can and cannot do. They should first verify if the 400 Bad Request is an actual bug and not just a malformed request on the customer's end.
