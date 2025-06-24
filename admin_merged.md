# _index.md

---
title: "GitHub Admin Questions"
hidden: true
cascade:
    exam: "GitHub Admin"
    Description: "Mock exam questions for the GitHub Admin Certification Exam."
---

### GitHub Admin

{{< library-links questions="GitHub Admin" >}}


---

# merged.md



---

# question-001.md

---
question: "As a GitHub Organization administrator, you want users to authenticate using a corporate identity provider. Which of the following is a way to achieve this?"
title: "Question 001"
---

> https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/about-authentication-with-saml-single-sign-on#about-authentication-with-saml-sso
1. [x] Setup SAML SSO
1. [ ] Corporate SSH Keys 
1. [ ] Setup OAuth SSO
1. [ ] Setup MFA


---

# question-002.md

---
title: "Question 002"
question: "What is the GitHub dependency graph?"
---


> https://docs.github.com/en/code-security/supply-chain-security/understanding-your-software-supply-chain/about-the-dependency-graph
1. [x] It is a representation of a repository's dependencies and dependents.
1. [ ] There is no such thing as the GitHub dependency graph.
1. [ ] It is a tool that automatically proposes version updates to dependencies in a repository.
1. [ ] It is a GitHub maintained list of known vulnerabilities in open source software packages.


---

# question-003.md

---
question: "Which is the minimum level of support that provides help with installing and using Advanced Security?"
title: "Question 003"
---

> https://docs.github.com/en/enterprise-server/support/learning-about-github-support/about-github-support#about-github-support
1. [x] GitHub Enterprise Support
1. [ ] GitHub Premium Support
1. [ ] GitHub Standard Support
1. [ ] GitHub Community Support


---

# question-004.md

---
question: "Which of the following issues can GitHub Support help resolve? (Choose four.)"
title: "Question 004"
---

> https://docs.github.com/en/enterprise-server/support/learning-about-github-support/about-github-support#scope-of-support
- [x] Installing and using GitHub Enterprise Server
- [x] Identifying and verifying the causes of suspected errors
- [x] Installing and using Advanced Security
- [x] Assistance with GitHub account and billing queries
- [ ] Technical advice on third-party integrations like Jira
- [ ] Help with external CI/CD tools such as Jenkins
- [ ] Guidance on writing/debugging new queries for CodeQL


---

# question-005.md

---
question: "Which of the following are correct methods to generate and share a diagnostic file for GitHub Enterprise Server? (Choose two.)"
title: "Question 005"
---

> https://docs.github.com/en/enterprise-server/support/contacting-github-support/providing-data-to-github-support#creating-and-sharing-diagnostic-files
- [x] Use the `ghe-diagnostics` command-line utility to retrieve the diagnostics for your instance.
- [x] Create a diagnostic file from the Management Console by navigating to the Support tab and clicking `Download diagnostics info`.
- [ ] Use the `ghe-support-bundle` command to create and upload the diagnostic file.
- [ ] Generate a diagnostic file using the GitHub mobile app.
- [ ] Run the `ghe-diagnostics -u` command to create and automatically upload the diagnostic file to GitHub Support.


---

# question-006.md

---
question: "Which of the following is the correct procedure for generating a support bundle in GitHub Enterprise Server? (Choose two.)"
title: "Question 006"
---

> https://docs.github.com/en/enterprise-server@3.15/support/contacting-github-support/providing-data-to-github-support#creating-and-sharing-support-bundles
- [x] Navigate to your GitHub Enterprise Server instance, select the `Site admin` page, then `Management Console`. Choose `Support` in the top navigation bar and click `Download support bundle`.
- [x] Generate and download a support bundle directly to your local machine via SSH using the `ghe-support-bundle -o > support-bundle.tgz` CLI command.
- [ ] First, access the `Settings` in your enterprise account, click on `License`, and under `GitHub Enterprise Help`, select `Upload a support bundle`. This will automatically generate and download the support bundle.
- [ ] Click your profile, then `Your enterprises`. In the enterprise account sidebar, select `Settings` and under `License`, click `Generate a support bundle`. This will create and download the bundle.


---

# question-007.md

---
question: "Which endpoints does the GitHub API provide to administer your enterprise? (Choose six.)"
title: "Question 007"
---

> https://docs.github.com/en/enterprise-cloud@latest/rest/enterprise-admin
- [x] Admin stats
- [x] Audit log
- [x] Billing
- [x] Code security and analysis
- [x] License
- [x] SCIM
- [ ] Marketplace
- [ ] Projects


---

# question-008.md

---
question: "What are the steps to install a GitHub App from GitHub Marketplace for an organization?"
title: "Question 008"
---

> https://docs.github.com/en/apps/using-github-apps/installing-a-github-app-from-github-marketplace-for-your-organizations
1. [x] Browse GitHub Marketplace, select the app, choose a plan, select the organization, and then review and install the app.
1. [ ] Contact GitHub support to manually install the app, then configure it via email instructions.
1. [ ] Download the app from an external site and manually upload it to your GitHub organization's repositories.
1. [ ] Install the app directly from the organization's dashboard without selecting any specific plan.


---

# question-009.md

---
question: "What are the benefits and risks of using apps and actions from the GitHub Marketplace?"
title: "Question 009"
---

1. [x] Benefits include automation of workflows and enhanced functionality; risks include potential security vulnerabilities and dependency on third-party services.
1. [ ] Benefits are limited to user interface improvements; risks include high costs and increased system complexity.
1. [ ] The only benefit is the ease of installation; risks involve complete access to codebase and data.
1. [ ] Benefits include official support from GitHub; risks include limited functionality and lack of customization options.


---

# question-010.md

---
question: "What are the key implications of enabling SAML single sign-on (SSO) for an organization in GitHub Enterprise Cloud?"
title: "Question 010"
---

> https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/about-authentication-with-saml-single-sign-on
1. [x] SAML SSO allows organization owners to control and secure access to organization resources.
1. [ ] SAML SSO restricts repository access to only those with a linked SAML identity.
1. [ ] Once SAML SSO is enabled, public repositories become inaccessible.
1. [ ] Enabling SAML SSO requires members to authenticate through GitHub, not the IdP.


---

# question-011.md

---
question: "What is a key difference between enabling SAML Single Sign-On (SSO) for all organizations in an enterprise account versus enabling it for a single organization in GitHub Enterprise Cloud?"
title: "Question 011"
---

