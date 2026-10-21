# Project continuity — PiVPN fork

Updated October 21, 2026. This is a source-based restart record for this fork; no installed VPN or host configuration was inspected.

## Repository baseline

- Repository: `Ltnetsudo/pivpn`; default branch: `master`.
- Upstream recorded by GitHub: `pivpn/pivpn`.
- Baseline commit: `2f64b12ec12017ad0c4c04558b3d83e466926382` (`docs: Add lockdown workflow`).
- Purpose in the source README: shell scripts for WireGuard/OpenVPN installation and management.
- The checked-in README contains a maintenance warning. Treat that as a statement in this snapshot; verify current upstream status before relying on it for new work.

## Resume and verify

Read [README.md](README.md), inspect the current branch/diff and the relevant scripts under `auto_install/`, `scripts/` and `ciscripts/`. No owner-specific host, VPN installation, custom configuration, active feature request or completed runtime test is documented in this continuity pass.

Do not run an installer merely to verify a documentation change; it modifies its target host. For future code work, select appropriate static checks and a deliberately isolated test environment after inspecting the affected scripts.

The existing `.github/workflows/publish-install.yml` targets master pushes and publishes `auto_install/` to GitHub Pages if enabled/configured. This pass changes root documentation only. No VPN configuration, host, keys or upstream source are modified.

## Handoff policy

Keep this root record updated with actual fork changes, relevant upstream revision, validation evidence and unresolved next steps. Record deployment/runtime details only when verified. Never commit private keys, VPN client profiles, host addresses or other private configuration. Existing upstream guidance remains in place.

Next action: establish the specific requested task and actual target environment before making runtime changes. This baseline must not be mistaken for a completed VPN setup or a current security assessment.
