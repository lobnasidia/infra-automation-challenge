# 🧩 Automate Server Bootstrap & App Deployment

**Scalyz 30 Days Job-Ready Challenge — Chapter 2: Automation & Infrastructure-as-Code**

---

## 📖 About This Assignment

This project is part of the **Scalyz 30 Days Job-Ready Challenge** — a public, community-driven assignment designed to push you beyond tutorials and into **real engineering work**.

All submissions are **public**.

- **Approved solutions** are **tagged** in the repository.
- **Current work** is visible in **open Pull Requests** with active discussions.

**Your role:** behave like a professional engineer — read existing discussions, learn from others, contribute ideas, and deliver your own solution.

---

## 💬 How to Participate

1. **Read ongoing discussions** in existing Pull Requests.
2. **Create issues** if you need help or spot potential improvements.
3. Ask for guidance **directly in the Scalyz community** or by commenting on PRs.
4. Submit your solution via Pull Request for review.

> 💡 This is a **public community assignment**.  
> The goal is for you to **experience the full engineering workflow**: reading requirements, collaborating, solving problems, and proving — to yourself and others — that you can do the job.

---

## 📝 Assignment Title

**Mission:** Automate the bootstrap of a fresh Ubuntu server, secure it, install core tools, deploy a sample containerized app, and ensure the process is **idempotent** and **repeatable**.

---

## 🎯 Problem Statement

Our fictional client is rolling out new apps across multiple environments.  
Their manual deployment process is slow, inconsistent, and error-prone.

They need **one reusable automation flow** that:

- Works on any fresh Ubuntu 24.04 server.
- Configures security and access.
- Deploys a containerized sample app.
- Can be re-run safely without breaking anything.

---

## ✅ Requirements

Your automation must:

- Create a dedicated user with `sudo` privileges and SSH key-based login.
- Disable root SSH login.
- Install and configure:
  - Docker (latest stable)
  - fail2ban
- Deploy a containerized sample app (provided or self-built).
- Configure log rotation and ensure logs remain clean.
- Be **idempotent** — multiple runs must not cause duplication or errors.

---

## 📦 Structure

You will work inside the provided repo structure:

```

infra-automation-challenge/
├── ansible/              # Or scripts/ if using Bash
│   ├── roles/
│   ├── playbooks/
│   └── vars/
├── docker/
│   └── app/
├── docs/
├── scripts/
└── tests/

```

---

## ⚙️ Constraints

- Use your own local VM or any free-tier cloud environment.
- No hardcoded environment-specific values or secrets.
- All configurable variables must be in one documented file.
- Automation must run **headless** (no manual prompts).

---

## 🔍 Evaluation Process

1. Submit a Pull Request to this repository.
2. **GitHub Actions** will:
   - Lint and validate syntax.
   - Check idempotency.
   - Verify the app is deployed and reachable.
3. **Community Review**:
   - At least 2 peers review your PR.
   - Feedback focuses on code quality, maintainability, security, and correctness.
4. **Approval & Tagging**:
   - Approved PRs are tagged and merged into the main branch.

---

## 📌 Tips for Success

- Review existing PRs before starting — you’ll learn faster.
- Ask questions in the Scalyz community.
- Document your decisions in `docs/decision-log.md`.
- Keep commits small and descriptive.
- Remember: this is about **building the habit** of delivering professional-grade work.

---

## 🚀 Your Next Step

- Fork the repo:
  ```bash
  git clone https://github.com/scalyzcommunity/infra-automation-challenge.git
  ```

* Work on your solution locally.
* Submit your PR when ready.

Let’s see what you can build.
Prove it — to the community, to future employers, and to yourself.

---

**— Scalyz Community**
_Engineer. Collaborate. Deliver._

---

## ✅ Pre-Submission Checklist

Before you open a Pull Request, confirm that you have completed all items below.  
**Tip:** Copy this checklist into your PR description and tick each item.

### 🔹 Functional Requirements

- [ ] Automation runs successfully on a fresh Ubuntu 24.04 server without manual intervention.
- [ ] A dedicated `sudo` user is created with SSH key-based login.
- [ ] Root SSH login is disabled.
- [ ] All required packages (Docker, fail2ban) are installed and configured.
- [ ] The sample containerized app is deployed and accessible on the documented port.
- [ ] Logs are rotated and remain clean after deployment.

### 🔹 Idempotency

- [ ] Running the automation multiple times produces the same end state without errors or duplication.
- [ ] Existing configurations are updated instead of re-created.

### 🔹 Code Quality & Structure

- [ ] File and folder structure follows the provided repository layout.
- [ ] All configurable variables are in one documented vars file.
- [ ] No hardcoded environment-specific values or secrets.
- [ ] Code is modular, readable, and free of unused files.

### 🔹 Documentation

- [ ] `README.md` includes clear setup and execution instructions.
- [ ] `docs/decision-log.md` explains tool choices and key decisions.
- [ ] All commands, ports, and variables are documented for future maintainers.

### 🔹 Git & Collaboration

- [ ] Commits are small and descriptive.
- [ ] Branch name is descriptive (e.g., `feature/automation-bootstrap`).
- [ ] I have reviewed at least one existing PR in the repository.
- [ ] I am ready to respond to reviewer feedback in the PR discussion.

---

**Reminder:** This is a public community assignment.  
Approved solutions will be tagged and remain visible as part of your **public engineering portfolio**.