> https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/about-authentication-with-saml-single-sign-on
1. [x] SAML SSO for a single organization allows for different IdPs for each organization, whereas enabling it for all organizations mandates a single IdP for the entire enterprise.
1. [ ] Enabling SAML SSO for all organizations requires separate authentication for each organization.
1. [ ] Enabling SAML SSO for all organizations limits repository access to internal collaborators only.
1. [ ] There is no difference in the implementation of SAML SSO between a single organization and all organizations in an enterprise account.


---

# question-012.md

---
question: "Which GitHub Support level provides SLA and written support in English 24/7?"
title: "Question 012"
---

> https://docs.github.com/en/enterprise-server/support/learning-about-github-support/about-github-support#about-github-support
1. [x] GitHub Premium Support
1. [ ] GitHub Enterprise Support
1. [ ] GitHub Standard Support
1. [ ] GitHub Community Support


---

# question-013.md

---
question: "What are the steps to enable and enforce SAML SSO for a single organization?"
title: "Question 013"
---

> https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-saml-single-sign-on-for-your-organization/enabling-and-testing-saml-single-sign-on-for-your-organization#enabling-and-testing-saml-single-sign-on-for-your-organization
1. [x] Navigate to `Your organizations`, choose `Settings`, click on `Authentication security`, select `Enable SAML authentication`, configure IdP settings, test SAML configuration, and enforce SAML SSO.
1. [ ] Go to `Organization Settings`, select `Security`, choose `SAML Authentication`, enter IdP information, perform a test of the SAML configuration, and enforce SAML SSO.
1. [ ] In the main menu, select `Organization`, then `Security Settings`, enable `SAML SSO`, fill in the IdP details, test the SSO configuration, and then enforce SAML SSO.
1. [ ] Access `Organization Settings`, click `Security`, enable `SAML SSO`, add IdP URL, test the configuration, and opt to enforce SAML SSO upon successful testing.


---

# question-014.md

---
question: "Which of the following identity providers (IdPs) is NOT officially supported and internally tested by GitHub Enterprise Cloud for SAML SSO?"
title: "Question 014"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/using-saml-for-enterprise-iam/configuring-saml-single-sign-on-for-your-enterprise#supported-identity-providers
1. [x] Google Identity Platform
1. [ ] Active Directory Federation Services (AD FS)
1. [ ] Microsoft Entra ID
1. [ ] Shibboleth


---

# question-015.md

---
question: "How do you require two-factor authentication (2FA) for an organization?"
title: "Question 015"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-two-factor-authentication-for-your-organization/requiring-two-factor-authentication-in-your-organization#requiring-two-factor-authentication-in-your-organization
1. [x] In the organization's settings, under `Security`, select `Authentication security`, and then choose `Require two-factor authentication for everyone in your organization`.
1. [ ] Go to the organization's page, click on `Members`, and individually set up 2FA for each member.
1. [ ] In your organization's settings, under `Billing`, select `Require two-factor authentication for billing managers only`.
1. [ ] Send an email to all organization members asking them to manually enable 2FA on their accounts.


---

# question-016.md

---
question: "Which identity providers (IdPs) support GitHub Enterprise Cloud SCIM API for organizations? (Choose three.)"
title: "Question 016"
---

> https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-saml-single-sign-on-for-your-organization/about-scim-for-organizations#supported-identity-providers
- [x] Microsoft Entra ID
- [x] Okta
- [x] OneLogin
- [ ] Amazon Cognito
- [ ] Google Identity Platform
- [ ] Auth0
- [ ] Keycloak


---

# question-017.md

---
question: "What is the primary function of Enterprise Managed Users in GitHub?"
title: "Question 017"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/understanding-iam-for-enterprises/about-enterprise-managed-users
1. [x] To centrally manage identity and access of enterprise members on GitHub from an identity provider (IdP).
1. [ ] To allow users to manage their own profile information and repository access independently.
1. [ ] To enable users to create public content and collaborate with other users on GitHub.
1. [ ] To provide a platform for individual developers to manage their private projects.


---

# question-018.md

---
question: "How are user accounts provisioned with Enterprise Managed Users?"
title: "Question 018"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/understanding-iam-for-enterprises/about-enterprise-managed-users
1. [x] User accounts are provisioned by the enterprise's IdP, with access provided to GitHub Enterprise Cloud.
1. [ ] User accounts are created manually by each user on GitHub.com.
1. [ ] User accounts are provisioned by GitHub without any input from the enterprise's IdP.
1. [ ] User accounts are automatically generated based on public email addresses.


---

# question-019.md

---
question: "What is required for a user to authenticate with an Enterprise Managed Users account?"
title: "Question 019"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/understanding-iam-for-enterprises/about-enterprise-managed-users#authenticating-with-a-managed-user-account
1. [x] Users must authenticate on the enterprise's IdP to access resources on GitHub.com.
1. [ ] Users authenticate through a public GitHub login page without any enterprise interference.
1. [ ] Authentication is bypassed for enterprise managed users for ease of access.
1. [ ] Users provide a special GitHub-managed authentication token.


---

# question-020.md

---
question: "Which statement is true regarding usernames and profile information for Enterprise Managed Users?"
title: "Question 020"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/understanding-iam-for-enterprises/about-enterprise-managed-users
1. [x] Usernames and profile information are set through the enterprise's IdP and cannot be changed by the users.
1. [ ] Users can change their usernames and profile information at any time on GitHub.
1. [ ] Usernames and profile information are set by the users themselves during the GitHub account setup.
1. [ ] GitHub automatically assigns random usernames and profile information for enhanced security.


---

# question-021.md

---
question: "What are the implications of a managed user needing to contribute to resources outside of the enterprise?"
title: "Question 021"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/understanding-iam-for-enterprises/about-enterprise-managed-users#supporting-developers-with-multiple-user-accounts-on-githubcom
1. [x] Managed users are not allowed to contribute to public resources, and they need a separate personal account for this purpose.
1. [ ] Managed users can freely contribute to public resources and external enterprises without restrictions.
1. [ ] Managed users must request special permission from GitHub to contribute to external resources.
1. [ ] Contributions to external resources are automatically managed by the enterprise's IdP.


---

# question-022.md

---
question: "What is SCIM in the context of GitHub?"
title: "Question 022"
---

