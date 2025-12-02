# 🤝 Contributing to EcoSnap-AI-Waste-Classification-Mobile-App

As the **Apex Technical Authority**, we welcome contributions that enhance the robustness, accuracy, and future-proofing of this Waste Classification Mobile Application. All contributions must adhere to the **Zero-Defect, High-Velocity, Future-Proof** philosophy.

## 1. Architectural Alignment & Standards

Before submitting any Pull Request (PR), ensure your changes align with the established 2026 mobile development standards and the core principles defined in our `AGENTS.md` file. 

**Key Pillars for Review:**

*   **TypeScript Strictness:** All new or modified TypeScript code must be strictly typed (no `any`).
*   **Performance Focus:** Mobile performance is paramount. Avoid unnecessary re-renders and inefficient state management.
*   **AI Model Integrity:** Changes touching the Computer Vision pipeline (TensorFlow Lite/CoreML wrappers) must include robust validation logic for input normalization and output confidence scores.
*   **DX (Developer Experience):** Maintain high standards for code clarity, adhering to the **SOLID**, **DRY**, and **YAGNI** principles.

## 2. Workflow: The Four Stages of Contribution

We utilize a standard GitHub flow, heavily augmented by automated checks enforced by our CI/CD pipeline (`.github/workflows/ci.yml`).

### Stage 1: Local Setup & Branching

1.  **Fork:** Fork this repository: `https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App`.
2.  **Clone:** Clone your fork locally.
3.  **Branching:** Create a new feature branch based off `main`. Name it descriptively using prefixes:
    *   `feat/short-description` for new features.
    *   `fix/issue-number-description` for bug fixes.
    *   `refactor/area-description` for structural improvements.

bash
git clone https://github.com/chirag127/EcoSnap-AI-Waste-Classification-Mobile-App.git
cd EcoSnap-AI-Waste-Classification-Mobile-App
git checkout -b feat/add-new-recycling-facility-lookup


### Stage 2: Development & Verification (Local Enforcement)

Before committing, ensure all local checks pass. This preempts CI failures and speeds up the review process.

1.  **Install Dependencies:**
    bash
npm install

2.  **Run Linter/Formatter (Biome):** Use Biome for instantaneous formatting and linting checks.
    bash
npm run lint:fix

3.  **Run Unit Tests (Vitest):** Ensure all affected unit tests pass.
    bash
npm run test:unit

4.  **Verification:** Run the application to manually verify your changes in the Expo environment.
    bash
npm run dev


### Stage 3: Submission (Pull Request)

1.  **Commit:** Commit changes following [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
    bash
git push origin feat/short-description

2.  **PR Creation:** Open a Pull Request targeting the `main` branch of `chirag127/EcoSnap-AI-Waste-Classification-Mobile-App`.
3.  **Template Usage:** **MANDATORY:** Use the provided `PULL_REQUEST_TEMPLATE.md` to structure your submission. Clearly document the motivation, technical approach, and verification steps taken.

### Stage 4: Review and Iteration

*   The CI pipeline will automatically trigger the Build, Test, and Lint stages. **Do not request a review until all checks pass.**
*   Address feedback promptly. Major architectural disagreements will be resolved by the Apex Technical Authority based on alignment with long-term maintainability goals.

## 3. Reporting Issues and Security

If you discover a bug or a security vulnerability, **DO NOT** open a public issue immediately. Refer to the dedicated files:

*   **Bugs:** Please use the issue template located at `.github/ISSUE_TEMPLATE/bug_report.md`.
*   **Security:** Follow the secure disclosure process outlined in `.github/SECURITY.md`.

## 4. Code Style & Commit Hygiene

We enforce a high standard for code readability and history integrity. 

*   **Linter:** All code must pass Biome checks without errors or warnings.
*   **Commits:** Commit messages must be atomic and descriptive. Imperfect, overlapping commits will be squashed during merge approval to maintain a clean project history.

--- 
*Thank you for contributing to the future of sustainable technology.*
