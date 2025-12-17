# Roadmap

## Current Status (December 2025)

### Completed

- [x] **Hub-and-Spoke Mirror Infrastructure**
  - GitHub Actions workflow for multi-platform mirroring
  - Support for GitLab, Codeberg, and Bitbucket
  - Conditional execution via repository variables

- [x] **Security Hardening**
  - SSH host key verification (prevents MITM attacks)
  - Pinned GitHub Action versions (commit SHA references)
  - Minimal workflow permissions (`read-all`)
  - Job timeouts (10 minutes max)
  - Concurrency controls (serialized mirror operations)

- [x] **Documentation**
  - README with setup instructions
  - Security policy (SECURITY.md)
  - Roadmap (this file)

---

## Planned Features

### Phase 1: Core Configuration Reporter

- [ ] **Nickel Configuration Parsing**
  - Implement Nickel config file parser
  - Support for common config patterns
  - Schema validation

- [ ] **Report Generation**
  - Human-readable config reports
  - Diff reports for config changes
  - JSON/YAML export formats

- [ ] **CLI Interface**
  - Command-line tool for local usage
  - Integration with CI/CD pipelines
  - Exit codes for validation status

### Phase 2: Extended Platform Support

- [ ] **Additional Mirror Targets**
  - Gitea instances
  - SourceHut
  - Self-hosted GitLab

- [ ] **Branch Protection Sync**
  - Mirror branch protection rules
  - Sync repository settings where APIs allow

- [ ] **Status Reporting**
  - Mirror status dashboard
  - Failure notifications (email, Slack, etc.)
  - Mirror health checks

### Phase 3: Advanced Features

- [ ] **Selective Mirroring**
  - Branch filters (only mirror specific branches)
  - Path-based exclusions
  - Size limits for mirrors

- [ ] **Webhook Integration**
  - Real-time sync triggers
  - Cross-platform issue sync
  - PR/MR mirroring (experimental)

- [ ] **Audit Logging**
  - Track all mirror operations
  - Compliance reporting
  - Retention policies

### Phase 4: Enterprise Features

- [ ] **Multi-Organization Support**
  - Template for new repos
  - Centralized secret management
  - Organization-wide policies

- [ ] **Disaster Recovery**
  - Automatic failover
  - Backup verification
  - Recovery runbooks

---

## Contributing

Contributions are welcome! Please see the [SECURITY.md](SECURITY.md) for security guidelines when contributing.

## Questions or Suggestions?

Open an issue on GitHub to discuss new features or improvements.
