---
name: Project Proposal
about: Propose a new collaborative data engineering project
title: "[Project Proposal]: "
labels: project-proposal
assignees: ''
---

# Project Proposal

**This proposal is for a collaborative project that will be built by multiple contributors.**

If approved, maintainers will:
1. Create a separate repository for this project
2. Assign a project lead
3. Open it for contributor applications

---

## 🏢 Business Context

**What company or system does this simulate?**

Describe the business scenario in 2-3 paragraphs. Make it feel real.

💡 **Good example:** "A mid-sized fintech company processing 500K daily mobile payments across East Africa. The fraud detection system currently has a 30% false positive rate, overwhelming customer support. Reports arrive 6 hours late, and cloud costs have tripled in 6 months."

**Your answer:**

[Describe the business context]

---

## 🎯 Problem Statement

**What is broken, slow, expensive, or unreliable?**

**The Setup:**
[What's currently failing?]

**Business Impact:**
[Who gets hurt? What breaks? What costs money?]

**Technical Constraints:**
[What makes this hard? Legacy systems? Scale? Budget? SLAs?]

💡 **Example:**
```
Setup: Fraud detection pipeline processes 500K events daily but takes 6 hours
Impact: $2M monthly fraud losses, customer support overwhelmed
Constraints: Must work with existing MySQL, <$500/month budget, can't change source systems
```

---

## 🔁 Production Reality Twist (Phase 2)

**This is mandatory - what changes midway through the project?**

### Initial State (Phase 1)
[What does the team build first?]

### Twist Event (Phase 2)
[What breaks or changes? Be specific.]

### Why This Matters
[What production truth does this simulate?]

💡 **Strong examples:**
- "Regulator mandates real-time transaction monitoring. Your batch system must become streaming within 30 days."
- "Black Friday traffic 10x overnight. Your 2-hour pipeline must handle same data in 15 minutes."
- "New payment provider with different schema and failure modes. Must integrate without breaking existing flows."

**Your twist:**

[Be specific about what changes and why]

---

## 🧩 Project Deliverable

**What will the team build?**

Describe the final data product in 2-3 paragraphs.

💡 **Example:** "A real-time fraud detection platform processing payment events from Kafka, scoring transactions with ML models, and alerting on suspicious patterns within 100ms. Includes monitoring dashboard, cost optimization, and Phase 2 compliance reporting."

**Your answer:**

[What's the end result?]

---

## 🗂️ Data Sources

**What systems produce the data?**

For each source, provide:

### Source 1: [Name]
**Type:** [Postgres / Kafka / REST API / Logs / Other]  
**Schema/Structure:** [Brief description of key fields]  
**Volume:** [Rough estimate: "100K records/day" or "50GB/day"]  
**Failure Modes:**
- [ ] Late-arriving data
- [ ] Duplicates
- [ ] Schema changes
- [ ] Missing/null fields
- [ ] Data corruption
- [ ] Other: [specify]

### Source 2: [Name] (if applicable)
[Same structure]

---

## 🛠️ Core Skills (Pick 3-5 max)

**What will contributors learn by working on this?**

❌ Don't check everything. Pick the 3-5 most important skills.

**Pick your top 3-5:**
- [ ] SQL & Query Optimization
- [ ] Python/Pandas Data Processing
- [ ] ETL Pipeline Design
- [ ] Real-time Stream Processing (Kafka, Flink)
- [ ] Change Data Capture (CDC)
- [ ] Cost Optimization (FinOps)
- [ ] Data Modeling (Star schema, normalization)
- [ ] Data Quality & Validation
- [ ] Docker & Containerization
- [ ] Kubernetes/Orchestration
- [ ] Monitoring & Observability
- [ ] Performance Tuning
- [ ] Architecture Decision Making
- [ ] Other: [specify]

---

## 🎚️ Difficulty & Scale

### Difficulty Level
- [ ] **Beginner** - Foundational skills, 1-2 months timeline
- [ ] **Intermediate** - Production complexity, 2-4 months timeline
- [ ] **Advanced** - Platform/distributed systems, 4-6 months timeline

### Data Scale
- [ ] **Small** - Laptop-scale (<10GB, can run locally)
- [ ] **Medium** - Cloud-friendly (10GB-1TB, modest resources)
- [ ] **Large** - Enterprise-scale (>1TB, optimization critical)

### Infrastructure Requirements
- [ ] **Runs fully on laptop** (8GB RAM)
- [ ] **Needs modest cloud resources** (~$50-200/month)
- [ ] **Needs significant cloud setup** (>$200/month)

---

## 💸 FinOps Constraint

**What's the cost pressure or trade-off?**

**Budget Tier:**
- [ ] Minimal (laptop-only, <$50/month)
- [ ] Low ($50-200/month)
- [ ] Medium ($200-1000/month)
- [ ] High (>$1000/month)

**Primary Trade-off:**
[What cost decision must be made?]

💡 **Examples:**
- "Balance S3 Standard vs Glacier for 5TB historical data"
- "Choose between Lambda (expensive, simple) vs EC2 (cheaper, complex ops)"
- "Optimize Kafka retention vs query performance"

**Your answer:**

[What's the cost challenge?]

---

## 🧑‍🤝‍🧑 Team Composition

### Estimated Team Size
**How many contributors would be ideal?**
- [ ] 2-3 people
- [ ] 4-6 people
- [ ] 7-10 people
- [ ] 10+ people

### Roles Needed

**What skills/roles are needed on the team?**

💡 **Example:**
- Data Engineers (2) - Build pipelines
- Platform Engineer (1) - Infrastructure & deployment
- ML Engineer (1) - If ML components
- Analytics Engineer (1) - Metrics & dashboards
- DevOps (1) - CI/CD & monitoring
- Technical Writer (1) - Documentation

**Your team composition:**

[List roles and rough numbers]

---

## 📊 Success Criteria

### Functional Requirements
**What must the system do?**
- [ ] [Requirement 1]
- [ ] [Requirement 2]
- [ ] [Requirement 3]
- [ ] Phase 2 twist implemented
- [ ] Documented with ADRs

### Performance Targets (Rough)

**Latency tier:**
- [ ] Real-time (<1 second)
- [ ] Near real-time (<1 minute)
- [ ] Micro-batch (<15 minutes)
- [ ] Batch (<1 hour)
- [ ] Daily batch (24 hours)

**Throughput tier:**
- [ ] Low (hundreds/sec)
- [ ] Medium (thousands/sec)
- [ ] High (tens of thousands/sec)

### Quality Standards
- [ ] Automated validation passes
- [ ] Cost stays within budget
- [ ] Monitoring/observability present
- [ ] Documentation complete
- [ ] ADRs document key decisions

---

## 🏗️ Architecture Approaches

**Describe at least 2 valid approaches to building this.**

This helps contributors understand there are multiple valid solutions.

### Approach A: [Name]
**Tech Stack:** [e.g., "Airflow + Spark + S3"]  
**Philosophy:** [e.g., "Batch-oriented, cost-optimized"]  
**Trade-offs:** [e.g., "Cheaper but higher latency, simpler operations"]

### Approach B: [Name]
**Tech Stack:** [e.g., "Kafka + Flink + Postgres"]  
**Philosophy:** [e.g., "Real-time streaming"]  
**Trade-offs:** [e.g., "Lower latency but higher cost, complex operations"]

### Approach C: [Name] (Optional)
[If there's a third interesting direction]

---

## 🗺️ Project Roadmap (High-Level)

**What are the major phases?**

### Phase 1: Foundation (Weeks 1-X)
**Goal:** [e.g., "Core data ingestion and basic transformations"]  
**Deliverables:**
- [ ] [Deliverable 1]
- [ ] [Deliverable 2]

### Phase 2: The Twist (Weeks X-Y)
**Goal:** [e.g., "Implement real-time requirements"]  
**Deliverables:**
- [ ] [Deliverable 1]
- [ ] [Deliverable 2]

### Phase 3: Optimization (Weeks Y-Z)
**Goal:** [e.g., "Cost optimization and observability"]  
**Deliverables:**
- [ ] [Deliverable 1]
- [ ] [Deliverable 2]

**Estimated total timeline:** [X months]

---

## 🎯 Your Role

### Can You Lead This Project?

**If approved, are you willing to be project lead?**
- [ ] **Yes** - I'll lead the project
- [ ] **Maybe** - Depends on team/support
- [ ] **No** - I'm proposing but can't lead
- [ ] **I'll contribute** - I can be a team member but not lead

**If yes to leading, what experience do you have?**
[Relevant experience with similar systems, team leadership, etc.]

### Your Contribution

**What parts can you personally contribute to?**
- [ ] Data pipeline development
- [ ] Infrastructure/DevOps
- [ ] Documentation
- [ ] Code review
- [ ] Architecture design
- [ ] Testing/validation
- [ ] Project management
- [ ] Other: [specify]

**Time commitment:**
- [ ] 5-10 hours/week
- [ ] 10-20 hours/week
- [ ] 20+ hours/week

---

## 📝 Additional Context

### Inspired By Real Experience?
[Share the story if you want - makes the project authentic]

### Similar Projects?
[Any existing open-source projects this relates to?]

### Technologies You Envision?
[Specific tools/frameworks in mind?]

### Potential Challenges?
[What will trip the team up? Schema evolution? Race conditions? Cost spikes?]

### Learning Resources?
[Any docs/tutorials that would help contributors?]

---

## ✅ Pre-Submission Checklist

Before submitting, ensure:

- [ ] Business context is clear and realistic
- [ ] Problem statement explains the pain
- [ ] Phase 2 twist is specific and meaningful
- [ ] Core skills limited to 3-5 most important
- [ ] Team composition estimated
- [ ] 2+ architecture approaches described
- [ ] High-level roadmap provided
- [ ] Indicated if you can lead or contribute
- [ ] Ready to commit time if approved

---

## 🚀 What Happens Next

### If Approved:
1. **Maintainers create** a new repository in the OS-Portfolio-Projects org
2. **Maintainers assign** project lead (likely you if you volunteered)
3. **Repository is set up** with standard structure and documentation
4. **Project opens** for contributor applications
5. **You coordinate** with contributors to build it

### If Needs Refinement:
1. Maintainers will ask clarifying questions
2. You can update the proposal
3. Resubmit for review

### Timeline:
- **Initial review:** Within 3 business days
- **Decision:** Within 1 week
- **Repo setup:** Within 1 week of approval

---

**Thank you for proposing a collaborative project!** 🎉

The community will benefit from your idea, and contributors will gain real portfolio-worthy experience building production-grade data systems.

**Questions?** Ask in [Discord #project-proposals](https://discord.gg/yourlink)
