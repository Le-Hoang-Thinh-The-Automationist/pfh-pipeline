# Utility Service

## **User Story: Manual Trigger for On-Demand Test Execution**

* **As a** Developer
* **I want** to manually trigger a GitHub Action to run a specific subset of tests (unit, integration, or E2E)  
* **So that** I can validate changes or investigate issues without waiting for automated pipeline triggers  

✅ **Acceptance Criteria:**  
- [ ] **AC.1:** Workflow can be triggered manually from the GitHub Actions UI with selectable test type parameters.  
- [ ] **AC.2:** Only the selected test suite runs; unrelated tests are skipped.  
- [ ] **AC.3:** Test results are displayed in the Actions log and stored as artifacts for later review.  
- [ ] **AC.4:** Workflow fails if tests do not meet the defined pass criteria.  

---

## **User Story: Manual Trigger for Dependency & Security Audit**

* **As a** Developer and DevOps engineer
* **I want** to manually run a GitHub Action that scans dependencies for vulnerabilities and license compliance  
* **So that** I can ensure the codebase is secure and compliant before a release or deployment  

✅ **Acceptance Criteria:**  
- [ ] **AC.1:** Workflow can be triggered manually with no code changes required.  
- [ ] **AC.2:** Performs dependency vulnerability scanning using the approved security tool.  
- [ ] **AC.3:** Generates a report with severity levels and actionable remediation steps.  
- [ ] **AC.4:** Validates license compliance for all dependencies and flags violations.  