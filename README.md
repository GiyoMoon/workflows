<div align="center"> <img src="./assets/logo.png" width=200 /></div>
<h1 align="center">Workflows</h1>
<div align="center">
 <strong>
  A collection of reusable Github workflows which I use across my projects
 </strong>
</div>

<br />

### 🦀 `rust-checks`
Executes rust lints, checks and tests. Properly caches crates and builds.
- `cargo fmt`
- `cargo clippy`
- `cargo check`
- `cargo audit`
- `cargo test`

**Inputs**
- `rust-version` (Optional): Rust toolchain version to use. Default is `beta`
- `workdir` (Optional): Directory of the Rust project to check. Default is root of the repository. Useful for monorepos
---

### 🐳 `docker-build`
Builds and publishes a Docker image to the Github Registry.

**Inputs**
- `images`: Image name. Example: `ghcr.io/giyomoon/workflows`
- `platforms` (Optional): Platforms to build the image for. Default: `linux/amd64,linux/arm64`
- `workdir` (Optional): Directory of the Dockerfile to build. Default is the root of the repository. Useful for monorepos
---
