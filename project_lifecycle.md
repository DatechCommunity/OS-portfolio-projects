# Project Lifecycle

This document explains the complete lifecycle of OS-Portfolio-Projects collaborative data engineering projects.

---

## States Overview

```
PROPOSED → APPROVED → SETUP → RECRUITING → ACTIVE → PHASE_2 → COMPLETE → MAINTAINED ⇄ ARCHIVED
```

Each state has specific entry criteria, actions, and exit conditions.

---

## 1️⃣ PROPOSED

**Definition:** A project idea has been submitted but not yet reviewed.

### Entry Criteria
- Community member submits [Project Proposal](.github/ISSUE_TEMPLATE/project_proposal.md)
- Proposal includes all required sections

### What Happens
- Proposal receives `project-proposal` label
- Maintainers review within 3 business days
- Discussion in comments to refine idea
- May request clarifications or changes

### Exit Conditions

**To APPROVED:**
- Maintainers vote to approve
- Proposal aligns with OS-Portfolio-Projects principles
- Project is feasible and valuable
- Phase 2 twist is meaningful

**To REJECTED:**
- Out of scope for the community
- Too similar to existing project
- Not feasible with available resources
- Proposer doesn't address feedback

### Duration
Typically 3-7 days

---

## 2️⃣ APPROVED

**Definition:** Maintainers approved the project, preparing for repo creation.

### Entry Criteria
- Maintainers approve proposal
- Project aligns with community goals
- Proposer confirms commitment

### What Happens
- Proposal receives `approved` label
- Maintainers prepare to create repository
- Decide on project lead (usually proposer if willing)
- Plan repository structure

### Actions by Maintainers
1. Create new repository in os-portfolio-projects org
2. Apply project repository template
3. Customize README, ROADMAP, docs
4. Set up GitHub labels and settings
5. Add project lead as collaborator
6. Update main repo PROJECTS.md

### Exit Conditions
- Repository created and configured
- Project lead assigned
- Moves to SETUP

### Duration
1-3 days

---

## 3️⃣ SETUP

**Definition:** Repository exists, being prepared for contributors.

### Entry Criteria
- Repository created in os-portfolio-projects org
- Project lead assigned and confirmed

### What Happens

**Project Lead:**
- Familiarizes with repository
- Reviews and refines documentation
- Creates initial project board
- Plans contributor onboarding
- May start foundational work

**Maintainers:**
- Support lead with questions
- Review initial documentation
- Help structure roadmap

### Required Setup Tasks
- [ ] README.md customized
- [ ] ROADMAP.md filled with phases
- [ ] docs/BUSINESS_CONTEXT.md complete
- [ ] docs/PHASE2_TWIST.md documented
- [ ] CONTRIBUTING.md project-specific additions
- [ ] Initial issues created
- [ ] Discord channel created (optional)

### Exit Conditions
- Setup checklist complete
- Lead ready to recruit contributors
- Moves to RECRUITING

### Duration
3-7 days

---

## 4️⃣ RECRUITING

**Definition:** Project actively seeking contributors.

### Entry Criteria
- Setup complete
- Project lead ready to onboard contributors
- Documentation sufficient for newcomers

### What Happens

**Visibility:**
- Project listed in PROJECTS.md as "Seeking Contributors"
- Announcement in Discord
- May be featured in newsletter (if applicable)
- README indicates "Accepting Applications"

**Application Process:**
1. Contributors find project in catalog
2. Read documentation
3. Submit [Join Project](.github/ISSUE_TEMPLATE/join_project.md) application
4. Project lead reviews application
5. Lead approves or provides feedback
6. Approved contributors added as collaborators
7. Onboarding issue created

**Project Lead Activities:**
- Review join applications
- Interview candidates (optional)
- Accept contributors
- Assign onboarding tasks
- Coordinate team

### Exit Conditions

**To ACTIVE:**
- Minimum team assembled (lead decides, no hard minimum)
- Core roles filled
- Team ready to start building

**To DORMANT (rare):**
- No applications after 4 weeks
- Proposer can't commit time
- Project paused until interest emerges

### Duration
Varies: 1-4 weeks typically

---

## 5️⃣ ACTIVE

**Definition:** Team is actively building Phase 1 of the project.

### Entry Criteria
- Team assembled (at least lead, ideally 2-3+ people)
- Contributors onboarded
- Initial tasks assigned

### What Happens

**Development:**
- Regular commits and PRs
- Team meetings (optional, async-first)
- Issues created and resolved
- Code reviews
- Documentation updates

**Project Lead:**
- Coordinates work
- Reviews PRs
- Resolves blockers
- Updates ROADMAP.md
- Manages team communication

**Contributors:**
- Work on assigned tasks
- Submit PRs
- Review others' work
- Ask questions, collaborate

**Milestones:**
- Track progress in ROADMAP.md
- Celebrate completed features
- Adjust timeline as needed

### Health Indicators

**Healthy:**
- Regular commits (weekly)
- Active discussions
- PRs reviewed promptly
- Roadmap updated

**At Risk:**
- No commits for 2+ weeks
- Blockers unresolved
- Contributors dropping out
- Lead unresponsive

**Intervention:**
- Maintainers check in
- Offer support
- May reassign lead if necessary

### Exit Conditions

**To PHASE_2:**
- Phase 1 milestones complete
- Core functionality working
- Ready for twist implementation

**To DORMANT:**
- Team disbanded
- No activity for 3+ months
- Lead stepped down, no replacement

