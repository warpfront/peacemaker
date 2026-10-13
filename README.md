# PeaceMaker

PeaceMaker's AMDGPU and AIE2P (XDNA2) kernel crates, with the full commit history of those crates.

## This repository is a mirror

The canonical development tree is **https://github.com/warpfront/hipfire**. This repository is generated from it by
`scripts/mirror-split.sh` and is rewritten on each update: open issues and pull requests, and
send contributions, at https://github.com/warpfront/hipfire (see its `CONTRIBUTING.md`), not here.

Author and commit dates and the commit topology of the kept paths are preserved. Commit
messages are replaced by `Mirror source update` plus the canonical source commit hash.

Generated from canonical commit `302cb49fffae5d39ab2bf84d9c56fb642c457fb3`.

## Contents

Crates (each lives at `crates/<name>`):

- `peacemaker-author`
- `peacemaker-ir`
- `peacemaker-isa`
- `peacemaker-lift`
- `peacemaker-npu`
- `peacemaker-rip`
- `radiowave`

`Cargo.toml`, `Cargo.lock`, `LICENSE`, `LICENSE-LLVM-EXCEPTION`, `README.md` and `.gitignore` at the root
are generated for this mirror. Everything else is copied from the canonical tree unchanged.

```
cargo build --workspace
cargo test --workspace
```

Tests that need a ROCm toolchain use `ROCM_PATH` (default `/opt/rocm`).

## History notes

- History of `crates/hipfire-isa` is kept under `crates/peacemaker-isa`.
- History of `crates/hipfire-rip` is kept under `crates/peacemaker-rip`.
- History of `crates/pm-npu` is kept under `crates/peacemaker-npu`.

## License

Apache-2.0 (see `LICENSE`, `LICENSE-APACHE`, `LICENSE-MIT` and `NOTICE`); files derived from the LLVM
and mlir-aie projects are `Apache-2.0 WITH LLVM-exception` (see `LICENSE-LLVM-EXCEPTION`).
Individual files keep their SPDX headers.