> https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-saml-single-sign-on-for-your-organization/about-scim-for-organizations
1. [x] SCIM, or System for Cross-domain Identity Management, is a protocol designed to automate identity provisioning and management. In GitHub, SCIM integrates with external Identity Providers (IdPs) to manage GitHub Enterprise Cloud organization memberships, using a base URL for SCIM endpoints to perform operations like listing, inviting, and updating user identities.
1. [ ] SCIM is a user management system exclusive to GitHub, allowing users to customize their profiles and repositories. In GitHub, SCIM works by providing a platform-specific interface for these customizations.
1. [ ] SCIM stands for System for Cross-domain Identity Management. It's a protocol that GitHub uses to manage internal database systems, focusing mainly on securing data and user information without integrating with any external systems.
1. [ ] SCIM is a GitHub-specific tool used for enhancing the network performance of GitHub servers. It works by managing internet bandwidth and traffic within the GitHub ecosystem, ensuring optimal performance for all users.


---

# question-023.md

---
question: "What's the purpose of SCIM and team synchronization in GitHub?"
title: "Question 023"
---

> https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-saml-single-sign-on-for-your-organization/managing-team-synchronization-for-your-organization
1. [x] Team synchronization connects GitHub teams with IdP groups for membership management, relying on SAML single sign-on, whereas SCIM automates identity provisioning and management across systems, including creating and updating user identities and access.
1. [ ] Team synchronization is an automated process that allows users to manage their public profiles and repositories through a GitHub-specific interface.
1. [ ] Team synchronization is used for internal data security and user information management, while SCIM is an interface for user profile and repository customization.
1. [ ] Both team synchronization and SCIM in GitHub are used for user provisioning services, inviting non-members to join organizations and managing public profiles and repositories.


---

# question-024.md

---
question: "What are valid authentication methods available in GitHub? (choose six.)"
title: "Question 024"
---

> https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github
- [x] Username and password (with optional 2FA)
- [x] Personal access token (PAT)
- [x] SSH KEY
- [x] SAML SSO for enterprise accounts
- [x] Passkey authentication (opt-in beta for passwordless login)
- [x] OAuth tokens for third-party app integrations
- [ ] QR code system linked to a mobile device
- [ ] Authentication via social media accounts like Facebook or Google


---

# question-025.md

---
question: "How does GitHub Enterprise Cloud differ from GitHub Enterprise Server?"
title: "Question 025"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-for-enterprises#about-deployment-options
1. [x] GitHub Enterprise Cloud is hosted by GitHub, while GitHub Enterprise Server is hosted on your own servers
1. [ ] GitHub Enterprise Cloud is hosted on your servers, while GitHub Enterprise Server is hosted by GitHub
1. [ ] GitHub Enterprise Cloud offers only public repositories, while GitHub Enterprise Server offers private repositories
1. [ ] GitHub Enterprise Cloud is designed for individual use, while GitHub Enterprise Server is for organizations


---

# question-026.md

---
question: "Which of the following are extra features provided by GitHub Enterprise Cloud over GitHub Free plan? (choose four.)"
title: "Question 026"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-enterprise-cloud
- [x] SAML authentication
- [x] Additional GitHub Actions minutes
- [x] Privately published GitHub Pages sites
- [x] Ability to restrict email notifications to verified domains
- [ ] Free public repositories for all users
- [ ] Unlimited private repositories for individual users
- [ ] Automatic code review for every push


---

# question-027.md

---
question: "What is the purpose of enterprise accounts in GitHub Enterprise Cloud?"
title: "Question 027"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-enterprise-cloud
1. [x] To provide administrators with a single point of visibility and management across multiple organizations
1. [ ] To provide individual users with unlimited private repositories
1. [ ] To offer free access to GitHub Enterprise Server
1. [ ] To allow users to manage their public and private contributions separately


---

# question-028.md

---
question: "Which of the following is a management option exclusive to GitHub Enterprise Cloud?"
title: "Question 028"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-enterprise-cloud
1. [x] Using Enterprise Managed Users to create and manage user accounts through your IdP
1. [ ] Allowing users to create and manage their own personal accounts without restrictions
1. [ ] Forcing all users to adopt a uniform coding standard
1. [ ] Requiring all code to be reviewed by GitHub before being published


---

# question-029.md

---
question: "Which is the main restriction of Enterprise Managed User accounts in GitHub Enterprise Cloud?"
title: "Question 029"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-enterprise-cloud
1. [x] They cannot interact with public repositories outside their enterprise.
1. [ ] They are restricted to a single organization within the GitHub Enterprise account.
1. [ ] They require administrator approval to create or join organizations outside the enterprise.
1. [ ] Access to third-party integrations is limited and must be approved by an enterprise administrator.


---

# question-030.md

---
question: "What is GitHub Enterprise Server primarily designed for?"
title: "Question 030"
---

> https://docs.github.com/en/enterprise-server@latest/admin/overview/about-github-enterprise-server
1. [x] A self-hosted platform for software development within your enterprise
1. [ ] A cloud-based software development platform for open-source projects
1. [ ] A platform for individual developers to host personal projects
1. [ ] A service for deploying and managing containerized applications


---

# question-031.md

---
question: "Which environments can GitHub Enterprise Server be deployed to?"
title: "Question 031"
---

> https://docs.github.com/en/enterprise-server@latest/admin/overview/about-github-enterprise-server
1. [x] On-premises data center or to a public cloud service (e.g., AWS, GCP, Azure)
1. [ ] Exclusively to private cloud environments
1. [ ] Only on GitHub-managed servers
1. [ ] Directly onto personal computing devices


---

# question-032.md

---
question: "Which of the following is a key feature of GitHub Enterprise Server?"
title: "Question 032"
---

> https://docs.github.com/en/enterprise-server@latest/admin/overview/about-github-enterprise-server
1. [x] Runs on your infrastructure and governed by access and security controls you define
1. [ ] Unlimited public and private repositories on GitHub.com
1. [ ] Free access to GitHub Actions and GitHub Packages
1. [ ] Automatic deployment to any cloud service provider


---

# question-033.md

---
question: "How can GitHub Enterprise Server's administration be handled?"
title: "Question 033"
---

> https://docs.github.com/en/enterprise-server@latest/admin/overview/about-github-enterprise-server
1. [x] Via browser, administrative SSH access, and REST or GraphQL APIs
1. [ ] Only through direct access to the server's console
1. [ ] Via GitHub.com's web interface exclusively
1. [ ] Through third-party management tools only


---

# question-034.md

---
question: "What does GitHub recommend for safeguarding against data loss in GitHub Enterprise Server?"
title: "Question 034"
---

