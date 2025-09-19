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
- [ ] **AC.6:** Deployment should be run only when trigger manually.
- [ ] **AC.7:** After Deployment success, check health running for a while before tear down the deployment to save resource.
- [ ] **AC.8:** After Merge PR, clean all artifacts of the PR to save resource.
- [ ] **AC.9:** Automatically add PIC for QA branch to PR's review if not already.

## **User Story: New Merged Quality Healthcheck**

* **As a** QA engineer
* **I want** new merged from QA to run full CI/CD and basic system testing
* **So that** I can have a fast feedback on 

✅ **Acceptance Criteria:**

- [ ] **AC.1:** Code quality checks (linting, security scanning, code coverage) executed automatically
- [ ] **AC.2:** Full test suite for functionality and component test.
- [ ] **AC.3:** Build SW and packaging them sucessfully.
- [ ] **AC.4:** Dependency vulnerability checks and license compliance validation.
- [ ] **AC.5:** QA should approve manually to continue deploy, else fails.
- [ ] **AC.6:** Deploy end-to-end services (UI, API-gateway, backend-services, infrastructure) on QA environment and check for time till running.
- [ ] **AC.7:** Perform regression end-to-end test as default, disable if to trigger manually.
- [ ] **AC.8:** Perform performance test as default, disable if to trigger manually.
- [ ] **AC.9:** Teardown deployment at the end as default, disable if trigger manually.

## **User Story: Latest QA Commit Status Tagging**

* **As a** QA engineer
* **I want** new merged from QA to run full CI/CD and basic system testing
* **So that** I can have a fast feedback on 