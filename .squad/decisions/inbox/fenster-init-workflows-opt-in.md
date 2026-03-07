### 2026-03-07: squad init --no-workflows flag for opt-in workflow installation
**By:** Fenster (Core Dev)
**What:** `squad init` now accepts `--no-workflows` to skip GitHub workflow installation. Default remains `true` (framework workflows are installed). The `RunInitOptions` interface accepts `includeWorkflows?: boolean`.
**Why:** Users in repos with existing CI/CD should be able to skip Squad's framework workflow installation. The 4 framework workflows are safe, but user control matters.
**Impact:** CLI help text updated, `RunInitOptions` extended, `initSquad` respects the flag.
