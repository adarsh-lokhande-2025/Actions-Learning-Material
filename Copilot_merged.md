# _index.md

---
title: "GitHub Copilot Questions"
hidden: true
cascade:
    exam: "GitHub Copilot"
    Description: "Mock exam questions for the GitHub Copilot Certification Exam."
---

### GitHub Copilot

{{< library-links questions="GitHub Copilot" >}}


---

# question-001.md

---
question: "Is GitHub Copilot free to use for everyone?"
title: "Question 001"
---

> https://github.com/features/copilot/plans
1. [ ] No
1. [X] Yes


---

# question-002.md

---
title: "Question 002"
question: "Which option below is NOT a possible way to grant access to Copilot for members of an organization?"
---

> Article Grant access to Copilot for members of an organization -https://docs.github.com/en/copilot/managing-copilot/managing-github-copilot-in-your-organization/managing-access-to-github-copilot-in-your-organization/granting-access-to-copilot-for-members-of-your-organization


1. [x] As a member of an Organization, you can enable Copilot directly from your account settings.
1. [ ] Via your Enterprise settings, enable GitHub Copilot for selected organizations or  all organizations.
1. [ ] Via your Organizations settings, enable GitHub Copilot for either selected teams or users or the entire organization.
1. [ ] You can use GitHub's REST API to grant access to GitHub Copilot for teams, or specific users, in your organization.


---

# question-003.md

---
title: "Question 003"
question: "What IDEs does GitHub Copilot support? (Choose two.)"
---

> https://docs.github.com/en/copilot/using-github-copilot/getting-code-suggestions-in-your-ide-with-github-copilot
- [x] Visual Studio Code, Xcode, Vim/NeoVim
- [x] Azure Data Studio, Visual Studio, IntelliJ IDEA
- [ ] Visual Studio, NetBeans, Eclipse
- [ ] Visual Studio, BlueJ, NetBeans


---

# question-004.md

---
title: "Question 004"
question: "What command is used to install the GitHub Copilot extension on the CLI?"
---


> https://docs.github.com/en/copilot/managing-copilot/configure-personal-settings/installing-github-copilot-in-the-cli
1. [x] gh extension install github/gh-copilot
1. [ ] gh copilot install
1. [ ] gh copilot setup
1. [ ] gh extension add copilot


---

# question-005.md

---
title: "Question 005"
question: "What are some of the principles of Prompt Engineering? (Choose three.)"
---


> https://docs.github.com/en/copilot/using-github-copilot/prompt-engineering-for-github-copilot
- [x] Focus on a single, well-defined task
- [x] Ensure instructions are detailed and explicit
- [x] Provide rich context for AI
- [ ] Write long, complex instructions
> If you want Copilot to complete a complex or large task, break the task into multiple simple, small tasks.


---

# question-006.md

---
title: "Question 006"
question: "How can you exclude specific files from GitHub Copilot?"
---


> https://docs.github.com/en/copilot/managing-copilot/configuring-and-auditing-content-exclusion/excluding-content-from-github-copilot
1. [ ] Editing the file .gitignore
> .gitignore is used to exclude the file from git, not copilot
1. [x] Browsing to the repository settings on GitHub and adding the paths to exclude
1. [ ] Configuring exclusions in the Copilot configuration file
1. [ ] Using a command in the terminal


---

# question-007.md

---
title: "Question 007"
question: "Which is true about Copilot's Content exclusions? (Choose two)"
---


> https://docs.github.com/en/copilot/managing-copilot/configuring-and-auditing-content-exclusion/excluding-content-from-github-copilot
- [x] Context exclusions can be configured at the repository and organization level
- [x] Copilot offers different plans with privacy considerations
- [ ] Copilot completely ignores excluded files
> Copilot may use information from an excluded file if the information is provided by the IDE.
- [ ] Content exclusions do not affect code completion
- [ ] Content exclusions are applied instantly
> After you add or change content exclusions, it can take up to 30 minutes to take effect


---

# question-008.md

---
title: "Question 008"
question: "Which of the following describes the GitHub Copilot Editor configuration file?"
---


> https://docs.github.com/en/copilot/customizing-copilot/adding-custom-instructions-for-github-copilot
1. [ ] A JSON file with security settings
1. [x] A Markdown file with natural language instructions for customizing Copilot Chat responses
1. [ ] A YAML file with build instructions
1. [ ] An XML file with deploy settings


---

# question-009.md

---
title: "Question 009"
question: "Which of the following describes how to use the GitHub Copilot's Productivity API?"
---


> https://docs.github.com/en/copilot/rolling-out-github-copilot-at-scale/analyzing-usage-over-time-with-the-copilot-metrics-api
1. [ ] To collect audit logs
1. [ ] To exclude specific files
1. [x] To collect usage metrics from organization members
1. [ ] To automatically update Copilot


