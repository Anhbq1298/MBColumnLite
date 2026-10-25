# Experimental full-feature WASM frontend branch

This branch is **not production-ready**. The production `main` site still calls the Singapore Render private API.

The browser worker is a compatibility scaffold only. The native source and build scripts are in the private `Anhbq1298/MBColumnLite-API` repository, branch `feature/wasm-full-feature`. No public WASM binary is deployed until the whole engine is validated.

**Acceptance before changing main:**
- End-to-end feature parity for section/rebar input, bundled bars, all load cases, slenderness, charts and reports.
- Baseline numerical comparisons of N/Mx/My, D/C, governing case and sample PM/MM/3D contours against existing JavaScript source.
- Load and stress tests (bad inputs, repeated Calculate, cancellations, cross-browser).
- Demonstrated offline calculation with no requests to Render and no source JS solver distributed.
- Security acknowledgment: WASM can be disassembled and cannot ensure IP secrecy.
