# Ticket 01 — VPN Disconnected and Won't Reconnect

**Category:** Network / VPN  
**Priority:** Normal  
**Status:** Resolved  
**Reported By:** Sophia Lee  
**Department:** Marketing  
**Location:** Remote / Working from Home  
**Contact:** x4260  

---

## Issue Summary

Sophia Lee reported that her VPN had disconnected and would not reconnect.

Because she was working remotely, she was unable to access internal company resources.

### Business Impact

- User unable to connect to the corporate VPN
- Internal company resources unavailable
- Marketing employee unable to perform tasks requiring internal network access

---

## Initial Assessment

The issue appeared to be isolated to the user's remote workstation rather than a company-wide VPN outage.

Since the user was working remotely, I used the available remote-support tools to investigate the workstation directly.

---

## Troubleshooting Process

### 1. Confirmed the User's Environment

Reviewed the ticket and confirmed that Sophia was:

- Working remotely
- Experiencing a VPN connectivity issue
- Unable to access internal resources

### 2. Connected to the Workstation

Used the **Remote Desktop** tool in the ServiceDesk Simulator environment to connect to the user's computer.

### 3. Opened the Terminal

Opened the Terminal application on the remote workstation.

### 4. Cleared the DNS Cache

Ran:

```bash
ipconfig /flushdns
```

This cleared the workstation's local DNS resolver cache.

### 5. Restarted the Workstation

Restarted the remote computer to apply the changes.

### 6. Signed Back Into the Workstation

After the reboot, the workstation returned to the sign-in screen.

Authentication was required before continuing the troubleshooting process.

> No passwords or credentials are stored in this portfolio.

### 7. Reconnected the VPN

Opened the VPN client and selected **Connect**.

### 8. Verified Connectivity

Confirmed that the VPN successfully re-established the connection and that the tunnel was back online.

---

## Findings

The simulator identified stale DNS cache information as contributing to the VPN reconnection failure.

After the DNS cache was cleared and the workstation restarted, the VPN was able to reconnect successfully.

---

## Root Cause

Stale DNS cache entries were identified by the simulator as the cause of the VPN reconnection failure.

---

## Resolution

The issue was resolved by:

1. Connecting to the user's workstation remotely
2. Flushing the DNS cache using `ipconfig /flushdns`
3. Restarting the workstation
4. Signing back into the workstation
5. Reconnecting the VPN
6. Verifying that the VPN connection was restored

**Final Status:** ✅ Resolved

---

## What I Learned

This ticket reinforced the importance of checking endpoint network configuration when troubleshooting VPN connectivity issues.

It also gave me practical experience with:

* Remote workstation access
* Windows network troubleshooting
* DNS cache management
* VPN troubleshooting
* Connectivity verification
* Service desk documentation

---

## Security Considerations

A VPN provides remote users with access to internal company resources. When troubleshooting VPN connectivity, it is important to ensure that the approved corporate VPN client and connection are being used.

Authentication information and passwords should never be included in portfolio documentation.

---

## Tools Used

| Tool                  | Purpose                               |
| --------------------- | ------------------------------------- |
| ServiceDesk Simulator | Ticket environment and investigation  |
| Remote Desktop        | Remote workstation access             |
| Terminal              | Command-line troubleshooting          |
| `ipconfig /flushdns`  | Clear local DNS resolver cache        |
| VPN Client            | Re-establish secure remote connection |
| Company Chat          | User communication                    |

---

## References

* Microsoft Learn — Troubleshooting DNS Clients
* ServiceDesk Simulator