---

# question-010.md

---
title: "Question 010"
question: "Which of the following integrates GitHub Copilot Chat with external tools?"
---


> https://docs.github.com/en/enterprise-cloud@latest/copilot/using-github-copilot/using-extensions-to-integrate-external-tools-with-copilot-chat
1. [x] GitHub Copilot Extensions
1. [ ] GitHub Copilot Marketplace
1. [ ] GitHub Copilot Integrations
1. [ ] GitHub Copilot Open


---

# question-011.md

---
title: "Question 011"
question: "How can you provide GitHub Copilot with context to generate tailored responses for your repository?"
---

> https://docs.github.com/en/enterprise-cloud@latest/copilot/customizing-copilot/adding-custom-instructions-for-github-copilot
1. [x] By creating a file named `.github/copilot-instructions.md` in the repository
1. [ ] By sending an email to GitHub support with your project details
1. [ ] By modifying the `.gitconfig` file to include custom instructions
> Modifying the `.gitconfig` file does not provide custom instructions to GitHub Copilot.
1. [ ] By creating a GitHub issue named `copilot-instructions` in the repository with the necessary context
> Creating a GitHub issue does not provide custom instructions to GitHub Copilot.


---

# question-012.md

---
title: "Question 012"
question: "Can GitHub Copilot use semantic information from a file that is ignored by GitHub Copilot content exclusions?"
---

> https://docs.github.com/en/copilot/managing-copilot/configuring-and-auditing-content-exclusion/excluding-content-from-github-copilot#limitations-of-content-exclusions
1. [x] Yes, if the information is provided by the IDE indirectly.
1. [ ] No, it will ignore all information from excluded files.
> It's possible that Copilot may use semantic information from an excluded file if the information is provided by the IDE indirectly. Examples of such content include type information and hover-over definitions for symbols used in code, as well as general project properties such as build configuration information.


---

# question-013.md

---
title: "Question 013"
question: "What happens when you exclude content from GitHub Copilot? (Choose two)"
---

> https://docs.github.com/en/copilot/managing-copilot/configuring-and-auditing-content-exclusion/excluding-content-from-github-copilot#about-content-exclusions-for-copilot
- [x] Code completion will not be available in the affected files.
- [x] The content in affected files will not inform code completion suggestions in other files.
- [ ] The content in affected files will continue to inform GitHub Copilot Chat's responses.
- [ ] Code completion will be unaffected in the affected files.


---

# question-014.md

---
title: "Question 014"
question: "What is the easiest way to get started with GitHub Copilot?"
---


> https://docs.github.com/en/copilot/using-github-copilot/getting-started-with-github-copilot
1. [ ] Request access from GitHub Support and wait for approval before using GitHub Copilot.
1. [ ] Use the Copilot website and paste your code when asking for suggestions.
1. [x] Install the Copilot extension in your preferred environment, such as Visual Studio Code.
1. [ ] Create a new public GitHub repo and enable Copilot to scan your code and make suggestions.


---

# question-015.md

---
title: "Question 015"
question: "What does GitHub Copilot analyze to offer relevant suggestions as you are developing new code?"
---


> https://docs.github.com/en/copilot/using-github-copilot/best-practices-for-using-github-copilot#guide-copilot-towards-helpful-outputs
1. [ ] Analyzes the context in all files within the repository.
1. [x] Analyzes the context in the current file and related files.
1. [ ] Analyzes only the context within the current file.
1. [ ] Analyzes only the context within the current line of code.


---

# question-016.md

---
title: "Question 016"
question: "Which of the following options best describes GitHub Copilot?"
---


> https://docs.github.com/en/copilot/about-github-copilot/what-is-github-copilot
1. [x] An AI coding assistant that helps developers by suggesting code and completing code snippets.
1. [ ] A version control system that tracks and manages changes in a codebase.
1. [ ] A code editor that provides debugging and error-checking features.
1. [ ] A tool that automatically tests and deploys code to production environments.


---

# question-017.md

---
title: "Question 017"
question: "How does GitHub Copilot handle data retention for code suggestions in the IDE?"
---

> https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/
1. [x] Suggestions are held temporarily in memory and discarded after use, not written to disk
1. [ ] All suggestions are permanently stored in a local database for future reference
1. [ ] Suggestions are automatically saved to GitHub repositories for version control
1. [ ] Code snippets are cached on disk for 30 days before being deleted


---

# question-018.md

---
title: "Question 018"
question: "Which steps occur when GitHub Copilot's proxy service processes a prompt?"
---

