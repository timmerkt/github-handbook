---
title: GitHub
tag:
- Git
---

[GitHub](https://github.com) is a platform that allows us to collaborate on documentation and code, both internally and with a broader audience.

The VA has staff that manage VA's GitHub org. See more information about that in [the VA GitHub documentation](#).

## <a id="setup">Setup</a>

GitHub is a web application, so there&rsquo;s no installation necessary, but you may find the [desktop app](https://desktop.github.com/) useful.

If you don&rsquo;t have a GitHub account, you must use your work email (rather than your personal email) to [sign up](https://github.com/join), as this helps us with identification. If you do have a GitHub account, please [add your work email to your profile](https://github.com/settings/emails) as your primary email.

### 1. Complete your profile

Include the following:

- Name: Your first or first and last name.
- Company: Your government agency. (If you also use GitHub for personal projects, consider specifying &ldquo;<code>agency</code> (work) + personal projects&rdquo; to make it clear that some of your GitHub projects may be personal in nature.)
- Location: Your primary work location (city, state).
- Photo: A headshot photo, or an image that is unique to you.

### 2. Set up two-factor authentication

[Enable two-factor authentication (2FA)](https://github.com/settings/security):

- [Use your work email](https://help.github.com/articles/setting-your-email-in-git) rather than your personal email for work-related commits. This only applies to people with more than one email address tied to their GitHub account. Note that this is different than [setting notifications to go to a specific email address](https://help.github.com/articles/choosing-the-delivery-method-for-your-notifications/). If you make commits via GitHub&rsquo;s web interface, it will use your &ldquo;primary&rdquo; email address for those commits, so check your [email settings](https://github.com/settings/emails) before making web commits.

- If you're using your work computer for personal projects on GitHub and want your personal email tied to those commits, you can set your GSA email as part of the global `.gitconfig`, then [override on a repository level](http://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration) with your personal email, or use a tool like [karn](https://github.com/prydonius/karn). If you have both emails in your [GitHub settings](https://github.com/settings/emails), they will both be tied to your GitHub account anyway.

### 3. Turn notifications on

**[Turn notifications on](https://github.com/settings/notifications)** and adjust the settings as needed. Some people watch every repo; others only watch when they're mentioned.

You will get a lot of emails when you turn notifications on. To help stem the tide, you can set up a email filter to automatically archive emails from `notifications@github.com`. However, you probably want to let through those emails that contain your GitHub username or are posted to a repo you're watching. Since on GitHub, each repo is considered its own mailing list, checking for that identifier is one reliable way to allow these notifications through. For example, if the repo name in GitHub is `18F/calc`, the mailing list will be `calc.18F.github.com`. You can also find this by opening an email from the desired repo, clicking the "more info" arrow in the "To" field, and copying the bracketed address in the "mailing list" field. Adding `list:(calc.18F.github.com)` to your filter's exceptions will allow any issues posted to that repo to reach your inbox.

### 4. Join the VA organization

- **VA team members:** After you've completed the above steps, hop into [#admins-github](https://gsa-tts.slack.com/messages/admins-github/) on Slack and **post the following**: "I've enabled two-factor authentication – please add me (`https://github.com/username`) to https://github.com/orgs/18F/teams/18f-staff/members on GitHub." An admin will verify compliance and add you, after which you'll need to accept their invite by going [here](https://github.com/orgs/18F/invitation?via_email=1).

## Rules

- **Abide by [the TTS Code of Conduct]({{site.baseurl}}/code-of-conduct).** If you see anyone violating our Code of Conduct, see the reporting section.

- **Do not grant Admin rights to anyone but 18F staff.**

- **Do not store sensitive information in GitHub**, including environment variables, private configuration data, or sensitive information about the public (including but not limited to PII). In the event that such variables or configuration data is pushed to a GitHub repository accidentally, even momentarily, consider it compromised and revoke or change the credentials immediately. Do not delete the commit itself. Then immediately follow the directions on the [incident response handbook page]({{site.baseurl}}/security-incidents). If you&rsquo;re unsure how to protect this information, consult with Infrastructure on GitHub or in the [#admins-github](https://gsa-tts.slack.com/messages/admins-github/) channel in Slack. Some projects use [Citadel](https://github.com/poise/citadel) to store secrets. Also refer to the [18F Handbook page on sensitive information]({{site.baseurl}}/sensitive-information) and [guidance on sensitive information in our open source policy.](https://github.com/18F/open-source-policy/blob/master/practice.md#protecting-sensitive-information)

    - To help you not commit sensitive information to Github, [please read about Git
      Seekrets]({{site.baseurl}}/sensitive-information#git-seekret).

- **Ask Infrastructure before integrating a service with GitHub.** Many websites offer the option to &ldquo;Sign in with GitHub&rdquo; and may further request permission to access your &ldquo;personal user data.&rdquo; Providing this level of access can not only share your public or private email address, but it can also grant the ability to access 18F&rsquo;s private repositories. For this reason, we ask that all organization members refrain from authorizing integrations and request any desired integrations through an [Infrastructure issue](https://github.com/18F/infrastructure).

- **Ask Infrastructure before creating private repositories.** We pay GitHub for the ability to create private repositories and need to bill clients for repositories created on their behalf. Before you do anything, drop into [#admins-github](https://gsa-tts.slack.com/messages/admins-github) and explain what you&rsquo;d like to do and why. Be sure to include a link in your repo README to a document that explains why it is private.  (See the **Exceptions** section of the [18F Open Source policy](https://18f.gsa.gov/open-source-policy/).)

- **You do not need approval to create public repositories.**

- **You do not need approval to archive a repository.** As discussed in the [18F open source policy](https://github.com/18F/open-source-policy/blob/master/practice.md), feel free to [archive a repository](https://help.github.com/articles/archiving-repositories/) (or ask #admins-github if you don't have permissions to do so) to deprecate it. [Here is a script to do so en masse.](https://gist.github.com/afeld/334c20d71a04bfbada95ed86194decf2) Note that archiving a repository is **not** the same as deleting a repository.

- **Ask Infrastructure before deleting repositories.** As a government team, we can’t delete repositories without Infrastructure first reviewing them for information that they may need to retain/archive (including issues, pull request comments, commit history, and other information). If you want to delete a repository, go to [#admins-github](https://gsa-tts.slack.com/messages/admins-github/) and explain what you&rsquo;d like to do and why, and wait for approval before deleting it.

- **You do not need approval to transfer a repository.** In some cases, it may make sense to transfer a repository to a client. The person performing the transfer will need to be a member of both organizations. After transferring the repository to the client's organization, create a fork of it in the 18F organization. 

## How-to

### Documentation

- [Brief onboarding class about GitHub]({{site.baseurl}}/intro-to-github).

- The VA [Open Source Policy](#) and accompanying [practice guide](#) explain why and how we write code and documentation in the open.

- [A guide to using GitHub and the Terminal](#).

- [GitHub Basics](#)

### Git and GitHub Usage

Git and GitHub are the standard tools for revision control at VA. Git is an open-source version control system, and GitHub is a commercial service that hosts Git repositories and adds extra features to support them, such as pull requests and issue tracking. Although this _sounds_ super technical, these tools are _not_ just for developers hacking code; VA uses GitHub to handle a number things including managing documentation and commenting on one another&rsquo;s work.

In other words, you&rsquo;ll probably use GitHub a lot at VA going forward. We recommend you get familiar with the basics. If you&rsquo;re new to GitHub and feel confused at first, that&rsquo;s normal. Try a few guides, review our documentation, and ask your teammates for help. GitHub also has a handy document that explains the typical [GitHub Workflow](https://guides.github.com/introduction/flow/).

### Working with outside collaborators

 <p style="color: red">need help here</p>

### Pull requests

VA defaults to using branches. Changes happen via [pull requests](https://help.github.com/articles/using-pull-requests/).

In the process of receiving feedback in a pull request, some individuals on some teams may choose to amend, reorder, or squash commits. This type of &ldquo;re-writing history&rdquo; is compliant with the Freedom of Information Act (FOIA) when it occurs on a pull request because git branches are considered a work in progress. These actions are not allowed on the master branch because that is considered the canonical source of information.

### Issues

If you want to make a suggestion to a VA project without making a specific change to its code, such as if you aren&rsquo;t sure how to fix a problem or want clarification before fixing something, file an issue on that project via GitHub. Try searching the list of open issues before you add one; the error you see might already be on the team&rsquo;s radar.

### Permissions

Teams can give groups of people administrative, write, or read permissions to VA repositories. Even if you have write access into a repository, we strongly encourage the submission of pull requests for improvements or fixes (see &ldquo;we prefer branching to forking when we&rsquo;re working together on VA projects,&rdquo; above).

Contractors or external government collaborators should only be added to teams with scoped write permissions to the repositories they're working on. They should never have administrative-level rights. In order to separate out these permissions, create a team in the format of `projectname-admins` for government staff, if necessary.

## Tips

- **Document your workflow.** There are many different ways to use GitHub, and each different team of people at the VA (likely) uses it differently. That said, teams should document their desired git workflow for each project, such as in your repository&rsquo;s ```contributing.md``` file. [GitHub flow](https://guides.github.com/introduction/flow/) is a great workflow option that can also be used as a starting point for your teams own process.

- **Do you fork or do you branch?** Git allows you to both &ldquo;fork&rdquo; and &ldquo;branch&rdquo; repositories to make a place to work on changes before you submit them for integration into the main code. **[Making a fork](https://help.github.com/articles/fork-a-repo/)** creates a copy of the repository in your own GitHub account. **Making a branch** of the main repository means you&rsquo;re working in your own little space, but it&rsquo;s still part of the main repository &mdash; which helps keep the project organized, since everyone can easily see what teammates are working on.

  **Note on forking:** Forking of private repos have been disabled for all users. Please use a branching workflow for these repos.

## Resources

- [Learning Lab](https://lab.github.com/)
- [Try Git](https://try.github.io/)

---

#### Still have questions?

Ask in Slack: [#git](https://gsa-tts.slack.com/messages/git), [#admins-github](https://gsa-tts.slack.com/messages/admins-github), [#dev](https://gsa-tts.slack.com/messages/dev)
