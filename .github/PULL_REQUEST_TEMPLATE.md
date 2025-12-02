# Pull Request Template: Apex Engineering Review

This template enforces the **Zero-Defect, High-Velocity, Future-Proof** standard dictated by the Apex Technical Authority.

Before merging, ensure all checks pass and the functionality aligns with the system's **Single Source of Truth (SSOT)**.

---

## 1. Summary & Context

<!-- Briefly describe the changes. Why is this PR necessary? Link to relevant issues (e.g., `Closes #123`). -->

**What this PR addresses:**

- [ ] **Feature:** New functionality implemented.
- [ ] **Bugfix:** Critical issue resolved.
- [ ] **Refactor:** Code structure/performance improvement.
- [ ] **Documentation:** Update to documentation artifacts.

**Related Issues:**

- 

---

## 2. Architectural & Code Review Checklist

*Self-review against Apex Principles before requesting reviews.*

### A. Core Principles (SOLID/DRY/YAGNI)

- [ ] **SOLID:** Are interfaces well-defined? (Especially for AI/API interactions).
- [ ] **DRY:** Have I avoided duplication of logic?
- [ ] **YAGNI:** Is this implementation minimal to solve the immediate requirement? Avoid premature generalization.

### B. Technology Stack Compliance (React Native / TypeScript)

- [ ] **TypeScript Strictness:** Are all new utilities/components fully typed? No `any` allowed.
- [ ] **State Management:** If state is modified, is the update traceable and atomic?
- [ ] **Performance:** Are list rendering operations optimized (e.g., using `FlatList` with correct `keyExtractor`)?
- [ ] **Native Bridge:** If native modules were touched, have I verified platform compatibility (iOS/Android)?

### C. AI/Data Integrity (For EcoSnap Logic)

- [ ] **Model Handlers:** If the classification pipeline changed, is the data contract between the frontend and the inference service clear?
- [ ] **Error Handling:** Have I gracefully handled API timeouts or low-confidence classification results?
- [ ] **History Persistence:** If history/logging is affected, is data persistence verified?

---

## 3. Testing & Verification

*Describe the verification steps taken for this change.*

**Test Strategy:**

1.  **Unit Tests:** Were `Vitest` tests written/updated to cover new logic? (Target: >90% coverage in modified files).
2.  **E2E Smoke Test:** Ran Playwright commands on the main user journey affected by this change.
3.  **Manual Verification:** 
    *   *Steps taken on physical device/emulator:* 

---

## 4. Final Sign-Off

By submitting this PR, I attest that this change adheres to the **Apex Technical Authority** standards and will not introduce technical debt.

**Reviewers Requested:**

- [ ] **Architectural Reviewer:**
- [ ] **Domain Expert Reviewer:**

**Commit Status:**

text
This PR is ready for automated CI checks and peer review.

Repository URL for Reference: https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App
