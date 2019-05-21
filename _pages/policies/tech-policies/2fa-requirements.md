---
title: Setting up two-factor authentication (2FA)
permalink: /2fa-requirements/
---

The VA requires two-factor authentication for anyone accessing one of the VA’s private repositories on GitHub.com. 

Two-factor authentication (2FA) is a security measure. In addition the typical username and password, logging in with 2FA requires a numeric code -- either via a SMS message or a special app.

Step-by-step instructions follow. But you can read [more detailed instructions for 2FA setup][1] in the GitHub Help documentation.

## Enabling 2FA for GitHub.com

1. If you do not have 2FA set up when you are invited to join, you'll find that the `Enable two-factor authentication` button is active and the `Join Department of Veterans Affairs` button is disabled.

    Here's what you need to do:

    [![accept\_invite\_email\_screen\_no\_2fa.png][image-1]][2]

2. Once you click `Enable two-factor authentication`, you'll be taken to your settings page and the first screen for 2FA setup:

    [![2fa\_setup\_screen\_1.png][image-2]][3]

3. Second screen for 2FA setup:

    [![2fa\_setup\_screen\_2.png][image-3]][4]

4. 2FA Account Security Codes.

    These are backup codes you can use if you misplace your phone or can’t receive an SMS. Keep them in a safe place.

    [![2fa\_setup\_screen\_3\_a.png][image-4]][5]

5. 2FA Account Security Codes Next button active: 

    [![2fa\_setup\_screen\_3\_b.png][image-5]][6]

6. Using an app for 2FA

    1. 2FA Setup usging an app: 

        If you choose to use a mobile app to setup 2FA such as Authy or Google Authenticator, you’ll see this screen. Any app that supports the TOTP protocol will work, so you may already have one of these. Follow the instructions provided by your app to scan the code, then confirm your setup by typing one of the 2FA numbers it provides.

        [![2fa\_setup\_screen\_4\_app.png][image-6]][7]

7. Using SMS for 2FA

    1. 2FA Setup using SMS: 

        You could instead choose to receive 2FA codes by SMS text messaging. This is a good choice if you will always have your phone with you (and your office has good enough cellular reception for you to receive text messages).

        [![2fa\_setup\_screen\_4\_sms\_a.png][image-7]][8]

    2. 2FA Setup using SMS second screen: 

        After entering your cell number and clicking `Send authentication code`, you will need to enter the code you receive by SMS in the textbox below.

        [![2fa\_setup\_screen\_4\_sms\_b.png][image-8]][9]

8. Setup Complete

    1. 2FA Setup complete: 

        [![2fa\_setup\_screen\_5.png][image-9]][10]

    2. Now go back and accept your invitation to the [VA organization on GitHub][11]. View invite banner by returning to org page: 

        [![invite\_notification\_in\_org.png][image-10]][12]

Back to: [main site]({{site.baseurl}}/) | [Joining VA Github Organization]({{site.baseurl}}/join-va-org/)

[1]: https://help.github.com/en/articles/configuring-two-factor-authentication
[2]: {{site.baseurl}}/images/2fa/accept_invite_email_screen_no_2fa.png
[3]: {{site.baseurl}}/images/2fa/2fa_setup_screen_1.png
[4]: {{site.baseurl}}/images/2fa/2fa_setup_screen_2.png
[5]: {{site.baseurl}}/images/2fa/2fa_setup_screen_3_a.png
[6]: {{site.baseurl}}/images/2fa/2fa_setup_screen_3_b.png
[7]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_app.png
[8]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_sms_a.png
[9]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_sms_b.png
[10]: {{site.baseurl}}/images/2fa/2fa_setup_screen_5.png
[11]: https://github.com/department-of-veterans-affairs
[12]: {{site.baseurl}}/images/2fa/invite_notification_in_org.png

[image-1]: {{site.baseurl}}/images/2fa/accept_invite_email_screen_no_2fa.png
[image-2]: {{site.baseurl}}/images/2fa/2fa_setup_screen_1.png
[image-3]: {{site.baseurl}}/images/2fa/2fa_setup_screen_2.png
[image-4]: {{site.baseurl}}/images/2fa/2fa_setup_screen_3_a.png
[image-5]: {{site.baseurl}}/images/2fa/2fa_setup_screen_3_b.png
[image-6]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_app.png
[image-7]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_sms_a.png
[image-8]: {{site.baseurl}}/images/2fa/2fa_setup_screen_4_sms_b.png
[image-9]: {{site.baseurl}}/images/2fa/2fa_setup_screen_5.png
[image-10]: {{site.baseurl}}/images/2fa/invite_notification_in_org.png
