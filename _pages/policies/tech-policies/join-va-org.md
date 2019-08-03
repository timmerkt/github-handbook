---
title: Accepting a GitHub invitation
permalink: /join-va-org/
---

# Accepting a GitHub invitation

The VA uses GitHub to manage collaboration around code and other projects in a way that meets VA security requirements. To that end, we'd like to share some helpful tips on accessing and securing your account :rocket::

- For background, you may want to read about the [two versions of GitHub in use at VA][11]

### 1. Sign up for a GitHub.com account

If your project, like most at the VA, is hosted on GitHub.com (also called GitHub Enterprise Cloud), you'll need to sign up for an account yourself.

- Sign up for a new GitHub.com account: <https://github.com/join>
  - Use your VA username (the part before the @ sign of your email)
    - Like this: eric-johnson5
  - And your VA email address
- If you already have a GitHub.com account, [add your VA email address and your real name to it][12]
- Use this GitHub.com user name to [request access to the VA organization][11]


### 2. Join the Department of Veterans Affairs organization on GitHub.com

After you [request access to the VA organization][11], you should receive an  email inviting you to join the VA organization. You'll need to log in and agree to this before you access any private repository at the VA.

1. Before you can access repositories in the [Veterans Affairs Organization on GitHub][1], you must accept an invitation join the organization:
    1. This will be sent to your VA address by email. (Search for an email message from github.com).

        <details><summary>Here's an example of that invitation email:</summary>
        <a href="2fa-docs/github_email.png"><img src="2fa-docs/github_email.png"/></a>
        </details>

    2. If you don't want to wait for the email, log in and look for the **View invitation** button in the banner of the Department-of-Veterans-Affairs Organization page <https://github.com/department-of-veterans-affairs>: 

        [![invite\_notification\_in\_org.png][image-2]][4]

2. Click **View invitation**, for the details. On the next screen, you'll be asked to confirm that you want to join the VA organization. VA policy requires everyone to enable 2-factor authentication, so you may have one more thing to do. 

    1. If you haven't yet set up 2FA, you'll find the `Enable two-factor authentication` button is active and the `Join Department of Veterans Affairs` button is disabled.

        In this case, [see our instructions for setting up 2FA.][10]


        [![accept\_invite\_email\_screen\_no\_2fa.png][image-3]][10]


    2. Accept invite screen with 2FA active:

        If you already have activated 2FA, the `Join Department of Veterans Affairs` button will be active. Simply click to join the VA organization.

        [![accept\_invite\_email\_screen.png][image-4]][7]


3. Once you successfully accepted the invitation, you'll see a blue banner at the top of the screen: 

    [![invite\_accespted.png][image-5]][8]


#### You've accepted your invitation — congratulations!

You are now a member of the [department-of-veterans-affairs organization][9]. You can create private repositories now and also be added to existing teams or repositories (by a team maintainer or a repository admin).



[1]: https://github.com/department-of-veterans-affairs
[2]: {{site.baseurl}}/images/2fa/github_email.png
[3]: https://github.com/department-of-veterans-affairs
[4]: {{site.baseurl}}/images/2fa/invite_notification_in_org.png
[5]: {{site.baseurl}}/images/2fa/accept_invite_email_screen_no_2fa.png
[6]: https://help.github.com/en/articles/configuring-two-factor-authentication
[7]: {{site.baseurl}}/images/2fa/accept_invite_email_screen.png
[8]: {{site.baseurl}}/images/2fa/invite_accespted.png
[9]: https://github.com/department-of-veterans-affairs
[10]: {{site.baseurl}}/2fa-requirements/
[11]: https://vaww.oit.va.gov/services/github/
[12]:   https://github.com/settings/emails

[image-1]: {{site.baseurl}}/images/2fa/github_email.png
[image-2]: {{site.baseurl}}/images/2fa/invite_notification_in_org.png
[image-3]: {{site.baseurl}}/images/2fa/accept_invite_email_screen_no_2fa.png
[image-4]: {{site.baseurl}}/images/2fa/accept_invite_email_screen.png
[image-5]: {{site.baseurl}}/images/2fa/invite_accespted.png
