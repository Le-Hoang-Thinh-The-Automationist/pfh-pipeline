# QA Service

## **User Story: Mandatory Checklist at PR into QA**

* **As a** QA engineer
* **I want** an PR to run full CI/CD before merge to QA branch
* **So that** I can be confident that the build is minimally deployable

✅ **Acceptance Criteria:**

- [ ] **AC.1:** Code quality checks (linting, security scanning, code coverage) executed automatically
- [ ] **AC.2:** Full test suite for functionality and component test.
- [ ] **AC.3:** Build SW and packaging them sucessfully.
- [ ] **AC.4:** Dependency vulnerability checks and license compliance validation.
- [ ] **AC.5:** Artifact should be tagged with something that is traceable to the current commit.
- [ ] **AC.6:** Deployment should be run and monitor for healthy deploy.
- [ ] **AC.7:** After Deployment success, tear down the deployment immediately to save resource.
- [ ] **AC.8:** After Merge PR, clean all artifacts of the PR to save resource.