> https://docs.github.com/en/enterprise-server@latest/admin/overview/about-github-enterprise-server
1. [x] Establishing a plan for disaster recovery and configuring backups
1. [ ] Using third-party cloud storage services for backup
1. [ ] Relying on GitHub's automatic cloud backup services
1. [ ] Manual backup by exporting data to local storage periodically


---

# question-035.md

---
question: "What's the usage cost of GitHub Actions for public repositories?"
title: "Question 035"
---

> https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions
1. [x] GitHub Actions usage is free for public repositories.
1. [ ] GitHub Actions incurs a charge for every minute used in public repositories.
1. [ ] Public repositories are given half the amount of free minutes compared to private repositories.
1. [ ] GitHub Actions is not available for public repositories.


---

# question-036.md

---
question: "How are minutes calculated for jobs that run on different operating systems in GitHub Actions?"
title: "Question 036"
---

> https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions
1. [x] Jobs on Windows and macOS consume minutes at 2 and 10 times the rate of jobs on Linux runners.
1. [ ] All jobs, regardless of the operating system, consume minutes at the same rate.
1. [ ] Jobs on Linux consume minutes at 2 and 10 times the rate of jobs on Windows and macOS runners.
1. [ ] Only jobs on macOS consume minutes at a different rate, 5 times that of Linux and Windows.


---

# question-037.md

---
question: "What is the default spending limit for GitHub Actions on monthly-billed accounts?"
title: "Question 037"
---

> https://docs.github.com/en/billing/managing-billing-for-github-actions/about-billing-for-github-actions
1. [x] The default spending limit is 0$, preventing additional usage beyond the included amounts.
1. [ ] The default spending limit is 50$, allowing some overage beyond the included amounts.
1. [ ] There is no default spending limit, and users are billed for any usage beyond the free tier.
1. [ ] The default spending limit varies based on the account's historical usage.


---

# question-038.md

---
question: "How can an organization owner find statistics on license usage for their GitHub Enterprise Server?"
title: "Question 038"
---

> https://docs.github.com/en/enterprise-server/billing/managing-your-license-for-github-enterprise/viewing-license-usage-for-github-enterprise
1. [x] By navigating to the `Site admin` dashboard to view the license usage under `Enterprise account` settings.
1. [ ] Through direct email requests to GitHub Support.
1. [ ] Checking the organization's public profile page for real-time stats.
1. [ ] Using the GitHub API to fetch real-time license usage data for GitHub Enterprise Server.


---

# question-039.md

---
question: "How can an organization admin set default permissions for new members in a GitHub organization?"
title: "Question 039"
---

> https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/setting-base-permissions-for-an-organization#setting-base-permissions
1. [x] In the `Access` section of the organization's settings, select `Member privileges`, then under `Base permissions`, choose a permissions level and confirm the change.
1. [ ] Default permissions are automatically determined by GitHub based on the organization's activity and cannot be manually set.
1. [ ] By individually setting permissions for each new member as they are added to the organization, with no default level available.
1. [ ] Default permissions for new members are set through a GitHub API call specifying the desired base permission level for the organization.


---

# question-040.md

---
question: "How does team synchronization with Microsoft Entra ID (previously Azure AD) benefit GitHub Enterprise Cloud organizations?"
title: "Question 040"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/identity-and-access-management/using-saml-for-enterprise-iam/managing-team-synchronization-for-organizations-in-your-enterprise
1. [x] It allows for automatic reflection of membership changes in the IdP group on GitHub, reducing the need for manual updates and custom scripts by synchronizing teams in GitHub organizations with IdP groups.
1. [ ] It enables GitHub to serve as an identity provider for Microsoft Entra ID, streamlining user authentication processes.
1. [ ] It automatically converts Microsoft Entra ID group memberships into corresponding GitHub repositories, facilitating resource allocation.
1. [ ] It backs up GitHub organization data to Microsoft Entra ID servers, providing an additional layer of data redundancy.


---

# question-041.md

---
question: "What is the primary purpose of a GitHub organization?"
title: "Question 041"
---

> https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations#about-organizations
1. [x] To allow businesses and open-source projects to collaborate across many projects at once with advanced security and administrative features.
1. [ ] To provide individual users with personal space to host their private projects.
1. [ ] To serve as a backup service for code repositories.
1. [ ] To offer a platform for personal blogging and website hosting.


---

# question-042.md

---
question: "Which role in a GitHub organization has the authority to manage access to the organization's resources?"
title: "Question 042"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] Organization owner
1. [ ] Team member
1. [ ] Outside collaborator
1. [ ] Repository contributor


---

# question-043.md

---
question: "How can access management and collaboration be simplified within a GitHub organization?"
title: "Question 043"
---

> https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations#about-organizations
1. [x] By creating nested teams that reflect the group's structure, with cascading access permissions and mentions.
1. [ ] Through the use of single sign-on (SSO) for all members exclusively.
1. [ ] By granting all members owner-level permissions.
1. [ ] Limiting repository creation to organization owners only.


---

# question-044.md

---
question: "Which GitHub plan allows to use secret scanning in private repositories?"
title: "Question 044"
---

1. [x] Any GitHub Enterprise plan with a GHAS license
1. [ ] GitHub Enterprise Cloud
1. [ ] GitHub Enterprise Server
1. [ ] GitHub Pro
1. [ ] GitHub Team


---

# question-045.md

---
question: "What is the advantage of having an enterprise account on GitHub Enterprise Cloud for an organization?"
title: "Question 045"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/overview/about-github-for-enterprises#about-github-for-enterprises
1. [x] It allows owners to centrally manage policy and billing for multiple organizations.
1. [ ] It provides unlimited private repositories for individual users.
1. [ ] It offers a free domain for hosting the organization's website.
1. [ ] It automatically enrolls the organization in a premium support plan.


---

# question-046.md

---
question: "How can an organization enhance the security of their GitHub Actions workflows?"
title: "Question 046"
---

> https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions
1. [x] By adopting security practices like secure handling of secrets and regularly reviewing audit logs for anomalies.
1. [ ] By requiring all members to use biometric authentication for accessing GitHub.
1. [ ] By making all repositories within the organization public to ensure transparency.
1. [ ] By disabling the creation and processing of issues and pull requests to reduce attack surfaces.


---

# question-047.md

