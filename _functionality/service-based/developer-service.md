# Developer Service

## **User Story: Fast Feedback at Commit Stage**

* **As a** developer working on feature branch, without creating PR
* **I want** to test only my functionality every push not the entire functionality test suite
* **So that** I can received a faster feedback on without waiting for 

✅ **Acceptance Criteria:**

- [ ] **AC.1:** Automatic linting and static analysis.
- [ ] **AC.2:** Only full test suite of component test should be executed.
- [ ] **AC.3:** Should only run the entire functionality of my choice and run full test if needed.
- [ ] **AC.4:** Trash dependencies detection and packaging to artifact.
- [ ] **AC.5:** Dependency vulnerability checks and license compliance validation if needed.
- [ ] **AC.5:** Removed artifacts after each build.