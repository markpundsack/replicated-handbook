# Security Setup

Getting started with Replicated security.

**Your Laptop**

Replicated uses Apple laptops for all employees. When you receive your laptop you will install our device management software on the device, currently Replicated uses [Fleetsmith](https://www.fleetsmith.com) to enforce device policies and to allow the device to be disabled remotely if it is ever lost or stolen.

On your device we ask that you use your best judgement on installing applications. You can consider any application directly purchased by Replicated to be officially approved for usage on your device. Major applications that are not directly tied to your work but are helpful for productivity are okay to use like Spotify when downloaded from the Mac App Store. Please do not install third-party application marketplaces like Steam.

Note that there are well known applications and browser extensions that gather excessive information about the user like Grammarly. We do not use Grammarly in any form because of the information that it gathers. Also, treat browser extensions the same way you would an application downloaded directly to your device. You can use extensions for applications purchased by Replicated bu use your judgement and ask for approval for other extensions.

**Antivirus**

Replicated uses Cylance for antivirus. You should download when invited and keep updated.

**YubiKey**

Replicated uses [yubikeys](https://www.yubico.com) for authentication. Please use as an authentication factor wherever available to do so. This should be used as a token for your Okta SSO login.

**Password Management**

Replicated uses [1Password](https://1password.com/teams/) for password management. All passwords for any Replicated account should be generated through 1Password and stored in 1Password. Your 1Password master password should be a passphrase longer than twelve characters. Any passwords or sensitive information that is shared \(even on a one-off basis\) should be shared through 1Password vaults.

**2 Factor Authentication**

For two-factor authentication always choose physical authentication through your yubikey where available, or through an authenticator app which generates an ephemeral token. Do not use SMS authentication if you have other options \(yubikey &gt; authenticator &gt; email &gt; nothing &gt; SMS\).