---
question: "Which of the following are recognized roles within a GitHub organization?"
title: "Question 047"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization#about-organization-roles
1. [x] Organization owners, Organization members, Organization moderators, Billing managers, Security managers, GitHub App managers, Outside collaborators
1. [ ] Project managers, Contributors, Observers, External consultants
1. [ ] System administrators, Database managers, IT support, External auditors
1. [ ] Lead developers, Junior developers, Senior developers, Project owners


---

# question-048.md

---
question: "Which role in a GitHub organization has the highest level of access?"
title: "Question 048"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] Owner
1. [ ] Member
1. [ ] Billing manager
1. [ ] Outside collaborator


---

# question-049.md

---
question: "What are the default permissions of a member in a GitHub organization?"
title: "Question 049"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] Members can create private repositories (subject to the organization's policy) and participate in projects within the organization to which they are granted access.
1. [ ] They have the ability to delete the organization.
1. [ ] They can manage billing information.
1. [ ] Members cannot interact with the organization's repositories until promoted to owner.


---

# question-050.md

---
question: "What is the primary responsibility of a billing manager in a GitHub organization?"
title: "Question 050"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] Managing billing settings for the organization, including updating payment methods and reviewing invoices.
1. [ ] They can manage team permissions and repository settings.
1. [ ] Creating and deleting all repositories within the organization.
1. [ ] Assigning and removing organization owners.


---

# question-051.md

---
question: "How does the role of an outside collaborator differ from that of a member within a GitHub organization?"
title: "Question 051"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] Outside collaborators are assigned access on a repository-by-repository basis, while members may have broader permissions within the organization depending on their role.
1. [ ] Outside collaborators have the capability to modify organization settings.
1. [ ] There is no distinction in access levels between outside collaborators and members.
1. [ ] Outside collaborators can add or remove members from the organization.


---

# question-052.md

---
question: "How can an organization owner change the role of a member within the organization?"
title: "Question 052"
---

> https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization
1. [x] By navigating to the organization's settings, selecting `Members`,and then adjusting the member's role from the list.
1. [ ] Members can change their own roles within the organization settings.
1. [ ] By deleting and re-inviting the member with the desired role.
1. [ ] Role changes within an organization are not possible; a new organization must be created.


---

# question-053.md

---
question: "How can you give a user the minimum required permissions necessary for accessing a specific repository within a GitHub organization?"
title: "Question 053"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Add the user as an outside collaborator to the repository with `Read` access, granting them the ability to clone the repository without allowing them to push changes.
1. [ ] Automatically grant them 'Owner' access to ensure they can manage organization settings and repository access.
1. [ ] Provide them with 'Write' access to all repositories in the organization to ensure they can contribute to projects.
1. [ ] It's not possible to grant users access to specific repositories; they must be given access to the entire organization.


---

# question-054.md

---
question: "What are the key features and functionalities of teams within a GitHub organization?"
title: "Question 054"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Teams in GitHub organizations enable managing access and notifications for groups reflecting the company's structure, with capabilities for admin, read, or write access to repositories, mentioning for notifications, and the use of nested teams for hierarchical management.
1. [ ] Teams are solely for social networking within GitHub, allowing members of an organization to communicate and share updates without any impact on repository access or organizational notifications.
1. [ ] GitHub teams are identical to organization members, with no distinct features or functionalities, such as access management or notifications.
1. [ ] Teams within GitHub can include outside collaborators and are mainly used for external communication, without any internal organizational structure or repository access permissions.


---

# question-055.md

---
question: "What distinguishes a visible team from a secret team in a GitHub organization?"
title: "Question 055"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Visible teams can be viewed and mentioned by any organization member, whereas secret teams are only visible to team members and organization owners, enhancing privacy for sensitive collaborations.
1. [ ] Visible teams have access to all repositories by default, while secret teams do not have any repository access until explicitly granted.
1. [ ] Secret teams can manage organization settings, unlike visible teams which can only manage repository settings.
1. [ ] There is no functional difference; the terms simply reflect the team's preference for communication.


---

# question-056.md

---
question: "How do nested teams benefit an organization's structure within GitHub?"
title: "Question 056"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Nested teams reflect the organization's hierarchy, inheriting access permissions from parent teams and streamlining permission management and communication across multiple levels of the organization.
1. [ ] Nested teams complicate the organization's structure and should be avoided to simplify team management.
1. [ ] Child teams can override the access permissions of their parent teams, providing flexibility in access control.
1. [ ] Members of nested teams have restricted access to communicate with members of their parent teams, enhancing security.


---

# question-057.md

---
question: "What can be found on a team’s page within a GitHub organization?"
title: "Question 057"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Team members, child teams, the team’s repositories, and access to team settings, including the ability to update the team’s description and profile picture.
1. [ ] A live chat feature that allows real-time communication between team members.
1. [ ] Financial reports related to the team's use of organization resources.
1. [ ] External links to non-GitHub resources used by the team.


---

# question-058.md

---
question: "What is the role of a Security Manager within a GitHub organization?"
title: "Question 058"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] A security manager has permissions to view security alerts and manage settings for code security across the organization, in addition to read permissions for all repositories.
1. [ ] Security managers are responsible for financial transactions and billing information security within the organization.
1. [ ] They can delete or transfer ownership of any repository within the organization for security reasons.
1. [ ] Security managers exclusively manage two-factor authentication settings for all organization members.


---

# question-059.md

---
question: "What permissions does a GitHub App manager have within an organization?"
title: "Question 059"
---

> https://docs.github.com/en/organizations/managing-programmatic-access-to-your-organization/adding-and-removing-github-app-managers-in-your-organization#about-github-app-managers
1. [x] GitHub App managers can manage the settings of GitHub App registrations owned by the organization but do not have permissions to install or uninstall GitHub Apps.
1. [ ] They can access and modify the source code of any GitHub Apps owned by the organization.
1. [ ] GitHub App managers are the only roles that can create new GitHub Apps within the organization.
1. [ ] They have the ability to grant app installation permissions to outside collaborators.


---

# question-060.md

---
question: "What roles can a team member hold within a GitHub team?"
title: "Question 060"
---

> https://docs.github.com/en/organizations/organizing-members-into-teams/about-teams
1. [x] Team maintainer, Team member
1. [ ] Project manager, Contributor, Viewer
1. [ ] Repository owner, Repository collaborator
1. [ ] Billing manager, Security manager, App manager


---

# question-061.md

---
question: "Which repository role in a GitHub organization is recommended for contributors who need to proactively manage issues and pull requests without having write access?"
title: "Question 061"
---

