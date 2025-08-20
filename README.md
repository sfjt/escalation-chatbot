# Escalation Chatbot Prompts

Escalation Chatbot Prompts
A comprehensive set of prompts and knowledge files designed to help technical support engineers write effective escalation tickets that get **faster resolution** from development and engineering teams.

## 🎯 Purpose

This chatbot system is a learning tool for support engineers to master the art of writing high-quality escalations. By using these prompts, you will learn to:

- **Follow best practices** for investigating and documenting issues, which leads to clearer tickets.
- **Communicate effectively** with engineering teams, ensuring your message is understood the first time.
- **Prevent common pitfalls**, like unclear priorities and the XY problem.
- **Ensure all necessary information is included**, which eliminates back-and-forth and leads to quicker response times and **faster case resolution**.

**Note:** The instructions are intentionally designed to be restrictive for educational purposes so the user can learn best practices through chatting.

## 📁 File Structure

### Core Files

| File | Purpose |
|------|---------|
| `instructions.txt` | Main workflow with investigation guidance and XY problem detection |
| `best_practices.txt` | Comprehensive escalation writing guidelines |
| `priorities.txt` | Priority definitions with clear decision framework |
| `good_examples.txt` | Effective escalation examples to model |
| `bad_examples.txt` | Learning examples with improvement guidance |

## 🚀 Key Features

### 1. **Investigation Checklist**
Structured approach to gather complete information before escalating:
- ✅ Document error messages and screenshots
- ✅ Attempt reproduction in test environment
- ✅ Review recent changes that might be related
- ✅ Search knowledge base for similar issues
- ✅ Gather comprehensive environment details
- ✅ Understand customer's business objective

### 2. **XY Problem Prevention**
Helps identify when customers describe attempted solutions rather than actual needs:
- **Recognition patterns**: Unclear business context or complex workarounds
- **Clarifying questions**: "What business goal are you trying to accomplish?"
- **Educational resource**: Links to https://xyproblem.info
- **Better outcomes**: Solve the real problem, not just the symptom

### 3. **Priority Decision Framework**
Clear criteria for consistent priority assignment:
1. **Complete service outage?** → P1
2. **Major user impact with no workaround?** → P1  
3. **Significant business impact?** → P2
4. **Standard issues** → P3

### 4. **Comprehensive Guidance**
Detailed best practices covering:
- Clear problem descriptions
- Business impact articulation
- Evidence collection
- Environmental context
- Customer impact assessment
- Investigation documentation

## 🛠️ Usage

### For Support Teams
1. Deploy these prompts to your AI chatbot system (Gemini, Claude, ChatGPT, etc.)
2. Use as a training resource for escalation best practices
3. Reference during escalation reviews and coaching sessions
4. Customize examples for your specific product/service

### For Support Engineers
1. **Follow the investigation checklist** to gather complete information
2. **Ask about business objectives** to understand true customer needs
3. **Use the priority framework** for consistent priority assignment
4. **Model good examples** for structure and communication style
5. **Learn from examples** to continuously improve escalation quality

### For AI Implementation
Configure your AI system with:
- **Main prompt**: `instructions.txt`
- **Knowledge base**: All `.txt` files as reference material
- **Company context**: Update company name in instructions as needed

## 📊 Benefits

**For Support Engineers:**
- **Faster resolution times** through complete, well-structured escalations
- **Improved relationships** with engineering teams
- **Skill development** in technical communication
- **Confidence** in escalation decisions

**For Engineering Teams:**
- **Complete context** for faster problem diagnosis
- **Appropriate prioritization** aligned with business impact
- **Fewer back-and-forth clarifications**
- **Focus on real problems** rather than XY problem symptoms

**For Organizations:**
- **Reduced escalation cycle time**
- **Better customer outcomes**
- **Improved team collaboration**
- **Knowledge sharing** and skill development

## 🔄 Continuous Improvement

### Customization Ideas
- **Add product-specific examples** relevant to your service
- **Include common customer scenarios** your team encounters
- **Update priority criteria** based on your SLA structure
- **Incorporate team feedback** on what works best

### Evolution
This system grows with your team:
- **Document new patterns** you discover
- **Share successful escalation examples** 
- **Refine guidance** based on engineering feedback
- **Update for new tools** and processes

## 🤝 Getting Started

### Initial Setup
1. **Update company context** in `instructions.txt`: Replace `**Company name:** N/A` with your actual company or product name (e.g., `**Company name:** Acme Corporation`). This enables the AI to reference your official documentation when encountering unfamiliar product features.

### Using the System
2. **Review the examples** in `good_examples.txt` to understand effective escalation structure
3. **Practice with the checklist** on your next few escalations  
4. **Use the priority framework** to build confidence in priority decisions
5. **Share feedback** on what works well and what could be improved

---

**Designed to help support engineers create escalations that get results.**

*Building skills, improving outcomes, strengthening team collaboration.*