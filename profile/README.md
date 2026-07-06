<p align="center">
  <img src="https://raw.githubusercontent.com/srelens/srelens/main/apps/desktop/src/assets/srelens-logo.svg" alt="SRELens" width="420" />
</p>

<p align="center">
  <strong>Open-source tooling for SREs.</strong>
</p>

---

## SRELens

[**SRELens**](https://github.com/srelens/srelens) is a fast, lightweight Kubernetes IDE built with [Tauri v2](https://v2.tauri.app) and a pure-Rust core — a modern take on Lens/Freelens without Electron.

What makes it different:

- ⚡ **Tauri, not Electron** — system WebView, small binary, low memory footprint.
- 🦀 **Pure-Rust backend** — cluster connections, watches, exec, port-forward, and logs run on `kube-rs` + `tokio`. No Node.js in the core.
- 🤖 **MCP-native by design** — every backend capability is also exposed as a [Model Context Protocol](https://modelcontextprotocol.io) tool, so AI agents like Claude can drive your clusters through the exact same code paths as the UI. A CI completeness test guarantees the two surfaces never drift.
- ✅ **Test-driven** — TDD is mandatory and coverage floors are enforced as hard CI gates.

**Status:** early, active development — the browse/operate core (live resource views, YAML editing, pod terminals, logs, port-forwarding, Helm, metrics) works end-to-end. Contributions welcome; see the [developer guide](https://github.com/srelens/srelens/blob/main/docs/DEVELOPMENT.md).
