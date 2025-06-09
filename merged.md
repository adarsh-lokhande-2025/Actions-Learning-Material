# File: _index.md

---
title: "GitHub Actions Questions"
hidden: true
cascade:
    exam: "GitHub Actions"
    Description: "Mock exam questions for the GitHub Actions Certification Exam."
---

### GitHub Actions

{{< library-links questions="GitHub Actions" >}}


---

# File: question-001.md

---
question: "Which statement is correct regarding passing permissions to reusable workflows?"
title: "Question 001"
---


> https://docs.github.com/en/actions/using-workflows/reusing-workflows#access-and-permissions

1. [x] The `GITHUB_TOKEN` permissions passed from the caller workflow can be only downgraded by the called workflow.
1. [ ] The `GITHUB_TOKEN` permissions passed from the caller workflow can be only elevated by the called workflow.
1. [ ] The `GITHUB_TOKEN` permissions passed from the caller workflow can be both downgraded and elevated by the called workflow.
1. [ ] The `GITHUB_TOKEN` permissions passed from the caller workflow can be neither downgraded or elevated by the called workflow.


---

# File: question-002.md

---
question: "What are the different permission levels you can assign to `GITHUB_TOKEN` in the `permissions` block?"
title: "Question 002"
---


> https://docs.github.com/en/actions/using-jobs/assigning-permissions-to-jobs

1. [x] none, write, read
1. [ ] read, write, delete
1. [ ] read, write


---

# File: question-003.md

---
question: "You can use `permissions` to modify the `GITHUB_TOKEN` permissions on: (Select two.)"
title: "Question 003"
---


> https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/controlling-permissions-for-github_token
- [x] Workflow level
- [x] Job level
- [ ] Step level


---

# File: question-004.md

---
question: "Are GitHub Actions free for public repositories?"
title: "Question 004"
---

1. [x] Yes
1. [ ] No


---

# File: question-005.md

---
question: "Which of these is not a valid event that could trigger a workflow?"
title: "Question 005"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#about-events-that-trigger-workflows
1. [x] Cloning the repository
1. [ ] Committing a file to master branch
1. [ ] A branch is created
1. [ ] Adding a label to a pull request


---

# File: question-006.md

---
question: "Which is true about workflows? (Select three.)"
title: "Question 006"
---

> https://docs.github.com/en/actions/using-workflows/about-workflows
- [x] Workflows can run one or multiple jobs at a time
- [x] Workflows can be triggered manually, by an event or run on a schedule
- [x] Workflows have to be defined in the `.github/workflows` directory
- [ ] Workflows can only be run on a schedule
- [ ] Workflow can run only one job at a time
- [ ] Workflows are written in any of `.yaml`, `.json` or `.toml` formats
- [ ] Workflows can be shared in GitHub Marketplace
  > Actions (not workflows) can be shared in GitHub Marketplace


---

# File: question-007.md

---
question: "Which components are required for a workflow? (Select two.)"
title: "Question 007"
---

> https://docs.github.com/en/actions/using-workflows/about-workflows#workflow-basics
- [x] One or more events that will trigger the workflow
- [x] One or more jobs
- [ ] Workflow name
- [ ] Defined branches on which the workflow will run


---

# File: question-008.md

---
question: "Which event is triggered by a webhook action from outside of the repository?"
title: "Question 008"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows
1. [x] repository_dispatch
1. [ ] webhook_dispatch
1. [ ] workflow_dispatch
1. [ ] remote_dispatch
1. [ ] api_dispatch


---

# File: question-009.md

---
question: "Workflows are defined in which format"
title: "Question 009"
---

1. [x] yaml
1. [ ] toml
1. [ ] json
1. [ ] xml


---

# File: question-010.md

---
question: "Where should you store sensitive data such as passwords or certificates that will be used in workflows"
title: "Question 010"
---

1. [x] secrets
1. [ ] config variables
1. [ ] vault
1. [ ] environment variables


---

# File: question-011.md

---
question: "In a workflow with multiple jobs the default behavior is:"
title: "Question 011"
---

> https://docs.github.com/en/actions/using-workflows/about-workflows#creating-dependent-jobs
1. [x] All jobs run in parallel
1. [ ] Jobs run in sequence


---

# File: question-012.md

---
question: "If job B requires job A to be finished you have to:"
title: "Question 012"
---

> https://docs.github.com/en/actions/using-workflows/about-workflows#creating-dependent-jobs
1. [x] use the `needs` keyword in job B to create this dependency
1. [ ] use the `needs` keyword in job A to create this dependency
1. [ ] use the `requires` keyword in job B to create this dependency
1. [ ] use the `requires` keyword in job A to create this dependency


---

# File: question-013.md

---
question: "In a workflow with multiple jobs, if job A fails then:"
title: "Question 013"
---

> https://docs.github.com/en/actions/using-workflows/about-workflows#creating-dependent-jobs
1. [x] the jobs that are dependent on job A are skipped
1. [ ] the jobs that are dependent on job A fail
1. [ ] the workflow immediately cancels all other jobs


---

# File: question-014.md

---
question: "This code will launch 6 different jobs in parallel using the matrix strategy. Can you use the matrix strategy to parallelize entire workflows?"
title: "Question 014"
---


```yaml
jobs:
  example_matrix:
    strategy:
      matrix:
        version: [10, 12, 14]
        os: [ubuntu-latest, windows-latest]
```
> https://docs.github.com/en/actions/using-workflows/reusing-workflows#using-a-matrix-strategy-with-a-reusable-workflow

1. [ ] No
1. [x] Yes


---

# File: question-015.md

---
question: "Which matrix job definition is syntactically correct?"
title: "Question 015"
---


> https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#using-a-matrix-strategy

1. [x] 
```yaml
  jobs:
    example_matrix:
      strategy:
        matrix:
          version: [10, 12, 14]
          os: [ubuntu-latest, windows-latest]
```

1. [ ] 
```yaml
  jobs:
    example_matrix:
      matrix:
        strategy:
          version: [10, 12, 14]
          os: [ubuntu-latest, windows-latest]
```

1. [ ] 
```yaml
  jobs:
    example_matrix:
      matrix:
        version: [10, 12, 14]
        os: [ubuntu-latest, windows-latest]
```

1. [ ] 
```yaml
  jobs:
    matrix:
      version: [10, 12, 14]
      os: [ubuntu-latest, windows-latest]
```


---

# File: question-016.md

---
question: "How do you access matrix variables in a matrix strategy job?"
title: "Question 016"
---


> https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#using-a-matrix-strategy
1. [ ] Using the `vars` context
1. [x] Using the `matrix` context
1. [ ] Using the `job` context
1. [ ] Using the `jobs` context


---

# File: question-017.md

---
question: "When using the `pull_request` and `pull_request_target` events, how do you configure the workflow to run only when targeting the `prod` branch?"
title: "Question 017"
---

> https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#using-filters-to-target-specific-branches-for-pull-request-events
1. [x] Using `branches` filter
1. [ ] Using `branch` filter
1. [ ] You create the workflow only on `prod` branch
1. [ ] Using glob patterns


---

# File: question-018.md

---
question: "This workflow will run on all pull requests where:"
title: "Question 018"
---

```yaml
on:
  pull_request:
    branches:
      - 'release/**'
      - '!release/**-alpha'
```
> https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#example-including-and-excluding-branches
1. [x] the target branch name starts with `release` but does not end with `-alpha`
1. [ ] the target branch name starts with `release`
1. [ ] the source branch name starts with `release` but does not end with `-alpha`
1. [ ] the source branch name starts with `release`


---

# File: question-019.md

---
question: "Fill in the blank: When using `push` event trigger filters you can use <____> patterns to target multiple branches"
title: "Question 019"
---

> https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#using-filters-to-target-specific-branches-or-tags-for-push-events
1. [x] glob
1. [ ] regex
1. [ ] scheme
1. [ ] action


---

# File: question-020.md

---
question: "Which event allows you to manually trigger a workflow from the GitHub UI?"
title: "Question 020"
---