> https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/
1. [x] Tests for toxic language, relevance checks, and detection of prompt hacking attempts
1. [ ] Translation to multiple programming languages and syntax validation
1. [ ] Automatic code compilation and execution in a sandbox environment
1. [ ] Direct transmission to public repositories for reference checking


---

# question-019.md

---
title: "Question 019"
question: "Which set of principles correctly represents Microsoft's six key principles for Responsible AI that guide GitHub Copilot's development?"
---

> https://learn.microsoft.com/en-us/training/modules/responsible-ai-with-github-copilot/3-six-principles-of-responsible-ai
1. [x] Fairness, Reliability and Safety, Privacy and Security, Inclusiveness, Transparency, and Accountability
1. [ ] Efficiency, Speed, Accuracy, Innovation, Reliability, and Security
1. [ ] Privacy, Performance, Accessibility, Scalability, Maintainability, and Testing
1. [ ] Security, Development, Operations, Maintenance, Support, and Documentation


---

# question-020.md

---
title: "Question 020"
question: "Which of the following is a potential benefit of using GitHub Copilot to enhance developer workflows?"
---


> https://docs.github.com/en/copilot
1. [x] It can suggest code snippets to increase developer productivity.
1. [ ] It completely replaces the need for code review in every project.
1. [ ] It automatically merges pull requests without human approval.
1. [ ] It only works with software written in a single programming language.


---

# question-021.md

---
title: "Question 021"
question: "Which statement correctly describes GitHub Copilot's CLI command functionality?"
---

> https://docs.github.com/en/copilot/using-github-copilot/using-github-copilot-in-the-command-line
1. [x] Users can get command explanations using 'gh copilot explain' and command suggestions using 'gh copilot suggest'
1. [ ] Commands are automatically executed without user confirmation when using 'gh copilot suggest'
1. [ ] The 'gh copilot explain' command modifies system files without showing the explanation
1. [ ] Suggested commands are directly executed without being copied to the clipboard first


---

# question-022.md

---
title: "Question 022"
question: "What is the primary purpose of the '/tests' slash command in GitHub Copilot?"
---

> https://docs.github.com/en/copilot/using-github-copilot/guides-on-using-github-copilot/writing-tests-with-github-copilot
1. [x] It generates a suite of unit tests for the currently open file, using context from existing test files if available
1. [ ] It runs all existing unit tests in the project without generating new ones
1. [ ] It only validates the syntax of existing test files without creating new tests
1. [ ] It permanently removes all existing test files to start fresh


---

# question-023.md

---
title: "Question 023"
question: "How is seat usage calculated for GitHub Copilot at the enterprise level during a billing cycle?"
---

> https://docs.github.com/en/enterprise-cloud@latest/copilot/managing-copilot/managing-copilot-for-your-enterprise/managing-access-to-copilot-in-your-enterprise/viewing-copilot-license-usage-in-your-enterprise 
1. [x] Number of seats × (Days elapsed / Total days in billing cycle)
1. [ ] Total number of commits × Number of active developers
1. [ ] Number of code suggestions × Number of accepted completions
1. [ ] Total repository size × Number of organizations


---

# question-024.md

---
title: "Question 024"
question: "How does GitHub Copilot's matching public code feature work?"
---

> https://docs.github.com/en/copilot/using-github-copilot/finding-public-code-that-matches-github-copilot-suggestions 
1. [x] It searches for matches by comparing code suggestions against an index of public GitHub repositories, which is refreshed every few months
1. [ ] It performs real-time searches across all GitHub repositories, including private ones
1. [ ] It only matches code from repositories that were created in the last 24 hours
1. [ ] It checks code against external code hosting platforms outside of GitHub


---

# question-025.md

---
title: "Question 025"
question: "What are the post-processing checks performed on GitHub Copilot's responses?"
---

> https://resources.github.com/learn/pathways/copilot/essentials/how-github-copilot-handles-data/
1. [x] Toxic language, relevancy, code quality (including security vulnerabilities), unique identifiers, and optional public code matching
1. [ ] Only syntax validation and code formatting checks
1. [ ] Performance benchmarking and memory usage optimization
1. [ ] Just checking for compilation errors and runtime exceptions


---

# question-026.md

---
title: "Question 026"
question: "Which elements can GitHub Copilot use as context when generating suggestions?"
---

> https://docs.github.com/en/copilot/using-github-copilot/getting-started-with-github-copilot#using-context-in-github-copilot
1. [x] Content in the current file, neighboring files, repository URLs, file paths, and previous chat interactions
1. [ ] Only the current line of code being edited without any surrounding context
1. [ ] Exclusively external documentation from the internet
1. [ ] Just the project's README file and nothing else


---

