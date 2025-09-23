# Developer Service

## **User Story: Fast Feedback at Commit Stage**

* **As a** developer working on feature branch, without creating PR
* **I want** to test only my functionality every push not the entire functionality test suite
* **So that** I can received a faster feedback on without waiting for 

✅ **Acceptance Criteria:**

- [X] **AC.1:** Automatic linting and static analysis.
- [X] **AC.2:** Only full test suite of component test should be executed.
- [X] **AC.3:** Should only run the entire functionality of my choice and run full test if needed.
- [X] **AC.4:** Trash dependencies detection and display the image size 
- [X] **AC.5:** Dependency vulnerability checks and license compliance validation if needed.
- [X] **AC.6:** Removed artifacts after each build.
- [X] **AC.7:** The Fast Feedback at Commit Stage shall not run when is has PR to merge QA.