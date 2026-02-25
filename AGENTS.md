## Cursor Cloud specific instructions

This is a **documentation-only repository** containing OCI GPU onboarding guides (Markdown) and Kubernetes YAML examples. There is no application code, no build system, no runtime services, and no automated test suite.

### Repository content

- `nvidia/` and `amd/` — GPU-specific quick-start guides organized by GPU family (B200, GB200, GB300, MI300X, MI355X)
- `amd/MI355X/k8s/` and `nvidia/B200/` — Example Kubernetes YAML manifests
- `media/icons/` — SVG badge icons

### Development tools

| Tool | Command | Purpose |
|------|---------|---------|
| markdownlint | `markdownlint '**/*.md'` | Lint Markdown files for style/formatting |
| yamllint | `yamllint -d relaxed <file>` | Validate YAML syntax on K8s manifests |
| grip | `grip 0.0.0.0:6419` | Render docs as GitHub-flavored Markdown (port 6419) |

### Notes

- `grip` renders Markdown locally via GitHub's CSS; it may hit GitHub API rate limits without a token. For unauthenticated use, rendering is local-only (no API calls needed for basic rendering).
- The existing Markdown and YAML files have numerous pre-existing lint warnings (line length, heading structure, trailing spaces). These are in the upstream content — do not treat them as regressions.
- `yamllint` is installed to `~/.local/bin`; ensure `PATH` includes it (`export PATH="$HOME/.local/bin:$PATH"`).
- Contribution guidelines are in `CONTRIBUTING.md` (requires Oracle Contributor Agreement sign-off on commits).
