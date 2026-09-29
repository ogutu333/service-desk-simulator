# Ticket 04 — Nobody on the 3rd Floor Has Internet

**Category:** Network / Infrastructure  
**Priority:** Critical  
**Status:** Resolved  
**Reported By:** Mike Reeves  
**Department:** Facilities  
**Location:** Floor 3  
**Contact:** x1095  

---

## Issue Summary

Mike Reeves reported that all users on the 3rd floor had lost internet connectivity.

The outage had started approximately 30 minutes earlier and affected both work areas and conference rooms. Users on the 2nd floor were still connected, indicating that the problem was localized to the 3rd floor rather than affecting the entire organization.

### Business Impact

* Multiple users on the 3rd floor were unable to access the internet.
* Multiple departments were unable to work normally.
* The Customer Service team could not access the CRM.
* Conference rooms on the affected floor also lost connectivity.

---

## Initial Assessment

The scope of the outage suggested that this was an infrastructure-level network issue rather than an individual user's device.

Since the entire 3rd floor was affected while the 2nd floor remained operational, I narrowed the investigation to network equipment serving the 3rd floor.

The **Floor 3 Switch** was therefore the primary device to investigate.

---

## Troubleshooting Process

### 1. Confirmed the Scope of the Outage

Reviewed the ticket information and confirmed that:

* Multiple users were affected.
* All affected users were located on Floor 3.
* Conference rooms on Floor 3 were also offline.
* Users on Floor 2 still had internet access.

This indicated a localized infrastructure issue rather than an organization-wide internet outage.

### 2. Accessed the Server Room

Navigated to:

**Tools → Server Room**

Opened the **Devices** tab to review the available network equipment.

### 3. Located the Floor 3 Switch

Identified the device labelled **Floor 3 Switch**.

Because the outage was isolated to the 3rd floor, this device was the most relevant piece of network infrastructure to investigate.

### 4. Rebooted the Switch

Used the device's **Power** button to reboot the Floor 3 Switch.

### 5. Waited for the Switch to Recover

Waited approximately **30–60 seconds** for the switch to restart and return to an operational state.

### 6. Verified Connectivity With the User

Contacted Mike through **Company Chat** and asked whether the internet connection had been restored.

The affected users confirmed that their internet connection was back.

---

## Findings

The outage was localized to Floor 3.

Other floors remained connected, while users and conference rooms on Floor 3 were simultaneously affected. This pointed toward the network infrastructure serving that floor rather than an individual workstation or organization-wide ISP outage.

Rebooting the **Floor 3 Switch** restored connectivity.

---

## Root Cause

The Floor 3 network switch had become unresponsive, resulting in loss of network connectivity for devices connected through that switch.

The simulator does not identify a specific underlying reason for why the switch became unresponsive.

---

## Resolution

The issue was resolved by:

1. Confirming that the outage affected multiple users on Floor 3.
2. Comparing the affected floor with the unaffected 2nd floor.
3. Accessing the Server Room through the simulator.
4. Locating the **Floor 3 Switch**.
5. Rebooting the switch.
6. Waiting for the switch to come back online.
7. Confirming with the affected user that internet connectivity had been restored.

**Final Status:** ✅ Resolved

---

## What I Learned

* The scope of a network outage can help identify the likely location of the problem.
* When multiple users in the same physical area lose connectivity simultaneously, shared network infrastructure should be investigated.
* Comparing affected and unaffected areas can help narrow down the source of a network issue.
* Network equipment should be given time to fully restart before determining whether a reboot resolved the problem.
* Always verify service restoration with an affected user before closing the ticket.

---

## Security Considerations

A network switch is part of the organization's core connectivity infrastructure, so troubleshooting it can affect multiple users simultaneously.

Because the outage affected an entire floor, changes to the network equipment should be limited to the identified device rather than making unnecessary changes elsewhere in the network.

The incident also demonstrates the importance of quickly identifying the **scope and blast radius** of a network outage before taking corrective action.

---

## Tools Used

| Tool                  | Purpose                                          |
| --------------------- | ------------------------------------------------ |
| ServiceDesk Simulator | Ticket environment and investigation             |
| Server Room           | Access network infrastructure                    |
| Devices Tab           | Locate network equipment                         |
| Floor 3 Switch        | Network device rebooted to restore connectivity  |
| Company Chat          | User communication and connectivity verification |

---

## References

* ServiceDesk Simulator