> https://docs.github.com/en/actions/using-workflows/manually-running-a-workflow
1. [x] workflow_dispatch
1. [ ] manual_dispatch
1. [ ] workflow_trigger
1. [ ] manual_trigger


---

# File: question-021.md

---
question: "What are the possible types of an input variable for a manually triggered workflow? (Select five.)"
title: "Question 021"
---

> https://docs.github.com/en/actions/writing-workflows/workflow-syntax-for-github-actions#onworkflow_dispatchinputsinput_idtype
- [x] choice
- [x] boolean
- [x] string
- [x] number
- [x] environment
- [ ] dropdown
- [ ] select


---

# File: question-022.md

---
question: "A workflow that has only `workflow_dispatch` event trigger can be triggered using GitHub's REST API"
title: "Question 022"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#onworkflow_dispatchinputs
1. [x] True
1. [ ] False


---

# File: question-023.md

---
question: "To stop a workflow from running temporarily without modifying the source code you should"
title: "Question 023"
---


> https://docs.github.com/en/actions/using-workflows/disabling-and-enabling-a-workflow
1. [x] Use the `Disable workflow` option in GitHub Actions
1. [ ] Remove secrets that are required for this workflow
1. [ ] Delete environment that is required for this workflow
1. [ ] Prevent any new commits to main branch


---

# File: question-024.md

---
question: "What are `activity types` of an event used for ?"
title: "Question 024"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#about-events-that-trigger-workflows
1. [x] Limiting workflow runs to specific activity types using the `types` filter
1. [ ] Checking if the activity comes from an user or a bot
1. [ ] Reacting to new activity on a repository (e.g new contributor)


---

# File: question-025.md

---
question: "You want to create a reusable workflow `CI` that runs some quality checks, linting and tests on code changes. What event trigger should the `CI` workflow define to allow reusing it in other workflows?"
title: "Question 025"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows
1. [x] workflow_call
1. [ ] workflow_trigger
> There is no such event trigger
1. [ ] workflow_dispatch
> This is used for manual triggers
1. [ ] workflow_run
> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#workflow_run


---

# File: question-026.md

---
question: "A reusable workflow named `build` creates zip file artifacts. How do you pass the zip file location to the caller workflow that is calling the `build` workflow? (Select three.)"
title: "Question 026"
---

> https://docs.github.com/en/actions/using-workflows/reusing-workflows#using-outputs-from-a-reusable-workflow

- [x] You define an output on workflow level in the `build` workflow
- [x] You define an output on job level in the `build` workflow
- [x] In the `build` workflow you write the output into `$GITHUB_OUTPUT` in one of the steps
- [ ] All outputs are automatically passed to the caller workflows


---

# File: question-027.md

---
question: "What are the valid use cases for using **defaults**? (Select two.)"
title: "Question 027"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#defaults

- [x] Using defaults.run on workflow level to set default shell (e.g bash) for an entire workflow
- [x] Using defaults.run on job level to set default working-directory for all steps in a single job
- [ ] Using defaults.run on step level to set default shell (e.g bash) for that single step
> defaults.run can only be set on workflow or job level
- [ ] Using defaults.env on workflow level to set default environment variables for an entire workflow
> There is no such thing as defaults.env
- [ ] Using defaults.env on job level to set default environment variables for all steps in a single job
> There is no such thing as defaults.env


---

# File: question-028.md

---
question: "How can you ensure that a workflow called `Deploy Prod` is always running at most one at a time?"
title: "Question 028"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#concurrency

1. [x] Use `concurrency` on workflow level
```yaml
concurrency: ${{ github.workflow }}
```
1. [ ] Use `queue` on workflow level
```yaml
queue: ${{ github.workflow }}
```
1. [ ] Use `order` on workflow level
```yaml
order: ${{ github.workflow }}
```
1. [ ] Use `parallel` on workflow level
```yaml
parallel: ${{ github.workflow }}
```


---

# File: question-029.md

---
question: "Your Pull Request analysis workflow uses multiple code analysis tools and takes about 20minutes to fully complete. It is triggered on `pull_request` event with `branches` filter set to `master`. Therefore if a developer pushes multiple commits within few minutes multiple workflows are running in parallel. How can you stop all previous workflow runs and only run the one with latest changes?"
title: "Question 029"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#example-using-concurrency-to-cancel-any-in-progress-job-or-run

1. [x] Use concurrency with cancel-in-progress
```yaml
  concurrency:
    group: ${{ github.workflow }}-${{ github.ref }}
    cancel-in-progress: true
```
1. [ ] Use concurrency
```yaml
  concurrency:
    group: ${{ github.ref }}
```
> This would queue runs on that github ref. It will not stop previous runs

1. [ ] Use activity types filter
```yaml
  on:
    pull_request:
      branches:
        - master
      types: [latest]
```
> There is no such activity type as `latest` for pull_request event
1. [ ] Use cancel-in-progress flag for `pull_request` event
```yaml
  on:
    pull_request:
      branches:
        - master
      cancel-in-progress: true
```


---

# File: question-030.md

---
question: "When will job3 run?"
title: "Question 030"
---

```yaml
  jobs:
    job1:
    job2:
      needs: job1
    job3:
      if: ${{ always() }}
      needs: [job1, job2]
```
> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#example-not-requiring-successful-dependent-jobs
1. [x] job3 will run after job1 and job2 have completed, regardless of whether they were successful
1. [ ] You cannot use `if: ${{ always() }}` and `needs` together. The workflow will fail on startup.
1. [ ] job3 will run after job1 and job2 have been successfully completed
1. [ ] job3 will run after both job1 and job2 have failed


---

# File: question-031.md

---
question: "What `jobs.job_id.if` conditional will make sure that job `production-deploy` is triggered only on `my-org/my-repo` repository? (Select two.)"
title: "Question 031"
---

```yaml
  jobs:
    production-deploy:  
      if: <CONDITION>
      runs-on: ubuntu-latest
      steps:
        ...
```
> https://docs.github.com/en/actions/learn-github-actions/contexts#github-context
- [x] `if: github.repository == 'my-org/my-repo'`
- [x] `if: ${{ github.repository == 'my-org/my-repo' }}`
- [ ] `if: ${{ github.organization == 'my-org' && github.repository == 'my-repo' }}`
> https://docs.github.com/en/actions/learn-github-actions/contexts#github-context
- [ ] `if: ${{ github.org == 'my-org' && github.repository == 'my-repo' }}`
> https://docs.github.com/en/actions/learn-github-actions/contexts#github-context


---

# File: question-032.md

---
question: "What GitHub-hosted runner types are available to use? (Select three.)"
title: "Question 032"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#choosing-github-hosted-runners
- [x] Windows
- [x] Ubuntu Linux
- [x] macOS
- [ ] Android


---

# File: question-033.md

---
question: "Is this statement true? `Not all steps run actions, but all actions run as a step`"
title: "Question 033"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idsteps
1. [x] True
1. [ ] False
> Steps can but don't have to run actions (e.g running a run command)


---

# File: question-034.md

---
question: "For any action published in GitHub Marketplace, you can often use it in multiple versions, which approach is the most stable and secure?"
title: "Question 034"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#example-using-versioned-actions

1. [x] Reference the commit SHA
1. [ ] Reference a version tag
1. [ ] Reference the main branch


---

# File: question-035.md

---
question: "To prevent a job from failure when one of the steps fails you can include:"
title: "Question 035"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepscontinue-on-error
1. [x] `continue-on-error` flag in the failing step
```yaml
  steps:
      - uses: my-org/failing-action@v1
        continue-on-error: true
```
1. [ ] `ignore-error` flag in the failing step
```yaml
  steps:
      - uses: my-org/failing-action@v1
        ignore-error: true
```
1. [ ] `failure()` conditional in the failing step
```yaml
  steps:
      - uses: my-org/failing-action@v1
        if: failure()
```
1. [ ] `always()` conditional in the failing step
```yaml
  steps:
      - uses: my-org/failing-action@v1
        if: always()
```


---

# File: question-036.md

---
question: "You defined a matrix job `example_matrix`. How can limit the matrix to run a maximum of 2 jobs at a time?"
title: "Question 036"
---


