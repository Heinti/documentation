# Detailed, step-by-step Twilio configuration guide 
<!-- title text differs from the file one -->
1. Create Twilio Account: https://www.twilio.com/try-twilio

![Twilio welcome page](/docs/_static/images/extensions/voip-integration/detailed-twilio-getStarted.png) <!-- paths need to be chanched -->

2. In the list on the left, go to United States (US1) (or any other country) > Phone Numbers > Manage > Active Numbers and buy a number by pressing *Buy a number* button in the upper-right corner.

![Twilio buy number](/docs/_static/images/extensions/voip-integration/detailed-twilio-buyNumber.png) 

3. Search for the `sip` word and go to *Voice SIP Domains*, then press the **plus** button to create SIP Domain.

![Twilio sip search](/docs/_static/images/extensions/voip-integration/detailed-twilio-sipSearch.png) 

4. Fill up Friendly Name for your SIP Domain, its SIP URL, then create a Credential List by pressing **plus** button in *Voice Authentication* section. In the *SIP Registration* section, click on the Disable slider to enable it, and select the Credential List you created. SIP URL and SIP Credentials usernames will be used in the following points to connect the user to the SIP client and more.

![Twilio friendly name/URL](/docs/_static/images/extensions/voip-integration/detailed-twilio-sipURL.png)
![Twilio friendly name/URL](/docs/_static/images/extensions/voip-integration/detailed-twilio-sipCredList.png)

5. Go to your instance of EspoCRM, click on the three dots in the top right corner and select your User. Paste the following value into Phone field in the following format: `credential_username@SIP_URL.sip.twilio.com`. It should look something like this (it is important that the Phone type is SIP, as in the screenshot):

![Twilio friendly name/URL](/docs/_static/images/extensions/voip-integration/detailed-twilio-espoUser.png)

