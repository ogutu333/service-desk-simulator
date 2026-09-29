# Ticket 03 — Legal Name Change After Marriage

**Category:** Account Update / User Administration
**Priority:** Low
**Status:** Resolved
**Reported By:** Amanda Foster
**Department:** Finance
**Location:** Not specified
**Contact:** Not specified

---

## Issue Summary

Amanda Foster requested an update to her company account following a legal name change after marriage.

Her legal name had changed from **Amanda Foster** to **Amanda Reyes**, and HR had already approved the change and updated her employee records.

She requested that her display name and primary email address be updated while keeping her previous email address as an alias.

### Business Impact

* Employee account information did not reflect the employee's updated legal name.
* The employee required a new primary email address.
* Removing the previous email address completely could result in missed replies to existing email conversations.

---

## Initial Assessment

This was an account administration request involving a legal name change.

Before making the changes, I confirmed that HR had already approved the name change and updated Amanda's employee records.

The requested changes were:

* **Display Name:** Amanda Reyes
* **Primary Email:** [areyes@servicedesk-simulator.com](mailto:areyes@servicedesk-simulator.com)
* **Email Alias:** [afoster@servicedesk-simulator.com](mailto:afoster@servicedesk-simulator.com)
* **Username:** afoster

The username would remain unchanged to avoid potentially affecting existing logins and group memberships.

---

## Troubleshooting Process

### 1. Confirmed HR Approval

Reviewed the request and confirmed that HR had already approved the legal name change and updated Amanda's employee records.

This was important because account identity changes should be based on an approved organizational record rather than an unverified user request.

### 2. Opened the Directory

Navigated to:

**Tools → Directory**

Searched for **afoster** and opened Amanda's profile.

### 3. Opened Name & Email Settings

Selected **Change Name & Email** to access the account's name and email configuration.

### 4. Updated the Display Name

Changed the display name from:

**Amanda Foster**

to:

**Amanda Reyes**

### 5. Updated the Primary Email

Changed the primary email address to:

**[areyes@servicedesk-simulator.com](mailto:areyes@servicedesk-simulator.com)**

### 6. Added the Previous Email as an Alias

Added:

**[afoster@servicedesk-simulator.com](mailto:afoster@servicedesk-simulator.com)**

as an email alias.

This ensured that messages sent to Amanda's previous address could still reach her after the primary email address changed.

### 7. Saved the Changes

Clicked **Save Changes** to apply the updated account information.

---

## Findings

The account could be updated without changing the employee's existing username.

The display name and primary email address required updating, while the previous email address needed to be manually added as an alias.

---

## Root Cause

The account information required updating because the employee had undergone an approved legal name change.

The existing account still reflected the employee's previous legal name and email address.

---

## Resolution

The account was updated by:

1. Confirming HR approval of the legal name change.
2. Locating Amanda's account in the Directory.
3. Updating the display name to **Amanda Reyes**.
4. Changing the primary email to **[areyes@servicedesk-simulator.com](mailto:areyes@servicedesk-simulator.com)**.
5. Adding **[afoster@servicedesk-simulator.com](mailto:afoster@servicedesk-simulator.com)** as an email alias.
6. Leaving the username **afoster** unchanged.
7. Saving the account changes.

**Final Status:** ✅ Resolved

---

## What I Learned

* Legal name changes can require updates to both account display information and primary email addresses.
* Existing email addresses should be preserved as aliases when appropriate so that users do not lose messages sent to their previous address.
* HR approval should be confirmed before making employee identity changes in an organization's directory.
* Keeping an existing username can help prevent unnecessary disruption to logins and group memberships.

---

## Security Considerations

Account identity changes should be based on an approved HR record to prevent unauthorized modifications to employee accounts.

The old email address was retained as an alias rather than being removed completely. This preserves email continuity while allowing the new address to become the primary address.

The username was not changed because unnecessary changes to account identifiers can potentially affect authentication, permissions, or group memberships.

---

## Tools Used

| Tool                  | Purpose                                       |
| --------------------- | --------------------------------------------- |
| ServiceDesk Simulator | Ticket environment and account administration |
| Directory             | Locate and manage the employee account        |
| Change Name & Email   | Update account identity and email information |

---

## References

* ServiceDesk Simulator
