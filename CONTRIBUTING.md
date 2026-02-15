# Contributing to Open Source Portfolio Projects

**Thank you for your interest in contributing!**

Open Source Portfolio Projects is built and maintained by data engineers who contribute their production experience to help others build strong portfolios. We welcome contributions at all experience levels—from fixing typos to designing complex challenges.

---

**Quick Links:** [Getting Started](#getting-started) · [Types of Contributions](#types-of-contributions) · [Submitting a Challenge](#submitting-a-challenge) · [Code of Conduct](CODE_OF_CONDUCT.md) · [Community](https://discord.gg/yourlink)

---

## Why Contribute?

### For the Community

Your contributions help data engineers worldwide:
- **Challenge designers** share production experience that others can learn from
- **Code reviewers** provide mentorship and catch issues before they reach users
- **Documentation writers** make the project more accessible to newcomers
- **Testers** ensure challenges work reliably across different environments

### For Your Portfolio

Contributing to OS-Portfolio-Projects demonstrates:
- **Technical depth** - Understanding of data engineering systems
- **Communication skills** - Clear documentation and code reviews
- **Collaboration** - Working with maintainers and community members
- **Leadership** - Helping guide the direction of an open-source project

Contributors are recognized in our [Hall of Fame](CONTRIBUTORS.md) and challenge authors are credited in each challenge they create.

---

## Getting Started

### Prerequisites

Before contributing, ensure you have:
- Git installed and configured
- Docker & Docker Compose (20.10+)
- Python 3.9+ for validators
- Familiarity with pull request workflow
- Read our [Code of Conduct](CODE_OF_CONDUCT.md)

### Your First Contribution

**New to open source?** Start with issues labeled [`good first issue`](https://github.com/DatechCommunity/os-portfolio-projects/labels/good%20first%20issue).

**Common first contributions:**
- Fix typos or improve documentation clarity
- Add test scenarios to existing validators
- Enhance data generator configurations
- Report bugs or suggest improvements
- Improve error messages in validators
- Add examples to documentation

**Steps:**
1. Fork the repository
2. Create a feature branch (`git checkout -b fix/typo-in-readme`)
3. Make your changes
4. Test locally (if applicable)
5. Commit with clear message (`git commit -m "Fix typo in beginner ETL challenge"`)
6. Push to your fork (`git push origin fix/typo-in-readme`)
7. Open a pull request

---

## Types of Contributions

We welcome many forms of contribution:

### Propose a Challenge

Design a new data engineering challenge based on production experience.

**Best for:** Senior engineers with 3+ years production experience

**Steps:**
1. Read the [Challenge Design Guide](docs/CHALLENGE-DESIGN-GUIDE.md)
2. Open an issue using [Challenge Proposal Template](.github/ISSUE_TEMPLATE/challenge-proposal.md)
3. Discuss design with maintainers (response within 3 business days)
4. Implement following [Submitting a Challenge](#submitting-a-challenge) guidelines
5. Submit pull request for review

**What we look for:**
- Based on real production scenarios
- Clear Phase 2 twist (requirements evolution)
- Includes FinOps constraints
- Automated validators for objective assessment
- Complete documentation

---

### Join a Project

Contribute to collaborative team-based projects.

**Best for:** All experience levels seeking team experience

**Steps:**
1. Browse active projects in [PROJECTS.md](PROJECTS.md)
2. Find a project matching your skills and interests
3. Read the project's business context and requirements
4. Submit application via project's "Join Project" template
5. Project lead reviews (3-5 days)
6. If approved, start contributing!

**Learn more:** [How to Join Projects](docs/JOINING-PROJECTS.md)

---

### Improve Infrastructure

Enhance tooling, automation, and project infrastructure.

**Best for:** Platform engineers, DevOps practitioners

**Areas needing help:**
- CI/CD pipeline improvements
- Docker optimization
- Validator framework enhancements
- Documentation tooling
- GitHub Actions automation
- Testing infrastructure

**Process:**
1. Check existing issues or create new one
2. Discuss approach with maintainers
3. Implement changes
4. Submit PR with tests

---

### Enhance Documentation

Improve guides, tutorials, and reference materials.

**Best for:** Technical writers, educators, experienced engineers

**Documentation needs:**
- Beginner-friendly setup guides
- Architecture decision record examples
- FinOps optimization strategies
- Troubleshooting guides
- Video walkthroughs
- Learning path recommendations

**Process:**
1. Identify gap or improvement opportunity
2. Write or update documentation
3. Submit PR with clear description

---

### Review & Mentor

Help review pull requests and mentor newcomers.

**Best for:** Experienced engineers with code review experience

**Responsibilities:**
- Review PRs for technical correctness
- Provide constructive feedback
- Help newcomers navigate contribution process
- Answer questions in Discord
- Test challenge solutions

**How to start:**
1. Join [Discord #contributors channel](https://discord.gg/yourlink)
2. Introduce yourself and areas of expertise
3. Maintainers will tag you on relevant PRs

---

### Report Bugs

Help identify and document issues.

**Best for:** Anyone using the challenges

**Good bug reports include:**
- Clear description of the issue
- Steps to reproduce
- Expected vs actual behavior
- Environment details (OS, Docker version, Python version)
- Relevant logs or error messages
- Screenshots if applicable

**Process:**
1. Check if issue already exists
2. Open new issue using [Bug Report Template](.github/ISSUE_TEMPLATE/bug_report.md)
3. Provide complete information
4. Respond to maintainer questions

---

## Submitting a Challenge

### Before You Begin

**Read these first:**
- [Challenge Design Guide](docs/CHALLENGE-DESIGN-GUIDE.md) - Design principles and patterns
- [ADR Guide](docs/ADR-GUIDE.md) - Architecture decision records
- [FinOps Playbook](docs/FINOPS-PLAYBOOK.md) - Cost optimization strategies

**Requirements:**
- Challenge must be based on real production experience
- Include Phase 2 twist (requirements evolution)
- Provide automated validators
- Complete documentation
- Reference solution (kept in `solutions/` directory)

### Challenge Structure

Your challenge must follow this structure:

```
challenge-name/
├── problem-statement.md          # Business context & requirements
├── data-generators/              # Docker services producing live data
│   ├── docker-compose.yml
│   ├── generator-configs/
│   └── README.md                # Setup instructions
├── architecture/
│   ├── TEMPLATE.md              # Starter ADR template
│   └── reference-diagrams/      # Example architectures (optional)
├── validators/
│   ├── validator.py             # Automated test suite
│   ├── test-scenarios/          # Edge cases & failure modes
│   └── README.md                # How to run validators
├── workspace/                    # Participant workspace
│   └── README.md                # Starter instructions
├── solutions/                    # Reference implementations
│   ├── APPROACH_A.md
│   └── APPROACH_B.md            # Multiple valid approaches
└── README.md                    # Challenge overview
```

### Required Components

**1. Problem Statement**
- Clear business context
- Technical requirements
- Success criteria
- Constraints (cost, time, resources)
- Phase 2 twist description

**2. Data Generators**
- Containerized services (Docker Compose)
- Realistic failure modes (late data, duplicates, schema drift)
- Configurable generation rates
- Clear documentation

**3. Validators**
- Automated correctness tests
- Performance benchmarks
- Cost efficiency checks
- Clear pass/fail criteria
- Helpful error messages

**4. Documentation**
- Setup instructions
- Expected outcomes
- Common pitfalls
- Reference architectures
- ADR templates

**5. Reference Solution**
- At least one complete implementation
- ADRs documenting key decisions
- Cost analysis
- Performance benchmarks

### Submission Process

**Step 1: Propose**
1. Open issue using [Challenge Proposal Template](.github/ISSUE_TEMPLATE/challenge-proposal.md)
2. Include:
   - Challenge overview
   - Learning objectives
   - Technical complexity
   - Phase 2 twist
   - Why this matters (production relevance)

**Step 2: Design Discussion**
- Maintainers review within 3 business days
- Expect questions and suggestions
- Iterate on design based on feedback
- Get approval before implementation

**Step 3: Implementation**
1. Fork the repository
2. Create branch: `challenge/your-challenge-name`
3. Implement all required components
4. Test thoroughly in clean environment
5. Document everything clearly

**Step 4: Pull Request**
1. Ensure all validators pass
2. Run `docker-compose up` successfully
3. Verify documentation is complete
4. Submit PR with description:
   - What the challenge teaches
   - Difficulty level
   - Estimated completion time
   - Prerequisites
   - Link to original proposal issue

**Step 5: Review**
- Two maintainers review each challenge
- Expect 1-2 rounds of feedback
- Address feedback promptly
- Maintainers respond within 3 business days

**Step 6: Merge & Recognition**
- Once approved, maintainers merge
- Challenge published in next release
- You're credited as challenge author
- Added to [Contributors Hall of Fame](CONTRIBUTORS.md)

---

## Quality Standards

All contributions must meet these standards:

### Code Quality

**For Challenges:**
- Data generators must run reliably in Docker
- Validators must pass consistently
- No hardcoded paths or credentials
- Clear error messages
- Documented dependencies

**For Code Contributions:**
- Follow existing code style
- Include tests where applicable
- Document complex logic
- No unnecessary dependencies

### Documentation Quality

- Clear, concise writing
- Proper grammar and spelling
- Code examples that work
- Links verified
- Screenshots where helpful
- Appropriate technical depth

### Testing

**Before submitting:**
- Test on clean system
- Verify Docker containers start
- Run all validators
- Check documentation links
- Test on macOS, Linux, and Windows (if possible)

---

## Review Process

### What to Expect

**Timeline:**
- Initial review: 3 business days
- Follow-up reviews: 2-3 business days
- Total time: 1-3 weeks depending on complexity

**Review Focus:**
- Technical correctness
- Production relevance
- Documentation clarity
- Validator reliability
- User experience

**Feedback Types:**
- **Required changes** - Must address before merge
- **Suggestions** - Improvements you can choose to make
- **Questions** - Clarifications needed

### Responding to Feedback

**Best practices:**
- Address all required changes
- Ask questions if feedback unclear
- Update PR with requested changes
- Mark conversations resolved when addressed
- Be professional and respectful

### After Merge

- Your contribution is live!
- Monitor for issues or questions
- Help maintain what you contributed
- Consider becoming a regular contributor

---

## Recognition

### Challenge Authors

Each challenge you create:
- Credits you in challenge README
- Links to your GitHub profile
- Counts toward Hall of Fame status
- Can be featured in your portfolio

### Regular Contributors

Active contributors receive:
- Recognition in [CONTRIBUTORS.md](CONTRIBUTORS.md)
- Invitation to contributor Discord channel
- Opportunity to become maintainer
- Community respect and gratitude

### Maintainers

Outstanding contributors may be invited to join as maintainers. Maintainers:
- Review pull requests
- Guide project direction
- Mentor newcomers
- Make final decisions on contributions

See [MAINTAINERS.md](MAINTAINERS.md) for governance details.

---

## Getting Help

### Where to Ask

**Technical questions:**
- [Discord #contributors](https://discord.gg/yourlink) - Real-time help
- [GitHub Discussions](https://github.com/DatechCommunity/os-portfolio-projects/discussions) - Long-form questions

**Process questions:**
- See [SUPPORT.md](SUPPORT.md)
- Ask in Discord #general

**Security concerns:**
- Follow [SECURITY.md](SECURITY.md) guidelines
- Do not open public issues for vulnerabilities

### Common Questions

**Q: How long does review take?**
A: Maintainers aim to provide initial review within 3 business days. Complex challenges may require multiple review rounds.

**Q: Can I work on multiple challenges simultaneously?**
A: Yes, but we recommend completing one before starting another to maintain quality.

**Q: What if I disagree with feedback?**
A: Discussion is welcome! Explain your reasoning respectfully. Maintainers have final say but will consider all viewpoints.

**Q: Can I abandon a contribution?**
A: Yes. Just comment on the issue/PR. No penalties. We appreciate whatever effort you contributed.

**Q: How do I become a maintainer?**
A: Consistent high-quality contributions and active community participation. Maintainers reach out when ready.

---

## Community Guidelines

### Code of Conduct

All contributors must follow our [Code of Conduct](CODE_OF_CONDUCT.md).

**Expected behavior:**
- Be respectful and professional
- Welcome newcomers warmly
- Provide constructive feedback
- Focus on what's best for the community
- Show empathy and patience

**Not tolerated:**
- Harassment or discrimination
- Trolling or insulting comments
- Personal attacks
- Publishing others' private information
- Spam or self-promotion

**Enforcement:**
- Violations reported to maintainers
- Maintainers investigate privately
- Actions range from warning to ban
- Appeal process available

### Communication Standards

**Pull Request Comments:**
- Be specific about requested changes
- Explain why changes are needed
- Suggest alternatives when possible
- Acknowledge good work

**Issues and Discussions:**
- Search before posting duplicates
- Provide context and details
- Stay on topic
- Update if situation changes

**Discord:**
- Use appropriate channels
- Be patient with newcomers
- Share knowledge freely
- Keep conversations professional

---

## Technical Guidelines

### Git Workflow

**Branch Naming:**
- Feature: `feature/description`
- Bug fix: `fix/description`
- Challenge: `challenge/name`
- Documentation: `docs/description`

**Commit Messages:**
```
Type: Brief description (50 chars max)

Longer explanation if needed. What changed and why.
Reference issues: Fixes #123

- Bullet points okay
- For detailed changes
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

### Docker Best Practices

- Use official base images
- Pin versions explicitly
- Minimize layers
- Clean up apt cache
- Use multi-stage builds when appropriate
- Document resource requirements

### Python Standards

- Follow PEP 8 style guide
- Use type hints
- Write docstrings
- Keep functions focused
- Test edge cases
- Handle errors gracefully

---

## Resources

### For Challenge Authors
- [Challenge Design Guide](docs/CHALLENGE-DESIGN-GUIDE.md)
- [ADR Guide](docs/ADR-GUIDE.md)
- [FinOps Playbook](docs/FINOPS-PLAYBOOK.md)
- [Example Challenges](beginner/ecommerce-etl-foundation/)

### For All Contributors
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Support Guide](SUPPORT.md)
- [Security Policy](SECURITY.md)
- [Discord Community](https://discord.gg/yourlink)

### Learning Resources
- [Learning Paths](docs/LEARNING-PATHS.md)
- [Recommended Prerequisites](docs/LEARNING-PATHS.md#prerequisites)

---

## Thank You

Every contribution—no matter how small—makes this project better. Whether you're fixing a typo, designing a challenge, or mentoring newcomers, you're helping data engineers worldwide build stronger portfolios.

**Questions?** Ask in [Discord](https://discord.gg/yourlink) or [open a discussion](https://github.com/DatechCommunity/os-portfolio-projects/discussions).

---

<div align="center">

**[Documentation](docs/) • [Browse Challenges](README.md#repository-structure) • [Community](https://discord.gg/yourlink) • [Code of Conduct](CODE_OF_CONDUCT.md)**

*Licensed under [MIT](LICENSE) • Maintained by the Datech Community*

**Thank you for contributing to OS-Portfolio-Projects!**

</div>
