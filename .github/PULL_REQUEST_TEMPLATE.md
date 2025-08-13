## ✅ Pre-Submission Checklist

Before submitting this PR, confirm you have completed all items:

### 🔹 Functional Requirements

- [ ] Automation runs on a fresh Ubuntu 24.04 server without manual steps.
- [ ] Dedicated `sudo` user with SSH key login created.
- [ ] Root SSH login disabled.
- [ ] Docker and fail2ban installed & configured.
- [ ] Sample containerized app deployed and accessible.
- [ ] Logs rotated and remain clean.

### 🔹 Idempotency

- [ ] Multiple runs produce the same result without duplication.
- [ ] Existing configs updated, not recreated.

### 🔹 Code Quality & Structure

- [ ] Follows repo structure.
- [ ] All variables in one vars file.
- [ ] No hardcoded secrets or environment values.
- [ ] Code is readable, modular, and clean.

### 🔹 Documentation

- [ ] `README.md` updated with setup instructions.
- [ ] `docs/decision-log.md` updated with tool choices.
- [ ] All commands, ports, and variables documented.

### 🔹 Collaboration

- [ ] Small, descriptive commits.
- [ ] Reviewed at least one other PR.
- [ ] Ready to respond to feedback.

---

**Note:** This is a public community assignment — approved solutions are tagged and remain public as part of your portfolio.