### Duration
Varies: 1-4 months typically

---

## 6️⃣ PHASE_2

**Definition:** Implementing the twist - requirements evolution.

### Entry Criteria
- Phase 1 complete
- Core system working
- Team ready for twist

### What Happens

**The Twist Activates:**
- Requirements change (as documented in PHASE2_TWIST.md)
- Team adapts the system
- May require significant refactoring
- Simulates production reality

**Team Activities:**
- Analyze impact of changes
- Create ADRs for major decisions
- Refactor/rebuild affected components
- Test new requirements
- Update documentation

**New Challenges:**
- May need additional skills
- Can recruit specialized contributors
- Existing team learns to adapt
- Demonstrates production engineering

### Exit Conditions

**To COMPLETE:**
- Phase 2 requirements met
- Validators pass
- Cost within budget
- Documentation updated
- ADRs explain decisions

### Duration
Varies: 2-8 weeks typically

---

## 7️⃣ COMPLETE

**Definition:** Core project finished, but open for improvements.

### Entry Criteria
- Phase 1 and Phase 2 done
- All success criteria met
- Validators passing
- Documentation complete

### What Happens

**Project Status:**
- Listed in PROJECTS.md as "Complete"
- README updated with completion status
- CONTRIBUTORS.md finalized
- Celebration / announcement

**Still Open For:**
- Bug fixes
- Performance improvements
- Additional features
- Documentation enhancements
- New contributor onboarding

**Contributors:**
- Can continue improving
- Can leave and return
- Credited for all contributions
- Portfolio-ready to use

### Transition Paths

**To MAINTAINED:**
- Active improvements ongoing
- Regular commits continue
- Team or new contributors engaged

**To ARCHIVED:**
- Manual decision by maintainers
- Team moved on
- No activity for extended period
- Dependencies outdated

### Duration
Indefinite - can stay here forever

---

## 8️⃣ MAINTAINED

**Definition:** Project complete and actively maintained/improved.

### Entry Criteria
- Project COMPLETE
- Ongoing improvements happening
- Contributors still engaged

### What Happens
- Regular updates and improvements
- Version releases
- Dependency updates
- New features added
- Community contributions

### Activities
- Accepting PRs
- Reviewing improvements
- Coordinating enhancements
- Supporting users

### Exit Conditions

**To ARCHIVED:**
- Manual decision by maintainers
- Team consensus to archive
- Significant time with no activity
- Technology outdated

### Duration
Varies: months to years

---

## 9️⃣ ARCHIVED

**Definition:** Project no longer active but preserved for learning.

### Entry Criteria
- Manual decision by maintainers
- OR 6+ months of inactivity
- OR project lead requests archival

### What Happens

**GitHub:**
- Repository archived (read-only)
- Listed in PROJECTS.md "Archived" section
- README updated with archived status
- Link to active fork (if exists)

**Still Available:**
- Code remains public
- Contributors still credited
- Can be forked
- Can be revived

### Can Be Revived

**To MAINTAINED:**
- Someone proposes revival
- Maintainers approve
- New lead assigned
- Dependencies updated
- Moved back to MAINTAINED

**Revival Process:**
1. Open issue proposing revival
2. Explain why and what you'll improve
3. Maintainers review
4. If approved, assign new lead
5. Unarchive repository
6. Update documentation
7. Resume development

### Duration
Indefinite

---

## Special Cases

### DORMANT (Not an Official State)

**What it means:**
- Project approved but stalled
- No team or team disbanded
- Not active but not archived

**Happens when:**
- RECRUITING failed (no applicants)
- ACTIVE team disbanded
- Lead stepped down

**Resolution:**
- Stays dormant until interest emerges
- Can be revived by new lead
- OR eventually archived

---

## State Tracking

### Where States Are Documented

**Main Repository (os-portfolio-projects):**
- PROJECTS.md - Lists all projects with current state

**Project Repository:**
- README.md - Status badge indicates state
- ROADMAP.md - Current phase documented

**GitHub:**
- Labels on project repository
- Project board stages
- Issues and milestones

### State Change Notifications

**Who Gets Notified:**
- Project contributors
- Discord announcements
- PROJECTS.md updates
- Repository watchers

---

## Metrics & Reporting

### Project Health Metrics

**Active Projects:**
- Commits per week
- Open vs closed issues
- PR merge rate
- Contributor activity

**Complete Projects:**
- Total contributors
- Timeline (start to finish)
- LOC, features delivered
- Learning impact

**Portfolio Value:**
- Skills demonstrated
- Complexity level
- Production-readiness
- Community impact

---

## FAQ

### How long should a project stay in RECRUITING?
2-4 weeks typically. If no applicants, may go DORMANT.

### Can a project skip RECRUITING?
Yes, if proposer has a team ready.

### What if Phase 1 takes too long?
That's OK. Roadmaps are estimates. Adjust timeline as needed.

### Can we go back to RECRUITING during ACTIVE?
Yes, if team needs more people for Phase 2 or specialists.

### Who decides when to ARCHIVE?
Maintainers, with input from project lead/team.

### Can ARCHIVED projects be used?
Absolutely! Fork it, learn from it, reference it in your portfolio.

### What if the lead quits during ACTIVE?
Maintainers find new lead from team, or project goes DORMANT.

---

This lifecycle ensures projects stay organized, contributors know what to expect, and the community benefits from transparency.

**Questions?** Ask in [Discord #projects](https://discord.gg/yourlink)
