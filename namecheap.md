
# IT Assignment: Namecheap Account Security & Ownership Cleanup

**Assigned to:** Lyle Rich  
**Project:** Tomo IT Infrastructure Audit  
**Priority:** High  
**Objective:** Secure Tomo's Namecheap account, establish reliable IT notifications, update credentials, and investigate moving company assets into a dedicated corporate account.

## 1. Configure Namecheap Email Notifications

The Namecheap primary email has already been updated to `itsupport@yourdrugtesting.com`.

Configure an Exchange Online mail flow rule so Namecheap notifications received by IT Support also reach Scott and Lyle.

Requirements:
- Use a server-side Exchange mail flow rule.
- Match verified Namecheap sender addresses.
- Preserve messages in the IT Support mailbox.
- Avoid duplicate notifications and forwarding loops.
- Test successful delivery to both administrators.

## 2. Secure the Existing Namecheap Account

Current account information:
- Username: `mickeymoore`
- Account name: Lyle Rich
- Primary email: `itsupport@yourdrugtesting.com`
- Two-factor authentication: Disabled

Tasks:
- Generate a new, strong password using 1Password.
- Change the Namecheap password.
- Enable two-factor authentication using an approved IT-controlled authenticator.
- Securely store MFA backup codes in the restricted IT vault.
- Confirm both Scott and Lyle have authorized access.

**Do not change the existing Recovery Settings, Security Alerts, or Incoming Invitations settings. Scott has reviewed and approved their current configuration.**

## 3. Mandatory MFA Coordination — Scott and Lyle

Scott and Lyle must both be able to authenticate when accessing the Namecheap account.

**Lyle must coordinate any MFA enrollment with Scott before completing activation.**

1. When Namecheap displays an authenticator QR code or setup key, stop and coordinate with Scott before completing enrollment.
2. Arrange a secure setup session so Scott can enroll his authenticator using the same initial setup information, if Namecheap supports this.
3. Lyle must enroll his approved authenticator or establish access through the authorized shared 1Password TOTP credential.
4. Do not transmit QR codes, setup keys, or backup codes through ordinary email or Teams messages.
5. If Namecheap supports only one authenticator enrollment, confirm the supported method for providing access to both administrators before proceeding.
6. Verify that Scott and Lyle can each generate valid authentication codes.
7. Store recovery codes securely in the restricted IT administrative vault.
8. Do not consider MFA implementation complete until both administrators have verified access.

**Important:** Scott must be involved whenever an account setup requires an authenticator, QR code, security key, or another authentication method he will also need to use. Sharing a TOTP secret permits access but does not provide separate user identities; individual administrator accounts are preferable if supported.

## 4. Mandatory Lockout Prevention

1. Verify that IT Support receives Namecheap emails and both administrators can access the mailbox.
2. Confirm the proposed MFA method and coordinate enrollment with Scott.
3. Keep the existing authenticated Namecheap session open.
4. Enroll both administrators using the supported authentication method.
5. Securely store backup codes.
6. Generate and change the account password.
7. Update the Namecheap entry in 1Password.
8. Open a separate private browser session and verify the new password and MFA.
9. Have Scott verify access from his own device.
10. Close the original session only after successful verification.

If verification fails, stop and preserve the existing session. Contact Namecheap Support if necessary. Do not modify approved recovery settings.

## 5. Update 1Password

Locate and update the Namecheap entry with:
- Correct login URL
- Current username
- New password
- Primary email
- MFA configuration, including TOTP if supported
- Backup recovery codes, stored with appropriate restrictions
- Account ownership information
- Date credentials were verified

Confirm Scott and Lyle can access the appropriate credential and authentication information. Review duplicate or outdated entries, but do not delete them until the new credentials have been verified.

## 6. Investigate a New Corporate Namecheap Account

Contact Namecheap Support to determine whether Tomo should retain the existing account or create a new company-controlled account.

Proposed configuration:
- Account name: Tomo Drug Testing
- Username: `tomoit` or similar
- Primary email: `itsupport@yourdrugtesting.com`
- Administrative ownership: Tomo IT
- Credentials: Managed in 1Password

Determine:
1. Whether the existing username can be changed.
2. Whether domains can be moved internally between Namecheap accounts.
3. Whether nameservers and DNS records remain unchanged.
4. Whether SSL certificates and hosting services can be transferred.
5. Whether billing, renewals, and expiration dates are preserved.
6. Whether separate administrator accounts are supported.
7. Whether a new account can use the existing IT Support email address.
8. What migration process Namecheap recommends to avoid service interruption.

**Investigation only. Do not create or migrate to a new account without Scott's approval.**

## 7. Inventory Existing Namecheap Assets

Document:
- All registered domains
- Domain expiration dates
- Nameservers
- DNS hosting providers
- SSL certificates and expiration dates
- Hosting services and subscriptions
- Automatic renewal settings
- Other purchased services

Investigate the two expiring or expired items shown in the dashboard.

## 8. Deliverables

Provide Scott with a short summary confirming:
- Namecheap notifications reach both IT administrators.
- Password has been changed.
- MFA is enabled and verified by Scott and Lyle.
- 1Password has been updated.
- Existing recovery and alert settings remain unchanged.
- Namecheap assets have been inventoried.
- Namecheap Support has explained the available migration options.
- A recommendation has been prepared to retain or replace the existing account.

## Change Restrictions

Do not change DNS records, nameservers, domain ownership, hosting configurations, SSL certificates, or existing recovery and alert settings without Scott's approval.

**Success criteria:** Tomo's Namecheap account is secured, both IT administrators receive notifications and can authenticate successfully, credentials are documented in 1Password, and a safe account migration strategy has been identified without disrupting production services.