```yaml
  jobs:
    example_matrix:
      strategy:
        matrix:
          version: [10, 12, 14]
          os: [ubuntu-latest, windows-latest]
```
> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstrategymax-parallel
1. [x] Set `jobs.example_matrix.strategy.max-parallel` to 2
1. [ ] Set `jobs.example_matrix.strategy.concurrency` to 2
1. [ ] Use GitHub's REST API to check if the job count is lesser than 2
1. [ ] It's not possible, a matrix will always run all of the jobs in parallel if there are runners available


---

# File: question-037.md

---
question: "Which of these is a proper way of setting an output parameter `PET` with a value of `DOG` in a `step`."
title: "Question 037"
---


> https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#setting-an-output-parameter
1. [x] `echo "PET=DOG" >> "$GITHUB_OUTPUT"`
1. [ ] `echo "DOG=PET" >> "$GITHUB_OUTPUT"`
1. [ ] `gh set-output "DOG=PET"`
1. [ ] `gh set-output "PET=DOG"`


---

# File: question-038.md

---
question: "Which of these is a way of using `action_state` in `step_two`? "
title: "Question 038"
---

```yaml
  steps:
    - name: Set the value
      id: step_one
      run: |
        echo "action_state=yellow" >> "$GITHUB_ENV"
    - name: Use the value
      id: step_two
      run: ?
```
> https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#example-of-writing-an-environment-variable-to-github_env
1. [x] `run: echo "$action_state"`
1. [ ] `run: echo "${{ steps.step_one.outputs.action_state }}"`
> That would be the case if `action_state` was written to `$GITHUB_OUTPUT`
1. [ ] `run: echo "$steps.step_one.outputs.action_state"`
1. [ ] `run: echo "${{ action_state }}"`


---

# File: question-039.md

---
question: "Is this statement true? `Workflows can be reused, but a reusable workflow cannot call another reusable workflow.`"
title: "Question 039"
---


> https://docs.github.com/en/actions/using-workflows/reusing-workflows#nesting-reusable-workflows
1. [x] False
1. [ ] True
> Reusable workflows can be nested, but there are limitations https://docs.github.com/en/actions/using-workflows/reusing-workflows#limitations


---

# File: question-040.md

---
question: "In the following example, `workflow A` passes all of its secrets to `workflow B`, by using the inherit keyword. Then `workflow B` calls `workflow C`. Which statement regarding `secrets` is true for that example?"
title: "Question 040"
---


```yaml
  jobs:
    workflowA-calls-workflowB:
      uses: octo-org/example-repo/.github/workflows/B.yml@main
      secrets: inherit
```

```yaml
  jobs:
    workflowB-calls-workflowC:
      uses: different-org/example-repo/.github/workflows/C.yml@main
```
> https://docs.github.com/en/actions/using-workflows/reusing-workflows#passing-secrets-to-nested-workflows
1. [x] All secrets available to `workflow A` will be also available to `workflow B`, but not to `workflow C`
1. [ ] All secrets from `octo-org` organization and `octo-org/example-repo` repository will be available to `workflow B`, but not to `workflow C`
> Not all secrets from `octo-org` organization have to be made available to `octo-org/example-repo`.
1. [ ] All secrets available to `workflow A` will be also available to `workflow B` and `workflow C`
> `Workflow B` would need to add `secrets: inherit` when calling `workflow C`
1. [ ] Only repository and environment secrets available to `workflow A` will be available to `workflow B`, but not to `workflow C`. Organization scoped secrets cannot be inherited


---

# File: question-041.md

---
question: "When should you use `caching`?"
title: "Question 041"
---



> https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#comparing-artifacts-and-dependency-caching

1. [x] When you want to reuse files that don't change often between jobs or workflow runs, such as build dependencies from a package management system.
1. [ ] When you want to reuse files that do change often between jobs or workflow runs, such as build dependencies from a package management system.
1. [ ] When you want to save files produced by a job to view after a workflow run has ended, such as built binaries or build logs.
> Artifacts should be used for that https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts
1. [ ] When you want to save binaries produced by a build job to use in a subsequent deploy job to deploy a new version of an application
> Artifacts should be used for that https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts


---

# File: question-042.md

---
question: "When should you use `artifacts`? (Select two.)"
title: "Question 042"
---



> https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts#about-workflow-artifacts

- [x] Use artifacts to save files produced by a job to view after a workflow run has ended, such as test results or build logs.
- [x] Use artifacts to save binaries produced by a build job to use in a subsequent deploy job to deploy a new version of an application
- [ ] Use artifacts to reuse files that don't change often between jobs or workflow runs, such as build dependencies from a package management system.
> Caching should be used for that https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#comparing-artifacts-and-dependency-caching
- [ ] Use artifacts to create new versions of your application together with release notes, mentions and/or contributors
> That's a use case for releases, not artifacts


---

# File: question-043.md

---
question: "If a workflow runs on a `feature-a` branch, can it restore `caches` created in the default `main` branch?"
title: "Question 043"
---


> https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#restrictions-for-accessing-a-cache
1. [x] Yes, all branches can restore caches created on the default branch
1. [ ] Yes, all caches can be accessed by workflows on any branch within the same repository
1. [ ] No, caches can only be restored from the same branch
1. [ ] Yes but only if no files were changed on `feature-a` branch


---

# File: question-044.md

---
question: "To access an `artifact` that was created in another, previously triggered workflow run you can:"
title: "Question 044"
---


> https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts#about-workflow-artifacts
1. [x] You cannot access `artifacts` that were created in a different workflow run
1. [ ] Use the `actions/download-artifact` action.
1. [ ] Use the `actions/upload-artifact` action.
1. [ ] Use the `actions/download-artifact` action and make sure the artifact is not expired


---

# File: question-045.md

---
question: "What should you use to store coverage reports or screenshots generated during a workflow that runs automated testing for a repository?"
title: "Question 045"
---


> https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts#comparing-artifacts-and-dependency-caching
1. [x] Artifacts
1. [ ] Caches
1. [ ] Packages
> https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages
1. [ ] Releases
> https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases


---

# File: question-046.md

---
question: "You can only upload a single file at a time when using `actions/upload-artifact` action"
title: "Question 046"
---


> https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts#uploading-build-and-test-artifacts
1. [x] False
1. [ ] True


---

# File: question-047.md

---
question: "In job `deploy`, if you want to access binaries (containing your application) that were created in job `build` you should"
title: "Question 047"
---


> https://docs.github.com/en/actions/using-workflows/storing-workflow-data-as-artifacts#comparing-artifacts-and-dependency-caching

1. [x] upload the binaries as artifacts in `build` and download them in `deploy`
1. [ ] upload the binaries as artifacts in `deploy` and download them in `build`
1. [ ] cache the binaries in `build` and read the files from cache in `deploy`
1. [ ] cache the binaries in `deploy` and read the files from cache in `build`


---

# File: question-048.md

---
question: "A job called `job2` is using artifacts created in `job1`. Therefore it's important to make sure `job1` finishes before `job2` starts looking for the artifacts. How should you create that dependency?"
title: "Question 048"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idneeds

1. [x] create this dependency using the `needs` keyword in `job2`
1. [ ] this dependency is created implicitly when using `actions/download-artifact` to download artifact from `job1`
1. [ ] create this dependency by defining `job2` after `job1` in the workflow's `.yaml` definition
1. [ ] create this dependency using the `concurrency` keyword in `job2`


---

# File: question-049.md

---
question: "Which is true about `Starter Workflows` ? (Select three.)"
title: "Question 049"
---


> https://docs.github.com/en/actions/using-workflows/creating-starter-workflows-for-your-organization
- [x] They allow users to leverage ready-to-use (or requiring minimal changes) workflow templates
- [x] GitHub provides and maintains starter workflows for different categories, languages and tooling
- [x] Your organization can create custom starter workflows for users in your organization
- [ ] Starter workflows cannot call reusable workflows
- [ ] Starter workflows are a paid GitHub feature
- [ ] Starter workflows are provided ready-to-use and cannot be modified or enhanced
> https://docs.github.com/en/actions/using-workflows/using-starter-workflows#using-starter-workflows


