# QA Service

## **User Story: Workflow toolbox for QA process**

* **As a** QA engineer and developer
* **I want** CI that can run automatically or manually on either QA branch or the branch that wished to merged to QA
* **So that** I can control the QA process better

✅ **Acceptance Criteria:**
- [X] **AC.1 — Automatic Trigger on QA Branch:** The CI workflow **automatically runs** when code is pushed to the `QA` branch.  
- [X] **AC.2 — Automatic Trigger on PRs Targeting QA:** The CI workflow **automatically runs** when a pull request is opened, synchronized, or reopened with the **target branch set to `QA`**.  
- [X] **AC.3 — Manual Trigger Support:** The CI workflow can be **manually triggered** via `workflow_dispatch` for:  
      - The `QA` branch  
      - Any feature branch intended to be merged into `QA`
- [x] **AC.4 — Branch Parameterization for Manual Runs:**  When triggered manually, the workflow **accepts a branch name as an input parameter** and runs QA checks against that branch.  
- [X] **AC.5 — Consistent QA Checks:** Regardless of trigger type (auto or manual), the workflow executes the **same QA validation steps** (e.g., build, tests, linting, security scans) to ensure consistent results.  
- [X] **AC.6 — Execution Feedback:** The workflow **reports pass/fail status** and provides **detailed logs** for each QA check step in the Actions UI.
- [X] **AC.7 — Deliverable Ouput:** The output should be a workflow template where it can be given out to other user repositories without expose the detail workflow configuration

## **User Story: Mandatory Checklist at PR into QA**

* **As a** QA engineer
* **I want** an PR to run full CI/CD before merge to QA branch
* **So that** I can be confident that the build is minimally deployable

✅ **Acceptance Criteria:**

- [X] **AC.1:** Code quality checks (linting, security scanning, code coverage) executed automatically
- [X] **AC.2:** Full test suite for functionality and component test.
- [X] **AC.3:** Build SW and packaging them sucessfully.
- [ ] **AC.4:** Dependency vulnerability checks and license compliance validation.
      - [X] **AC.4.1:** Design concept & Boilerplate
      - [ ] **AC.4.2:** Implementation (Will be implemented once the User Story for Security is given)
- [ ] **AC.5:** Artifact should be tagged with something that is traceable to the current commit.
      - [X] **AC.5.1:** Design concept & Boilerplate
      - [ ] **AC.5.2:** Implementation (Will be implemented when the infrastructure provision pipeline exist)
- [ ] **AC.6:** Deployment should be run only when trigger manually.
      - [X] **AC.6.1:** Design concept & Boilerplate
      - [ ] **AC.6.2:** Implementation (Will be implemented when the infrastructure provision pipeline exist)
- [ ] **AC.7:** Automatically add PIC for QA branch to PR's review if not already.
      - [X] **AC.7.1:** Design concept & Boilerplate
      - [ ] **AC.7.2:** Implementation (Will be implemented at another time)

## **User Story: New Merged Quality Healthcheck**

* **As a** QA engineer
* **I want** new merged from QA to run full CI/CD and basic system testing
* **So that** I can have a fast feedback on 

✅ **Acceptance Criteria:**

- [ ] **AC.1:** Code quality checks (linting, security scanning, code coverage) executed automatically
  - [X] **AC.1.1:** - Boilerplate
  - [ ] **AC.1.2:** - Implement (Will be implemented when new User Story for integrated external server)
- [X] **AC.2:** Full test suite for functionality and component test.
- [X] **AC.3:** Build SW and packaging them sucessfully.
- [ ] **AC.4:** Dependency vulnerability checks and license compliance validation.
      - [X] **AC.4.1:** Design concept & Boilerplate
      - [ ] **AC.4.2:** Implementation (Will be implemented once the User Story for Security is given)
- [ ] **AC.5:** Deployment should be run only when trigger manually.
      - [X] **AC.5.1:** Design concept & Boilerplate
      - [ ] **AC.5.2:** Implementation (Will be implemented when the infrastructure provision pipeline exist)

## **User Story: Multi-Service Testing on QA environment**

* **As a** QA engineer and DevOps
* **I want** a CD/CT to check for deployment and E2E testing, and other Non-functional testing 
* **So that** I can quick check for releasable service

- [ ] **AC.1:** Check infrastructure provision and environment configuration before deploy
- [ ] **AC.2:** Deploy end-to-end services (UI, API-gateway, backend-services) on QA environment and check for time till running.
- [ ] **AC.3:** Perform regression end-to-end test as default, can be configured to be disabled.
- [ ] **AC.4:** Perform non-functional test as default, can be configured to be disabled.
- [ ] **AC.5:** Teardown deployment at the end as default, can be configured to be disabled.
- [ ] **AC.6:** The system's SLA, SLO and SLI for non-functional test should be configurable.