> https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization
1. [x] Triage
1. [ ] Read
1. [ ] Write
1. [ ] Maintain


---

# question-062.md

---
question: "What are the repository roles available in a GitHub organization? (Choose five.)"
title: "Question 062"
---

> https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#repository-roles-for-organizations
- [x] Read
- [x] Triage
- [x] Write
- [x] Maintain
- [x] Admin
- [ ] Owner
- [ ] Moderator


---

# question-063.md

---
question: "What functionality does the audit log provide to organization admins within a GitHub organization?"
title: "Question 063"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-security-settings-for-your-organization/reviewing-the-audit-log-for-your-organization
1. [x] The audit log allows organization admins to review actions performed by members, including details such as who performed the action, what the action was, and when it was performed, aiding in security and compliance monitoring.
1. [ ] It enables organization admins to directly modify repository settings and enforce branch protection rules.
1. [ ] Audit access grants the ability to approve or reject code changes before they are merged.
1. [ ] It provides a temporary permission set for performing administrative actions within a repository.


---

# question-064.md

---
question: "Which formats are available for exporting the audit log from a GitHub organization?"
title: "Question 064"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-security-settings-for-your-organization/reviewing-the-audit-log-for-your-organization
1. [x] JSON and CSV.
1. [ ] PDF and DOCX.
1. [ ] TXT and RTF.
1. [ ] ZIP.


---

# question-065.md

---
question: "How can an organization admin search the audit log for events related to webhook modifications?"
title: "Question 065"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-security-settings-for-your-organization/reviewing-the-audit-log-for-your-organization
1. [x] By using the `operation` qualifier in the search query, such as `operation:modify` to find events where an existing resource, like a webhook, was modified.
1. [ ] Directly typing 'webhook modifications' into the audit log search bar.
1. [ ] Filtering the audit log exclusively by date range without the ability to specify event types.
1. [ ] Using voice commands to verbally request a search for webhook modification events.


---

# question-066.md

---
question: "Why might webhooks be considered an efficient alternative to the audit log or API polling in certain use cases within GitHub organizations?"
title: "Question 066"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-security-settings-for-your-organization/reviewing-the-audit-log-for-your-organization
1. [x] Webhooks provide real-time notifications to your server when specific events occur, which can be more efficient than searching the audit log or polling the API for those events.
1. [ ] Webhooks allow organization admins to manually review and approve each event before it is logged.
1. [ ] They provide a more detailed and comprehensive log of events than the audit log.
1. [ ] Webhooks are the only method to receive notifications about private repository actions.


---

# question-067.md

---
question: "Which tools can be used to remove sensitive data from a Git repository's history?"
title: "Question 067"
---

> https://docs.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository
1. [x] git filter-repo & BFG Repo-Cleaner
1. [ ] Git Merge & Git Rebase
1. [ ] Git Stash & Git Checkout
1. [ ] Git Pull & Git Fetch


---

# question-068.md

---
question: "What should you do before running git filter-repo or BFG Repo-Cleaner to remove sensitive data from your repository?"
title: "Question 068"
---

> https://docs.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository
1. [x] Merge or close all open pull requests
1. [ ] Delete the .git directory
1. [ ] Create a new branch
1. [ ] Push all local changes to GitHub


---

# question-069.md

---
question: "After sensitive data is removed from a repository's history and pushed to GitHub, what is a necessary step to fully remove the data from GitHub?"
title: "Question 069"
---

> https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#fully-removing-the-data-from-github
1. [x] Contact GitHub Support to remove cached views and references
1. [ ] Notify all users who have forked the repository
1. [ ] Change the repository's visibility to private
1. [ ] Rename the repository


---

# question-070.md

---
question: "Which of these practices can help avoid committing sensitive data or files to a git repository?"
title: "Question 070"
---

> https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository#avoiding-accidental-commits-in-the-future
1. [x] Using a visual program like GitHub Desktop to review commits
1. [ ] Regularly changing your passwords
1. [ ] Disabling push access to the repository
1. [ ] Using `git add .` before all commits


---

# question-071.md

---
question: "Which of these best defines GitHub Enterprise Policies?"
title: "Question 071"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/policies/enforcing-policies-for-your-enterprise/enforcing-repository-management-policies-in-your-enterprise
1. [x] Settings managed by organization owners to control aspects like repository management, team access, and security features within their GitHub organization.
1. [ ] Policies set at the enterprise level that dictate the billing and subscription details for all organizations under an enterprise account.
1. [ ] Guidelines suggested by GitHub to improve collaboration and productivity across all organizations without enforcement capabilities.
1. [ ] Default settings applied to all new repositories within an organization, which can be overridden by the organization owners.


---

# question-072.md

---
question: "What are enterprise policies in the context of GitHub Enterprise Cloud?"
title: "Question 072"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/policies/enforcing-policies-for-your-enterprise/enforcing-repository-management-policies-in-your-enterprise
1. [x] Enterprise policies mandate a uniform policy across all organizations within an enterprise, thereby eliminating the option for organizations to apply their own distinct policies.
1. [ ] Individual user settings that apply only to personal accounts within the GitHub Enterprise Cloud, unrelated to organizational or enterprise governance.
1. [ ] A collection of recommended practices for open-source projects hosted on GitHub, aimed at enhancing community engagement and contribution.
1. [ ] Security protocols that automatically scan and fix vulnerabilities in the codebases across all repositories within the enterprise account.


---

# question-073.md

---
question: "What steps should organization admins follow to access audit logs of actions performed within their GitHub organization?"
title: "Question 073"
---

> https://docs.github.com/en/organizations/keeping-your-organization-secure/managing-security-settings-for-your-organization/reviewing-the-audit-log-for-your-organization
1. [x] Select profile photo > Your organizations > Settings > Archives > Logs > Audit log. Then, use the Export dropdown to export as JSON or CSV.
1. [ ] Directly email GitHub support to request an audit log be sent monthly to the organization's admin email.
1. [ ] Navigate to the main GitHub page, use the search bar to type "Organization audit logs" and expect GitHub to automatically download the log.
1. [ ] Check individual member profiles for a summary of their actions, compile these summaries manually, and format them for auditing.


---

# question-074.md

---
question: "Which of the following are types of access tokens supported by GitHub? (Choose three.)"
title: "Question 074"
---