---

# File: question-050.md

---
question: "Secrets and configuration variables can be scoped to: (Select three.)"
title: "Question 050"
---


> https://docs.github.com/en/actions/using-workflows/sharing-workflows-secrets-and-runners-with-your-organization#sharing-secrets-and-variables-within-an-organization
- [x] The entire organization, or selected repositories in an organization
- [x] A single repository
- [x] An environment in a repository
- [ ] An environment shared across multiple repositories
> Environments cannot be shared across repositories
- [ ] Multiple repositories that do not share an organization/enterprise
- [ ] A specific workflow in a repository
> Environment variables can be scoped to a workflow, configuration variables cannot
- [ ] A specific job in a workflow
> Environment variables can be scoped to a workflow, configuration variables cannot


---

# File: question-051.md

---
question: "What are the three types of Actions?"
title: "Question 051"
---

> https://docs.github.com/en/actions/creating-actions/about-custom-actions#types-of-actions
1. [x] `Docker container actions`, `JavaScript Actions`, `Composite Actions`
1. [ ] `Python Actions`, `JavaScript Actions`, `Custom Actions`
1. [ ] `Docker container Actions`, `JavaScript Actions`, `Custom Actions`
1. [ ] `Docker container actions`, `Java Actions`, `Composite Actions`


---

# File: question-052.md

---
question: "Is this statement true? `Docker container actions are usually slower than JavaScript actions`"
title: "Question 052"
---

> Docker container actions are slower than JavaScript actions
1. [x] True
1. [ ] False
> Because of the latency to build and retrieve the container, Docker container actions are slower than JavaScript actions.


---

# File: question-053.md

---
question: "When creating a custom GitHub Action you have to store the source code in `.github/workflows` directory"
title: "Question 053"
---

> https://docs.github.com/en/actions/creating-actions/about-custom-actions#choosing-a-location-for-your-action
1. [x] False
1. [ ] True
> That is true for `workflows`, not for `actions`


---

# File: question-054.md

---
question: "When creating custom GitHub Actions - in what file does all the action `metadata` have to be defined?"
title: "Question 054"
---


Metadata examples: name, description, outputs or required inputs
> https://docs.github.com/en/actions/creating-actions/metadata-syntax-for-github-actions
1. [x] In the `action.yml` or `action.yaml` file in the action repository
1. [ ] In the repository `README` file
> While it's good practice to do that, it's not a requirement for the action to work
1. [ ] It's edited in GitHub Marketplace UI when published for sharing
1. [ ] In the `action.yml` or `action.yaml` file in the action repository, but it is not required if the action is not meant to be shared and used by the public
> All actions require the metadata file.


---

# File: question-055.md

---
question: "A workflow was initially run on `commit A` and failed. You fixed the workflow with the subsequent `commit B`. When you re-run that workflow it will run with code from which commit?"
title: "Question 055"
---

> https://docs.github.com/en/actions/managing-workflow-runs/re-running-workflows-and-jobs#about-re-running-workflows-and-jobs
1. [x] It will run with code from `commit A`
1. [ ] It will run with code from `commit B`
> Re-running a workflow uses the same commit SHA and Git ref of the original event that triggered the workflow run.
1. [ ] You cannot re-run workflows in GitHub Actions. You have to trigger a new workflow which will run with latest changes
1. [ ] It will trigger two workflows, one with code from `commit A` and one with code from `commit B`


---

# File: question-056.md

---
question: "How can you require manual approvals by a maintainer if the workflow run is targeting the `production` environment?"
title: "Question 056"
---

> https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment
1. [x] Using deployment protection rules
1. [ ] Setting the required reviewers in the `production` workflow
1. [ ] Using branch protection rules
1. [ ] Manual approvals are not supported by GitHub Actions


---

# File: question-057.md

---
question: "Which is true about environments?"
title: "Question 057"
---

> Each job in a workflow can reference a single environment.
1. [x] Each job in a workflow can reference a single environment.
1. [ ] Each workflow can reference a single environment.
1. [ ] Each job in a workflow can reference a maximum of two environments.
1. [ ] Each workflow can reference a maximum of two environments.


---

# File: question-058.md

---
question: "When using GitHub Actions to access resources in one of the cloud providers (such as AWS, Azure or GCP) the safest and recommended way to authenticate is"
title: "Question 058"
---

