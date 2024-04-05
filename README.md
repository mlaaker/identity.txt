# identity.txt
Server configuration file to instruct password managers how to best create and update accounts/credentials

Account security is a constant challenge for both apps/services needing stronger protections for their users' data and for users trying to reasonably manage an ever-growing account keychain with each service setting arbitrary authentication rules. In the middle sit a suite of Password or Keychain Managers, such as 1Password, LastPass, Dashlane, Authy, Google Password Manager, Microsoft Autofill, and iCloud Keychain. 

In the model of the [Robots Exclusion Protocol](https://www.rfc-editor.org/rfc/rfc9309.html), identity.txt is a standard for machine-readable server-hosted text file to:
* define the authentication requirements and related details associated with the organization's sites and apps,
* ensure that Password Managers (like 1Password, LastPass, Dashlane, iCloud Keychain and Google Password Manager) have an automated way to understand a site or app's authentication requirements, and tailor their Password Generators and Autofill behaviors accordingly. 
supply a wider range of Identity attestations, such as their online profiles, contact methods, and support services, to simplify such services' facilitation of followup actions.

At minimum, such a standard enables Password/Keychain Managers to identify the availablity of and specific requirements around:
* passkeys
* passwords (# min/max, special characters, rules)
* usernames
* security keys
* second-factor formats (SMS, app, THOTH, etc)
* reset link
* creation link
* 'Sign In with' providers