> https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github#githubs-token-formats
- [x] Personal Access Token (PAT)
- [x] Installation Access Token for a GitHub App
- [x] User Access Token for a GitHub App
- [ ] IoT Token for an IoT device
- [ ] Ephemeral Access Token for temporary access


---

# question-075.md

---
question: "What is the primary rate limit for authenticated personal users making REST API requests to GitHub API?"
title: "Question 075"
---

> https://docs.github.com/en/rest/using-the-rest-api/rate-limits-for-the-rest-api#primary-rate-limit-for-authenticated-users
1. [x] 5,000 requests per hour
1. [ ] 60 requests per hour
1. [ ] 15,000 requests per hour
1. [ ] 1,000 requests per hour


---

# question-076.md

---
question: "What's the difference between GitHub Apps and OAuth apps?"
title: "Question 076"
---

> https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/differences-between-github-apps-and-oauth-apps
1. [x] GitHub Apps offer granular permissions to specific repositories, while OAuth Apps request access to user data across all repositories.
1. [ ] GitHub Apps and OAuth Apps do not differ; they provide the same level of permissions.
1. [ ] OAuth Apps offer more granular permissions compared to GitHub Apps.
1. [ ] GitHub Apps can only access public repositories, whereas OAuth Apps can access both public and private repositories.


---

# question-077.md

---
question: "How can GitHub Apps react to specific events, and what are some examples of these events?"
title: "Question 077"
---

> https://docs.github.com/en/apps/creating-github-apps/registering-a-github-app/using-webhooks-with-github-apps#subscribing-to-webhook-events
1. [x] GitHub Apps subscribe to events through webhooks, which notify the app of specific actions like pull request openings or issue creations.
1. [ ] GitHub Apps can subscribe to events like push, pull request, and issue events through the app's configuration.
1. [ ] GitHub Apps work on webhooks - receiving all events from GitHub. If the GitHub App should react only on specific event, that filtering is done within the GitHub App code
1. [ ] GitHub Apps use a websocket connection that notifies the GitHub app of all `push` and `pull_request` events


---

# question-078.md

---
question: "How can enterprises track their usage of GitHub Actions?"
title: "Question 078"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/github-actions/getting-started-with-github-actions-for-your-enterprise/introducing-github-actions-to-your-enterprise#tracking-usage
1. [x] By using webhooks to subscribe to information about workflow jobs and runs, and potentially using a data archiving system.
1. [ ] By manually counting workflow runs and jobs in each repository at the end of each month.
1. [ ] Through unlimited access to GitHub's internal analytics dashboard without any additional configuration.
1. [ ] GitHub Actions usage cannot be tracked; enterprises must estimate usage based on developer feedback.


---

# question-079.md

---
question: "Who can configure IP allow lists for an enterprise on GitHub?"
title: "Question 079"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/configuration/hardening-security-for-your-enterprise/restricting-network-traffic-to-your-enterprise-with-an-ip-allow-list
1. [x] Enterprise owners
1. [ ] Organization owners
1. [ ] Security Managers
1. [ ] Organization moderators


---

# question-080.md

---
question: "Can organization owners manage IP allow list entries inherited from the enterprise account's allow list?"
title: "Question 080"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/configuration/hardening-security-for-your-enterprise/restricting-network-traffic-to-your-enterprise-with-an-ip-allow-list#about-githubs-ip-allow-list
1. [x] No, they cannot manage entries inherited from the enterprise account's allow list
1. [ ] Yes, they have full control over inherited entries
1. [ ] Yes, but only with approval from enterprise owners
1. [ ] No, only GitHub support can manage inherited entries


---

# question-081.md

---
question: "Which runners must you use with GitHub Actions when an IP allow list is enabled on your enterprise?"
title: "Question 081"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/configuration/hardening-security-for-your-enterprise/restricting-network-traffic-to-your-enterprise-with-an-ip-allow-list#using-github-actions-with-an-ip-allow-list
1. [x] Self-hosted runners or GitHub-hosted larger runners with static IP address ranges
1. [ ] Only GitHub-hosted standard runners
1. [ ] Any runner without considering the IP address
1. [ ] Only runners within the organization's network without IP restrictions


---

# question-082.md

---
question: "How can you ensure your self-hosted or larger hosted runners can communicate with GitHub when using an IP allow list?"
title: "Question 082"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/configuration/hardening-security-for-your-enterprise/restricting-network-traffic-to-your-enterprise-with-an-ip-allow-list#using-github-actions-with-an-ip-allow-list
1. [x] Add the IP address or IP address range of your runners to the IP allow list configured for your enterprise
1. [ ] Disable the IP allow list for GitHub Actions runners
1. [ ] Register the runners in Enterprise > Network security > Actions settings
1. [ ] Use a VPN for all runners to bypass the IP allow list


---

# question-083.md

---
question: "When an Enterprise IP allow list is in place, what happens when you try publish your GitHub Pages site from a branch instead of using a custom GitHub Actions workflow?"
title: "Question 083"
---

> https://docs.github.com/en/enterprise-cloud@latest/admin/configuration/hardening-security-for-your-enterprise/restricting-network-traffic-to-your-enterprise-with-an-ip-allow-list#using-github-pages-with-an-ip-allow-list
1. [x] The build runner will have access to the repository for the GitHub Pages site by default
1. [ ] The build runner will be blocked from accessing the repository until manually added to the allow list
1. [ ] GitHub Pages cannot be built or updated until the IP allow list is disabled
1. [ ] You must manually trigger builds for GitHub Pages sites


---

# question-084.md

---
question: "What are some potential abuse vectors of enabling self-hosted runners on public repositories? (Choose four.)"
title: "Question 084"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/about-self-hosted-runners#self-hosted-runner-security
- [x] Malicious programs running on the machine
- [x] Escaping the runner sandbox environment
- [x] Exposing network environment
- [x] Persisting dangerous data
- [ ] Automatic environment cleanup after job execution can cause data loss
- [ ] Lower computational efficiency due to security measures
- [ ] Limited integration with GitHub-hosted services


---

# question-085.md

---
question: "How should you select appropriate runners to support your workflow's specific workloads?"
title: "Question 085"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/about-self-hosted-runners#differences-between-github-hosted-and-self-hosted-runners
1. [x] Choose self-hosted runners for customized environments or GitHub-hosted for automatic updates and clean instances.
1. [ ] Always prefer GitHub-hosted runners for all workloads to ensure maximum security.
1. [ ] Use only self-hosted runners, regardless of workload complexity, to minimize costs.
1. [ ] Restrict to using GitHub-hosted runners with custom hardware configurations for better performance.