> https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/about-security-hardening-with-openid-connect
1. [x] Using OIDC
1. [ ] Using Vault
1. [ ] Storing access keys in `secrets`
> Using long lasting access keys is not recommended in case of any security leaks or attacks such as [script injection](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions#understanding-the-risk-of-script-injections)
1. [ ] Storing access keys in `variables`
> No sensitive values should be stored in `variables`


---

# File: question-059.md

---
question: "Your open-source publicly available repository contains a workflow with a `pull_request` event trigger. How can you require approvals for workflow runs triggered from forks of your repository?"
title: "Question 059"
---

> https://docs.github.com/en/actions/managing-workflow-runs/approving-workflow-runs-from-public-forks#about-workflow-runs-from-public-forks
1. [x] Setup required approvals for fork runs in the repository
1. [ ] Setup deployment protection rules for the repository
> Deployment protection rules are used for protecting environments
1. [ ] Setup branch protection rules for the repository
1. [ ] The workflow will not trigger for forks if using `pull_request` event. If you want to do that you should use `fork_pull_request` event trigger with `require-approval` flag.


---

# File: question-060.md

---
question: "Which of the following default environment variables contains the name of the person or app that initiated the workflow run?"
title: "Question 060"
---


> https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables

1. [ ] `GITHUB_USER`
1. [ ] `GITHUB_REPOSITORY`
1. [ ] `GITHUB_WORKFLOW`
1. [x] `GITHUB_ACTOR`


---

# File: question-061.md

---
question: "Which of the following are default environment variables in GitHub Actions? (Select three.)"
title: "Question 061"
---


> https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables

- [x] `GITHUB_REPOSITORY`
- [x] `GITHUB_WORKFLOW`
- [x] `GITHUB_ACTOR`
- [ ] `GITHUB_USER`
- [ ] `GITHUB_ORGANIZATION`
- [ ] `GITHUB_TOKEN`


---

# File: question-062.md

---
question: "Your organization defines a secret `SomeSecret`, however when you reference that secret in a workflow using `${{ secrets.SomeSecret }}` it provides a different value than expected. What may be the reason for that?"
title: "Question 062"
---

> https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions#naming-your-secrets
1. [x] The secret `SomeSecret` is also declared in repository scope
1. [ ] The secret `SomeSecret` is also declared in enterprise scope
> If a secret with the same name exists at multiple levels, the secret at the lowest level takes precedence.
1. [ ] `${{ secrets.SomeSecret }}` expression is only used for repository scoped secrets
1. [ ] You need to use the GitHub API to access organization scoped secrets


---

# File: question-063.md

---
question: "Which is a correct way to print a debug message?"
title: "Question 063"
---

> https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#example-setting-a-debug-message
1. [x] `echo "::debug::Watch out here!"`
1. [ ] `echo ":debug:Watch out here!"`
1. [ ] `echo "::debug::message=Watch out here!"`
1. [ ] `echo "Watch out here!" >> $GITHUB_DEBUG`


---

# File: question-064.md

---
question: "How can organizations which are using GitHub Enterprise Server enable automatic syncing of third party GitHub Actions hosted on GitHub.com to their GitHub Enterprise Server instance?"
title: "Question 064"
---

> https://docs.github.com/en/enterprise-server@3.6/admin/github-actions/managing-access-to-actions-from-githubcom/enabling-automatic-access-to-githubcom-actions-using-github-connect
1. [x] Using GitHub Connect
1. [ ] GitHub Enterprise Server has access to all GitHub.com Actions by default
> GitHub Actions on GitHub Enterprise Server is designed to work in environments without full internet access. By default, workflows cannot use actions from GitHub.com and GitHub Marketplace.
1. [ ] Using actions-sync tool
> https://docs.github.com/en/enterprise-server@3.6/admin/github-actions/managing-access-to-actions-from-githubcom/manually-syncing-actions-from-githubcom#about-the-actions-sync-tool
1. [ ] GitHub Enterprise Server cannot use GitHub.com Actions because of it's on-premise nature and no internet access


---

# File: question-065.md

---
question: "Where can you find network connectivity logs for a GitHub self-hosted-runner?"
title: "Question 065"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/monitoring-and-troubleshooting-self-hosted-runners#checking-self-hosted-runner-network-connectivity
1. [x] In the `_diag` folder directly on the runner machine
1. [ ] On GitHub.com on that specific Runner's page
1. [ ] In the job run logs of a job that ran on that Runner
1. [ ] In the job run logs of a job that ran on that Runner with debug logging enabled


---

# File: question-066.md

---
question: "How can you validate that your GitHub self-hosted-runner can access all required GitHub services?"
title: "Question 066"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/monitoring-and-troubleshooting-self-hosted-runners#checking-self-hosted-runner-network-connectivity
1. [x] Using a GitHub provided script on the runner machine
1. [ ] By trying to access the runner machine by `ssh` to validate the network connectivity
1. [ ] By using the predefined GitHub Actions workflow `network-connectivity.yml`
1. [ ] GitHub will validate the network connectivity automatically when the runner application is installed on the runner machine


---

# File: question-067.md

---
question: "Which is the correct way of triggering a job only if configuration variable `MY_VAR` has the value of `MY_VALUE`?"
title: "Question 067"
---

> https://docs.github.com/en/actions/learn-github-actions/contexts#example-usage-of-the-vars-context
1. [x] By creating the following conditional on job level
```yaml
  my-job:
    if: ${{ vars.MY_VAR == 'MY_VALUE' }}
```
1. [ ] By creating the following conditional on job level
```yaml
  my-job:
    if: ${{ vars.MY_VAR }} == 'MY_VALUE'
```
> This will always be evaluate to True
1. [ ] It's not possible because configuration variables cannot be used in `if` conditionals
> That is true for `secrets` but not for configuration variables
1. [ ] It's not possible because configuration variables cannot be used in job level `if` conditionals
> That is true for `secrets` but not for configuration variables


---

# File: question-068.md

---
question: "To run a `step` only if the secret `MY_SECRET` has been set, you can:"
title: "Question 068"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#example-using-secrets
1. [x] Set the secret `MY_SECRET` as a job level environment variable, then reference that environment variable to conditionally run that step
```yaml
  my-job:
    runs-on: ubuntu-latest
    env:
      my_secret: ${{ secrets.MY_SECRET }}
    steps:
      - if: ${{ env.my_secret != '' }}
```
1. [ ] By creating the following conditional on job level
```yaml
  my-job:
    runs-on: ubuntu-latest
    if: ${{ secrets.MY_SECRET == '' }}
```
> secrets cannot be directly referenced in if: conditionals
1. [ ] By creating the following conditional on step level
```yaml
  my-job:
    runs-on: ubuntu-latest
    steps:
      - if: ${{ secrets.MY_SECRET == '' }}
```
> secrets cannot be directly referenced in if: conditionals
1. [ ] By creating the following conditional on step level
```yaml
  my-job:
    runs-on: ubuntu-latest
    steps:
      - if: ${{ secrets.MY_SECRET }}
```
> secrets cannot be directly referenced in if: conditionals


---

# File: question-069.md

---
question: "How can you use the GitHub API to download workflow run logs?"
title: "Question 069"
---

> https://docs.github.com/en/rest/actions/workflow-runs?apiVersion=2022-11-28#download-workflow-run-logs
1. [x] `GET /repos/{owner}/{repo}/actions/runs/{run_id}/logs`
1. [ ] `POST /repos/{owner}/{repo}/actions/runs/{run_id}/logs`
1. [ ] `HEAD /repos/{owner}/{repo}/actions/runs/{run_id}/logs`
1. [ ] `PUT /repos/{owner}/{repo}/actions/runs/{run_id}/logs`


---

# File: question-070.md

---
question: "How can you use the GitHub API to create or update a repository secret?"
title: "Question 070"
---

> https://docs.github.com/en/rest/actions/secrets?create-or-update-a-repository-secret=&apiVersion=2022-11-28#create-or-update-a-repository-secret
1. [x] `PUT /repos/{owner}/{repo}/actions/secrets/{secret_name}`
1. [ ] `POST /repos/{owner}/{repo}/actions/secrets/{secret_name}`
1. [ ] `HEAD /repos/{owner}/{repo}/actions/secrets/{secret_name}`
1. [ ] `GET /repos/{owner}/{repo}/actions/secrets/{secret_name}`


---

# File: question-071.md

---
question: "How can you override an organization-level GitHub Secret `API_KEY` with a different value when working within a repository? (Select two.)"
title: "Question 071"
---

> https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions#naming-your-secrets
- [x] By creating a repository secret with the same name `API_KEY`
- [x] By creating a environment secret with the same name `API_KEY`
- [ ] By creating a enterprise secret with the same name `API_KEY`
- [ ] By creating a enterprise secret with the name `OVERRIDE_API_KEY`
- [ ] By creating a repository secret with the name `OVERRIDE_API_KEY`
- [ ] By creating a environment secret with the name `OVERRIDE_API_KEY`
- [ ] By creating a repository secret with the name `REPOSITORY_API_KEY`
- [ ] By creating a environment secret with the name `ENVIRONMENT_API_KEY`


---

# File: question-072.md

---
question: "What components can be reused within a GitHub Organization? (Select four.)"
title: "Question 072"
---

- [x] Secrets
- [x] Configuration Variables
- [x] Self Hosted Runners
- [x] Workflow Templates
- [ ] Artifacts
> Artifacts are used to preserve data after a job has completed and/or share that data with another job within the same workflow. 
- [ ] Cache
> Cache can be reused across workflows within one repository
- [ ] Environment Variables
> Environment variables can be scoped to a step, job or a workflow. They cannot be shared across workflows/repositories or organizations


---

# File: question-073.md

---
question: "How many jobs will be executed in the following workflow?"
title: "Question 073"
---

```yaml
jobs:
  matrix-job:
    runs-on: ubuntu-latest
    strategy:
      matrix:
        pet: [cat, dog]
        color: [pink, brown]
        include:
          - color: white
            pet: dog
    steps:
      - run: echo "Hello ${{ matrix.color }} ${{ matrix.pet }}"
```
> https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#using-a-matrix-strategy
1. [x] 5
1. [ ] 4
1. [ ] 6
1. [ ] 7


---

# File: question-074.md

---
question: "Which of the following default environment variables contains the full name (e.g `octocat/hello-world`) of the repository where the workflow is running?"
title: "Question 074"
---


> https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables

1. [x] `GITHUB_REPOSITORY`
1. [ ] `GITHUB_REPOSITORY_ID`
1. [ ] `GITHUB_REPOSITORY_OWNER`
1. [ ] `GITHUB_REPOSITORY_OWNER_ID`


---

# File: question-075.md

---
question: "In a workflow that has multiple jobs, all running on GitHub-hosted runners, is it true that all jobs are guaranteed to run on the same runner machine?"
title: "Question 075"
---

> https://docs.github.com/en/actions/using-jobs/choosing-the-runner-for-a-job#choosing-github-hosted-runners
1. [x] No
1. [ ] Yes
> Each job runs in a fresh instance of a runner image specified by runs-on


---

# File: question-076.md

---
question: "What's the maximum amount of reusable workflows that can be called from a single workflow file? "
title: "Question 076"
---


> https://docs.github.com/en/actions/using-workflows/reusing-workflows#limitations
1. [x] 20
1. [ ] 5
1. [ ] 1
1. [ ] 10


---

# File: question-077.md

---
title: "Question 077"
question: "What is a self-hosted runner?"
---


> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/about-self-hosted-runners 
1. [x] A self-hosted runner is a system that you deploy and manage to execute jobs from GitHub Actions on GitHub.com
1. [ ] A self-hosted runner is a system to upload code to a private server
1. [ ] A self-hosted runner is a system to be able to create workloads automatically
1. [ ] A self-hosted runner is a system to manage pull requests from users of the organization


---

# File: question-078.md

---
title: "Question 078"
question: "Which of the following is a correct statement about GitHub Workflows and Actions?"
---


> https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions
1. [ ] Each action is composed of one or more workflows which is composed of one or more jobs, and each job is composed of one or more step
1. [ ] Each workflow is composed of one or more action which is composed of one or more jobs, and each job is composed of one or more step
1. [x] Each workflow is composed of one or more job which is composed of one or more step, and each step is an action or a script
1. [ ] Each action is composed of one or more job which is composed of one or more step, and each step is a workflow


---

# File: question-079.md

---
title: "Question 079"
question: "On which commit and branch do scheduled workflows run in GitHub Actions?"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#schedule

1. [ ] Scheduled workflows run on the specific commit on last modified branch.
   > incorrect, both specific commit and on last modified branch
1. [ ] Scheduled workflows run on the specific commit on the main branch.
   > incorrect, both specific commit and main branch
1. [x] Scheduled workflows run on the latest commit on the repository default branch.
1. [ ] Scheduled workflows run on the latest commit on the main branch.
   > latest commit is correct but the main branch is not


---

# File: question-080.md

---
title: "Question 080"
question: "What is the correct syntax for setting the directory for all `run` commands in a workflow?"
---

> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#defaultsrunworking-directory

1. [x] set `working-directory` under `defaults.run`
   ```yaml
    defaults:
        run:
            shell: bash
            working-directory: ./scripts
   ```
1. [ ] set `directory` under `defaults.run`
   ```yaml
    defaults:
        run:
            shell: bash
            directory: ./scripts
   ```
1. [ ] set `working-directory` under `job`
   ```yaml
    defaults:
        run:
            shell: bash
    job:
        working-directory: ./scripts
   ```
1. [ ] set `directory` under `job`
   ```yaml
    defaults:
        run:
            shell: bash
    job:
        directory: ./scripts
   ```


---

# File: question-081.md

---
title: "Question 081"
question: "How can you reuse a defined workflow in multiple repositories? (Choose two.)"
---


> https://docs.github.com/en/actions/using-workflows/creating-starter-workflows-for-your-organization
- [ ] By copying the workflow file to each repository
- [x] By using workflow templates
- [ ] By creating a reusable action
- [x] By defining the workflow in a central repository


---

# File: question-082.md

---
title: "Question 082"
question: "How can you ensure a job runs only on a specific branch?"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#using-filters
1. [x] By using the branches filter
1. [ ] By using the runs-on filter
1. [ ] By using the jobs filter
1. [ ] By using the branch keyword


---

# File: question-083.md

---
title: "Question 083"
question: "What does the `needs` keyword do in a GitHub Actions workflow?"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idneeds
1. [x] Specifies the dependencies of a job
1. [ ] Defines environment variables
1. [ ] Sets up the environment
1. [ ] Triggers a job based on an event


---

# File: question-084.md

---
title: "Question 084"
question: "Which keyword allows you to define environment variables in a GitHub Actions workflow?"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idenv
1. [x] env
1. [ ] vars
1. [ ] secrets
1. [ ] config


---

# File: question-085.md

---
title: "Question 085"
question: "What is the purpose of the `with` keyword in a GitHub Actions workflow?"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepswith
1. [ ] To define environment variables
1. [x] To specify input parameters for an action
1. [ ] To set up dependencies
1. [ ] To trigger another workflow


---

# File: question-086.md

---
title: "Question 086"
question: "Which of the following GitHub Actions syntax is used to run multiple commands in a single step?"
---


> https://docs.github.com/en/enterprise-cloud@latest/actions/using-workflows/workflow-commands-for-github-actions#example-of-a-multiline-string
1. [ ] Using && to chain commands
1. [ ] Defining commands in an array
1. [x] Using a multiline string with |
1. [ ] Separating commands with a semicolon ;


---

# File: question-087.md

---
title: "Question 087"
question: "How can you cache dependencies to speed up workflow execution?"
---


> https://docs.github.com/en/enterprise-cloud@latest/actions/using-workflows/caching-dependencies-to-speed-up-workflows#about-caching-workflow-dependencies
1. [ ] Using the cache keyword
1. [x] Using the actions/cache action
1. [ ] By storing them in the repository
1. [ ] By using the store keyword


---

# File: question-088.md

---
title: "Question 088"
question: "What does the `matrix` keyword do in a GitHub Actions workflow?"
---


> https://docs.github.com/en/enterprise-cloud@latest/actions/using-jobs/using-a-matrix-for-your-jobs
1. [x] Allows defining multiple job configurations to run in parallel
1. [ ] Sets environment variables for the job
1. [ ] Triggers workflows based on a schedule
1. [ ] Defines secrets for the workflow


---

# File: question-089.md

---
title: "Question 089"
question: "Which of the following can be used to limit the number of concurrent jobs running in a GitHub Actions workflow?"
---


> https://docs.github.com/en/enterprise-cloud@latest/actions/using-jobs/using-concurrency
1. [x] concurrency
1. [ ] limit
1. [ ] max-jobs
1. [ ] parallelism


---

# File: question-090.md

---
title: "Question 090"
question: "What is the default timeout for a GitHub Actions job?"
---


> https://docs.github.com/en/actions/learn-github-actions/usage-limits-billing-and-administration#usage-limits
1. [ ] 30 minutes
1. [ ] 60 minutes
1. [ ] 120 minutes
1. [x] 360 minutes


---

# File: question-091.md

---
title: "Question 091"
question: "How can you specify the operating system for a job in GitHub Actions?"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idruns-on
1. [ ] Using the os keyword
1. [x] Using the runs-on keyword
1. [ ] Using the platform keyword
1. [ ] Using the env keyword


---

# File: question-092.md

---
title: "Question 092"
question: "In a GitHub Actions workflow, how do you specify a specific version of Node.js to use in a job?"
---


> https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-nodejs#specifying-the-nodejs-version
1. [x] 
```yaml
  uses: actions/setup-node@v4
  with:
    node-version: 20
```
1. [ ] 
```yaml
  uses: actions/node-setup@v4
  with:
    node-version: 20
```
1. [ ] 
```yaml
  uses: setup-node@v4
  with:
    version: 20
```
1. [ ] 
```yaml
  uses: setup-node@v4
  with:
    node: 20
```


---

# File: question-093.md

---
title: "Question 093"
question: "How do you reference a secret stored in GitHub Secrets in a workflow?"
---


> https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions#using-secrets-in-a-workflow
1. [x] ${{ secrets.SECRET_NAME }}
1. [ ] ${{ secret.SECRET_NAME }}
1. [ ] ${{ env.SECRET_NAME }}
1. [ ] ${{ config.SECRET_NAME }}


---

# File: question-094.md

---
title: "Question 094"
question: "What is the default shell used by GitHub Actions on Windows runners?"
---


> https://github.blog/changelog/2019-10-17-github-actions-default-shell-on-windows-runners-is-changing-to-powershell/
1. [ ] bash
1. [ ] sh
1. [x] powershell
1. [ ] cmd


---

# File: question-095.md

---
title: "Question 095"
question: "Which of the following statements are true about adding a self-hosted runner in GitHub Actions? (Choose three.)"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/adding-self-hosted-runners#adding-a-self-hosted-runner-to-a-repository
- [x] You can add a self-hosted runner to a repository
- [x] You can add a self-hosted runner to an organization
- [x] You can add a self-hosted runner to an enterprise
- [ ] You can add a self-hosted runner to a workflow
> You can't add to workflow level
- [ ] You can add a self-hosted runner to a step
> You can't add to step level


---

# File: question-096.md

---
question: "Select the default environment variable that contains the operating system of the runner executing the job"
title: "Question 096"
---

> https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
1. [x] `RUNNER_OS`
1. [ ] `GITHUB_RUNNER_OS`
1. [ ] `RUNNER_ARCH`
1. [ ] `RUNNER_NAME`


---

# File: question-097.md

---
question: "How does the `actions/cache` action in GitHub Actions handle a cache miss?"
title: "Question 097"
---

> https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#managing-caches
1. [ ] by requiring manual intervention to create a new cache
1. [ ] by searching for a cache in other repositories
1. [x] by automatically creating a new cache if the job is completed successfully
1. [ ] by terminating the workflow if a cache miss occurs


---

# File: question-098.md

---
question: "How can you specify the schedule of a GitHub actions workflow to run on weekdays only?"
title: "Question 098"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#schedule
1. [ ] add a condition in the workflow YAML for weekdays
1. [ ] it is not possible in GitHub actions
1. [ ] use the on: schedule: weekdays event trigger
1. [x] use the on: schedule: cron event trigger


---

# File: question-099.md

---
question: "What is the recommended approach for storing secrets larger than 48 KB?"
title: "Question 099"
---

> https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions#limits-for-secrets
1. [ ] avoid storing large secrets entirely to ensure security
1. [ ] secrets larger than 48 KB cannot be stored
1. [x] encrypt and store secrets in the repository but keep the decryption passphrase as a secret
1. [ ] store large secrets directly as repository secrets to avoid limitations


---

# File: question-100.md

---
question: "Select status check functions in GitHub Actions"
title: "Question 100"
---

> https://docs.github.com/en/actions/learn-github-actions/expressions#status-check-functions
1. [x] `success()`, `always()`, `cancelled()` and `failure()`
1. [ ] `completed()`, `always()`, `cancelled()` and `failure()`
1. [ ] `status()`, `always()`, `cancelled()` and `failure()`
1. [ ] `state()`, `always()`, `cancelled()` and `failure()`


---

# File: question-101.md

---
question: "How do you ensure that `Upload Failure test report` step is executed only if `Run Tests` step fails?"
title: "Question 101"
---


> https://docs.github.com/en/actions/learn-github-actions/expressions#status-check-functions

1. [x] 
```yaml
    - name: Run Tests
      id: run-tests
      run: npm run test

    - name: Upload Failure test report
      if: failure() && steps.run-tests.outcome == 'failure'
      run: actions/upload-artifact@v3
      with:
        name: test-report
        path: test-reports.html
```

1. [ ] 
```yaml
    - name: Run Tests
      id: run-tests
      run: npm run test

    - name: Upload Failure test report
      if: always() && steps.run-tests.outcome == 'failure'
      run: actions/upload-artifact@v3
      with:
        name: test-report
        path: test-reports.html
```

1. [ ] 
```yaml
    - name: Run Tests
      id: run-tests
      run: npm run test

    - name: Upload Failure test report
      if: steps.run-tests.outcome == 'failure'
      run: actions/upload-artifact@v3
      with:
        name: test-report
        path: test-reports.html
```

1. [ ] 
```yaml
    - name: Run Tests
      id: run-tests
      run: npm run test

    - name: Upload Failure test report
      run: actions/upload-artifact@v3
      with:
        name: test-report
        path: test-reports.html
```


---

# File: question-102.md

---
question: "Which context holds information about the event that triggered a workflow run?"
title: "Question 102"
---

> https://docs.github.com/en/actions/using-workflows/triggering-a-workflow#using-event-information
1. [x] `github.event`
1. [ ] `github.repository`
1. [ ] `github.job`
1. [ ] `jobs.<job_id>.result`


---

# File: question-103.md

---
question: "In GitHub Actions, if you define both branches and paths filter, what is the effect on the workflow execution?"
title: "Question 103"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#onpull_requestpull_request_targetbranchesbranches-ignore
1. [x] the workflow will only run when both `branches` and `paths` are satisfied
1. [ ] the workflow will run when either `branches` or `paths` are satisfied, but will only apply the matching filter
1. [ ] the workflow will run when either `branches` or `paths` are satisfied
1. [ ] the workflow will not run when both `branches` and `paths` are satisfied


---

# File: question-104.md

---
question: "What is the recommended practice for treating environment variables in GitHub Actions, regardless of the operating system and shell used?"
title: "Question 104"
---


> https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/workflow-commands-for-github-actions#setting-an-environment-variable
1. [x] treat environment variables as case-sensitive
1. [ ] use only uppercase letters for environment variable names
1. [ ] ignore case sensitivity as GitHub Actions handles it automatically
1. [ ] depend on the behavior of the operating system in use


---

# File: question-105.md

---
question: "Which of the following statements accurately describes the behavior of workflow jobs referencing an environment's protection rules?"
title: "Question 105"
---


> https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment
1. [x] workflow jobs won't start until all the environment's protection rules pass
1. [ ] workflow jobs will never start if the environment has protection rules
1. [ ] workflow jobs will start immediately, regardless of the environment's protection rules
1. [ ] workflow jobs will only start if some of the environment's protection rules pass


---

# File: question-106.md

---
question: "What is the purpose of the `restore-keys` parameter in `actions/cache` in GitHub Actions?"
title: "Question 106"
---


> https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#managing-caches
1. [x] provide alternative keys to use in case of a cache miss
1. [ ] indicate whether a cache hit occurred
1. [ ] specify the location of the cached files
1. [ ] enable cross-OS cache functionality


---

# File: question-107.md

---
question: "Which variable would you set to `true` in order to enable step debug logging?"
title: "Question 107"
---

> https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/enabling-debug-logging
1. [x] `ACTIONS_STEP_DEBUG`
1. [ ] `ACTIONS_JOB_DEBUG`
1. [ ] `ACTIONS_RUNNER_DEBUG`
1. [ ] `ACTIONS_WORKFLOW_DEBUG`


---

# File: question-108.md

---
question: "Which configuration is appropriate for triggering a workflow to run on webhook events related to check_run actions?"
title: "Question 108"
---


> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#check_run

1. [x] 
```yaml
on:
    check_run:
        types: [rerequested, completed]
```

1. [ ] 
```yaml
on:
    check_run:
        types: [started]
```

1. [ ] 
```yaml
on:
    check_run:
        type: [closed]
```

1. [ ] 
```yaml
on:
    check_run:
        filter: [requested]
```


---

# File: question-109.md

---
question: "What is the purpose of the `timeout-minutes` keyword in a step?"
title: "Question 109"
---


> https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepstimeout-minutes
1. [x] it limits the execution time for individual step
1. [ ] it defines the time interval for individual commands within a step
1. [ ] it sets the timeout for waiting on external events before proceeding to the next step
1. [ ] it specifies the maximum duration a job is allowed to run


---

# File: question-110.md

---
question: "Dave is creating a templated workflow for his organization. Where must Dave store the workflow files and associated metadata files for the templated workflow?"
title: "Question 110"
---


> https://docs.github.com/en/actions/using-workflows/creating-starter-workflows-for-your-organization
1. [x] inside a directory named `workflow-templates` within a repository named `.github`
1. [ ] inside a directory named `workflow-templates` within the current repository
1. [ ] inside a directory named `.github/org-templates`
1. [ ] inside a directory named `.github/workflow-templates`


---

# File: question-111.md

---
question: "Dave wants to be notified when a comment is created on an issue within a GitHub repository. Which event trigger should be used within the workflow configuration?"
title: "Question 111"
---

> https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#issue_comment
1. [x] `issue_comment`
1. [ ] `issues.comment`
1. [ ] `issues`
1. [ ] `comment`


---

# File: question-112.md

---
question: "What level of access is required on a GitHub repository in order to delete log files from workflow runs?"
title: "Question 112"
---

> https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/using-workflow-run-logs
1. [x] write 
1. [ ] read
1. [ ] admin
1. [ ] owner


---

# File: question-113.md

---
question: "What is true about the following workflow configuration if triggered against the `octo/my-dev-repo` repository?"
title: "Question 113"
---

```yaml
name: deploy-workflow
on: [push]
jobs:
    production-deploy:
        if: github.repository == 'octo/my-prod-repo'
        runs-on: ubuntu-latest
        steps:
            - uses: actions/checkout@v4
            - uses: actions/setup-node@v4
              with:
                  node-version: '14'
            - run: npm install -g bats
```
> https://docs.github.com/en/actions/using-jobs/using-conditions-to-control-job-execution
1. [x] the `production-deploy` job will be marked as skipped
1. [ ] the `production-deploy` job will error
1. [ ] the `production-deploy` job will execute three steps
1. [ ] the `production-deploy` job will run if the `node-version` is `14`


---

# File: question-114.md

---
question: "How can you access the current values of variables in a matrix within a job in the example below:"
title: "Question 114"
---

```yaml
jobs:
    example_matrix:
        strategy:
            matrix:
                version: [10, 12, 14]
                os: [ubuntu-latest, windows-latest]
```
> https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#using-a-matrix-strategy
1. [x] reference variables through the `matrix` context with syntax like`matrix.version` and `matrix.os`
1. [ ] by using the `matrix.property` syntax
1. [ ] by using the `context` keyword within the job configuration
1. [ ] by accessing the variables directly with the syntax `version` and `os`


---

# File: question-115.md

---
question: "What level of permission is required to re-run the workflows"
title: "Question 115"
---

> https://docs.github.com/en/actions/managing-workflow-runs/re-running-workflows-and-jobs
1. [x] write 
1. [ ] read
1. [ ] admin
1. [ ] owner


---

# File: question-116.md

---
question: "When can you delete workflow runs? (select two)"
title: "Question 116"
---

> https://docs.github.com/en/actions/managing-workflow-runs/deleting-a-workflow-run
- [x] When workflow run has been completed
- [x] When workflow run is two weeks old
- [ ] When workflow run is 10 days old
- [ ] When workflow run is in progress


---

# File: question-117.md

---
question: "Who can bypass configured deployment protection rules to force deployment (by default)"
title: "Question 117"
---

> https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment#allow-administrators-to-bypass-configured-protection-rules
1. [x] Repository administrators
1. [ ] Anyone with repository write permission
1. [ ] Anyone with repository read permission


---

# File: question-118.md

---
question: "How can you skip the following workflow run when you commit or create a PR?"
title: "Question 118"
---

```yaml
name: Build
on: [push, pull_request]

jobs:
  build:
    runs-on: ubuntu-latest
    name: Extract artifact version
...
```

>https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs

1. [x] By including any one of the following keywords in the commit message or in the title of the pull-request
```yaml
[skip ci]
[ci skip]
[no ci]
[skip actions]
[actions skip]
```

1. [ ] Provide `SKIP_WORKFLOW` in the commit message
1. [ ] The above workflow will run in every event of push or pull request in every case


---

# File: question-119.md

---
title: "Question 119"
question: "How can you determine if an action is a container action by looking at its action.yml file?"
---


> https://docs.github.com/en/actions/creating-actions/metadata-syntax-for-github-actions#runs-for-docker-container-actions

1. [x] `runs.using` has `docker` as value
1. [ ] `runs.using` has `container` as value
1. [ ] `runs.using` has `Dockerfile` as value
1. [ ] `runs.main` has `container` as value


---

# File: question-120.md

---
title: "Question 120"
question: "What is the correct syntax for specifying a cleanup script in a container action?"
---


> https://docs.github.com/en/actions/creating-actions/metadata-syntax-for-github-actions#runspost-entrypoint

1. [x] 
```yaml
    runs:
      using: 'docker'
      image: 'Dockerfile'
      entrypoint: 'entrypoint.sh'
      post-entrypoint: 'cleanup.sh'
```

1. [ ] 
```yaml
    runs:
      using: 'docker'
      image: 'Dockerfile'
      entrypoint: 'entrypoint.sh'
      post: 'cleanup.sh'
```

1. [ ] 
```yaml
    runs:
      using: 'docker'
      image: 'Dockerfile'
      entrypoint: 'entrypoint.sh'
      after: 'cleanup.sh'
```

1. [ ] 
```yaml
    runs:
      using: 'docker'
      image: 'Dockerfile'
      entrypoint: 'entrypoint.sh'
      after-entrypoint: 'cleanup.sh'
```

1. [ ] 
```yaml
    runs:
      using: 'docker'
      image: 'Dockerfile'
      entrypoint: 'entrypoint.sh'
      cleanup: 'cleanup.sh'
```


---

# File: question-121.md

---
title: "Question 121"
question: "What’s true about default variables? (choose three)"
---


> https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
- [x] Default environment variables are set by GitHub and not defined in a workflow
- [x] Most of the default environment variables have a corresponding context property
- [x] Currently, the value of the default CI environment variable can be overwritten, but it's not guaranteed this will always be possible
- [ ] You can add a new default environment variable adding the prefix “GITHUB_” to it
- [ ] Default environment variables always have the prefix “GITHUB_”
- [ ] Default environment variables can be accessed using the env context


---

# File: question-122.md

---
title: "Question 122"
question: "What are the scopes defined for custom variables in a workflow? (choose three)"
---


> https://docs.github.com/en/actions/learn-github-actions/variables#defining-environment-variables-for-a-single-workflow
- [x] The entire workflow, by using `env` at the top level of the workflow file
- [x] The contents of a job within a workflow, by using `jobs.<job_id>.env`
- [x] A specific step within a job, by using `jobs.<job_id>.steps[*].env`
- [ ] All the jobs within a workflow, by using `jobs.env`
- [ ] The entire workflow, by using `custom.env` at the top level of the workflow file
- [ ] A specific environment in the repository, by using `environment.<environment_id>.env` at the top level of the workflow file


---

# File: question-123.md

---
question: "What must be added to `actions/checkout` if `my-org/my-private-repo` is a private repository differing from the one containing the current workflow?"
title: "Question 123"
---

```yaml
name: deploy-workflow
on: [push]
jobs:
    my-job:
        runs-on: ubuntu-latest
        steps:
          - name: "Checkout GitHub Action"
            uses: actions/checkout@v4
            with:
               repository: my-org/my-private-repo
               path: ./.github/actions/my-org/my-private-repo
```

> https://docs.github.com/en/actions/writing-workflows/workflow-syntax-for-github-actions#example-using-an-action-inside-a-different-private-repository-than-the-workflow

1. [x] Create a GitHub secret `MY_ACCESS_TOKEN`
```yaml
with:
    repository: my-org/my-private-repo
    path: ./.github/actions/my-org/my-private-repo
    token: ${{ secrets.MY_ACCESS_TOKEN }}
```

1. [ ] Create an input `MY_ACCESS_TOKEN`
```yaml
with:
    repository: my-org/my-private-repo
    path: ./.github/actions/my-org/my-private-repo
    token: ${{ MY_ACCESS_TOKEN }}
```

1. [ ] The environmental variable `GITHUB_TOKEN`
```yaml
with:
    repository: my-org/my-private-repo
    path: ./.github/actions/my-org/my-private-repo
    token: $GITHUB_TOKEN
```

1. [ ] Leave as is since access tokens will be passed automatically
```yaml
with:
    repository: my-org/my-private-repo
    path: ./.github/actions/my-org/my-private-repo
```


---

# File: question-124.md

---
question: "Given the following configuration, how many jobs will GitHub Actions run when this matrix is evaluated?"
title: "Question 124"
---

```yaml
strategy:
  matrix:
    os: [ubuntu-latest, windows-latest]
    node: [14, 16]
    include:
      - os: macos-latest
        node: 18
      - os: ubuntu-latest
        node: 14
```

> https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/running-variations-of-jobs-in-a-workflow#expanding-or-adding-matrix-configurations

1. [ ] 4 jobs
1. [x] 5 jobs
1. [ ] 6 jobs
1. [ ] 7 jobs
1. [ ] No jobs will run because the syntax is invalid.


---

# File: question-125.md

---
title: "Question 125"
question: "At what levels can environment variables be defined ? (Choose three)"
---


> https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/store-information-in-variables
- [x] Workflow level
- [x] Job level
- [x] Step level
- [ ] Action level


---

# File: question-126.md

---
title: "Question 126"
question: "How should a dependent job reference the `output1` value produced by a job named `job1` earlier in the same workflow?"
---

> https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/passing-information-between-jobs

1. [x] `${{needs.job1.outputs.output1}}`
1. [ ] `${{job1.outputs.output1}}`
1. [ ] `${{needs.job1.output1}}`
1. [ ] `${{depends.job1.output1}}`


---

