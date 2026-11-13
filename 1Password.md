# 1Password — IT Administration, Vault Access & Account Cleanup

Lyle,

I need you to complete the configuration and cleanup of our company 1Password environment.

The objective is to ensure that you and I both have full administrative capabilities, access to all company-managed shared vaults, and that our user accounts and permissions are properly maintained.

Our 1Password environment is integrated with Microsoft Entra ID, so some changes must be made through Microsoft rather than directly in 1Password.

## 1. Microsoft Entra ID Group Membership

1. Go to https://entra.microsoft.com.
2. Navigate to **Identity → Groups → All groups**.
3. Locate **1Password - IT**.
4. Verify that both accounts are members:
   - Scott Bradley — scottbradley@yourdrugtesting.com
   - Lyle Rich — lylerich@yourdrugtesting.com
5. Add any missing memberships.
6. Review other Entra-managed 1Password groups to determine whether additional membership is required.

If group membership is managed dynamically or through another provisioning configuration, investigate that configuration rather than creating duplicate groups.

## 2. 1Password Administrator Permissions

1. Sign in at https://start.1password.com.
2. Open the Admin Console.
3. Navigate to **Groups → Administrators**.
4. Verify that both Scott and Lyle are administrators.
5. Add any missing memberships using the appropriate management method.
6. Verify that both accounts can manage users, groups, vaults, and permissions.

We should have equivalent administrative capabilities. Ownership and billing permissions are not necessary unless specifically required.

## 3. Access to All Shared Vaults

1. Navigate to **Vaults** in the 1Password Admin Console.
2. Review every company-managed shared vault.
3. Confirm that both Scott and Lyle have access, preferably through the **1Password - IT** group.
4. Configure appropriate permissions to view, create, edit, copy, and share credentials.
5. Verify that both accounts can access all intended shared vaults.

This does not include employees' private vaults.

## 4. Remove Logan Wooldridge

Logan has been gone for approximately four months. His 1Password account currently shows as suspended.

1. Confirm his account remains suspended.
2. Remove him from the **1Password - IT** group and any other access groups.
3. Review credentials, integrations, or recovery responsibilities associated with his account.
4. Transfer anything still needed to an active administrator.
5. Identify and rotate shared privileged credentials that may still be known to him.
6. Permanently remove his account once retention and offboarding checks are complete.

## 5. Investigate and Resolve the IT Support Account

The **itsupport@yourdrugtesting.com** account is an IT-owned account that we need to retain.

It currently appears in 1Password with a **Needs Recovery** status.

Please:

1. Investigate why the account requires recovery.
2. Determine whether this is an account recovery issue, authentication issue, or provisioning issue.
3. Complete the appropriate recovery process.
4. Verify that the account can authenticate successfully.
5. Confirm its permissions and group memberships are appropriate.
6. Document how the account is managed and recovered.

We need this account functioning properly, but it should not be used as a substitute for our individual administrator accounts.

## 6. Review Other Accounts and Permissions

While completing this work, review the remaining 1Password users and groups for:

- Former employees who still have access.
- Duplicate accounts.
- Accounts requiring recovery or confirmation.
- Excessive administrative privileges.
- Unnecessary vault access.
- Problems with Entra ID provisioning or synchronization.

Correct routine access issues and flag anything that requires further review.

## 7. Final Verification

When complete, confirm the following:

- [ ] Scott and Lyle both have 1Password administrator privileges.
- [ ] Both have access to all intended company-managed shared vaults.
- [ ] Entra ID group provisioning is working correctly.
- [ ] Logan's access has been removed, with permanent deletion handled appropriately.
- [ ] The IT support account is recovered and functioning.
- [ ] Other inactive or unnecessary accounts have been reviewed.
- [ ] Any outstanding security or configuration issues have been documented.

Please handle this cleanup and send me a summary of what was completed, what you discovered, and anything that still needs attention.