---

# question-086.md

---
question: "How do you add a self-hosted runner to a GitHub repository?"
title: "Question 086"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/adding-self-hosted-runners
1. [x] Navigate to the repository settings, select Actions, then Runners, and follow the instructions to download, configure, and run the self-hosted runner application.
1. [ ] Directly clone the repository to your local machine and run a specific script to automatically add it as a self-hosted runner.
1. [ ] Email GitHub support to request the addition of a self-hosted runner to your repository.
1. [ ] Use the GitHub API to send a request for adding a self-hosted runner without any manual configuration.


---

# question-087.md

---
question: "What is required to add a self-hosted runner to an organization on GitHub?"
title: "Question 087"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/adding-self-hosted-runners
1. [x] Organization owner access, navigate to organization settings, select Actions, then Runners, and follow the setup instructions for the self-hosted runner.
1. [ ] General member access with no special permissions, and utilize a GitHub Action to automatically register a self-hosted runner.
1. [ ] Public repository access within the organization and manual script execution on the server intended as a runner.
1. [ ] Submit a form on GitHub's website to request the GitHub team to add a self-hosted runner to your organization manually.


---

# question-088.md

---
question: "How can you manage access to self-hosted runners in an organization using runner groups?"
title: "Question 088"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-access-to-self-hosted-runners-using-groups
1. [x] Create runner groups to collect sets of runners, then configure access policies for repositories within the organization.
1. [ ] Manually assign each self-hosted runner to individual repositories without using runner groups.
1. [ ] Use a single default runner group for all runners and repositories
1. [ ] By creating runner groups which are then assigned to teams of people within an organization. These teams can then manage these groups and assign the runner groups to repositories they manage


---

# question-089.md

---
question: "What steps are involved in creating a self-hosted runner group for an organization on GitHub?"
title: "Question 089"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-access-to-self-hosted-runners-using-groups
1. [x] Navigate to organization settings, select Actions, click Runner groups, create a new group, and assign a repository access policy.
1. [ ] In the `.github` repository modify the `.gitconfig` file to specify runner groups and associated access policies.
1. [ ] Contact GitHub support to request the creation of a runner group and provide a list of repositories for access configuration.
1. [ ] Use a GitHub Actions workflow to automatically generate runner groups based on repository activity and usage patterns.


---

# question-090.md

---
question: "How do you change which repositories can access a specific runner group in an organization?"
title: "Question 090"
---

> https://docs.github.com/en/actions/hosting-your-own-runners/managing-access-to-self-hosted-runners-using-groups
1. [x] In organization settings, navigate to Actions, select Runner groups, choose a group, and modify the repository access settings.
1. [ ] Use the GitHub CLI to execute a command that reassigns repository access to different runner groups within the organization.
1. [ ] Edit the runner group's configuration file located on the server hosting the self-hosted runners to update repository access.
1. [ ] Repositories automatically gain access to all runner groups without the need for manual configuration changes.


---

# question-091.md

---
question: "How can you use 3rd party vaults to manage secrets for GitHub Actions?"
title: "Question 091"
---

> https://developer.hashicorp.com/vault/docs/platform/github-actions
> https://bitwarden.com/help/github-actions-integration/
> https://docs.keeper.io/en/keeperpam/secrets-manager/integrations/github-actions
1. [x] Store secrets in the 3rd party vault and use a decryption step in your workflow to access them, with the decryption key stored as a GitHub Actions secret.
1. [ ] Direct integration with 3rd party vaults is supported natively within GitHub Actions without needing any additional configuration.
1. [ ] Third party vaults should be accessed by embedding their API keys within the workflow files and using the API or CLI of that vendor
1. [ ] GitHub Actions does not support the use of 3rd party vaults for secret management; all secrets must be stored within GitHub.


---

# question-092.md

---
question: "Which package managers and formats are supported by GitHub Packages? (Choose five.)"
title: "Question 092"
---

> https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages#about-github-packages
- [x] npm for JavaScript
- [x] RubyGems for Ruby
- [x] Maven and Gradle for Java
- [x] Nuget for .NET
- [x] Docker and OCI images
- [ ] Poetry for Python
- [ ] Cargo for Rust


---

# question-093.md

---
question: "How can one authenticate to GitHub Packages?"
title: "Question 093"
---

> https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages#authenticating-to-github-packages
1. [x] By authenticating using a PAT with appropriate scope
1. [ ] GitHub Packages can be accessed and shared publicly without any authentication.
1. [ ] Access to GitHub Packages is restricted to GitHub Enterprise accounts only.
1. [ ] By using the default GitHub login without needing any special authentication tokens.


---

# question-094.md

---
question: "What is required to download or publish a GitHub Package within workflows, such as with GitHub Actions or other CI/CD tools?"
title: "Question 094"
---

> https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages#authenticating-to-github-packages
1. [x] Use `GITHUB_TOKEN` for publishing packages associated with the workflow repository, and a PAT for installing packages from private repositories.
1. [ ] GitHub Packages cannot be used in GitHub Actions workflows or any CI/CD tools.
1. [ ] Only SSH keys are required for using GitHub Packages in workflows.
1. [ ] Manual download and upload of packages is required for each workflow run.


---

# question-095.md

---
question: "What are the differences and use cases between GitHub Packages and releases?"
title: "Question 095"
---

> https://docs.github.com/en/packages/learn-github-packages/introduction-to-github-packages#about-github-packages
1. [x] GitHub Packages is optimized for hosting and managing packages, offering integrated permissions management and billing, while releases are for distributing software versions directly linked to Git tags.
1. [ ] GitHub Packages and releases are functionally identical, with no differences in use cases.
1. [ ] Releases are used for private software distribution, whereas GitHub Packages is exclusively for public package hosting.
1. [ ] GitHub Packages requires external CI/CD integration for distribution, unlike releases which are fully managed within GitHub.


---

# question-096.md

---
question: "By which header can you check the number of requests you have made in the current rate limit window when using the GitHub REST API?"
title: "Question 096"
---

> https://docs.github.com/en/rest/using-the-rest-api/rate-limits-for-the-rest-api#checking-the-status-of-your-rate-limit
1. [x] `x-ratelimit-used`
1. [ ] `x-ratelimit-limit`
1. [ ] `x-ratelimit-remaining`
1. [ ] `x-ratelimit-reset`
1. [ ] `x-ratelimit-resource`


---

