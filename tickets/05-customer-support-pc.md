# Ticket 05 — Customer Support PC Completely Dead

**Category:** Hardware / Computer Replacement  
**Priority:** Critical  
**Status:** Resolved  
**Reported By:** Quinn Adams  
**Department:** Customer Support  
**Location:** Floor 1  
**Contact:** x2280  

---

## Issue Summary

Quinn Adams reported that their Customer Support desktop computer would not power on.

The workstation showed no lights, fan activity, or beep when the power button was pressed. Quinn had already tried pressing the power button several times and confirmed that the wall outlet was working by testing it with another device.

Because Quinn is a Customer Support agent with a queue of incoming calls, the hardware failure immediately affected their ability to work.

### Business Impact

* Customer Support agent unable to access their workstation.
* Agent unable to take incoming customer calls.
* Calls were accumulating in the queue.
* Customer Support operations were directly disrupted.

---

## Initial Assessment

The symptoms indicated a complete hardware power failure rather than a software or operating system issue.

Before replacing the workstation, I needed to confirm that the problem was not caused by the power source or power cable.

Because the user worked in Customer Support, I also needed to determine the appropriate replacement build. Customer Support agents require the **Server Imaging** configuration because of their legacy softphone and on-premises device policies.

---

## Troubleshooting Process

### 1. Confirmed the Power Failure

Through **Company Chat**, asked Quinn to:

* Try a known-good electrical outlet.
* Try a different power cable.

The workstation remained completely unresponsive, with:

* No power lights
* No fan activity
* No beep

This confirmed that the workstation required replacement rather than additional software troubleshooting.

### 2. Confirmed the Computer Type

Asked Quinn through **Company Chat** whether the affected machine was a laptop or desktop.

Quinn confirmed that the affected machine was a **desktop**.

This ensured that the replacement workstation would match the user's existing hardware type.

### 3. Built the Replacement Workstation

Navigated to:

**Tools → Computer Deployment**

Built a replacement workstation using **Server Imaging**.

This configuration was selected because Customer Support agents require the legacy softphone and on-premises device policies.

After the build was completed, the replacement desktop became available on the **PC Shelf**.

### 4. Collected the Shipping Address

Opened:

**Tools → Ship Manager**

Asked Quinn through Company Chat for their shipping address so the replacement workstation could be delivered.

### 5. Prepared the Replacement for Shipping

Under **Select a computer to ship**, selected the newly built desktop from the PC Shelf.

Enabled:

**Include return label**

This ensured that Quinn would have a prepaid label for returning the failed workstation.

### 6. Shipped the Replacement

Kept the shipping speed set to:

**Rush Priority (Instant)**

Selected **Ship** to dispatch the replacement workstation.

### 7. Arranged Return of the Failed Workstation

Instructed Quinn to return the failed desktop using the prepaid return label included with the replacement shipment.

---

## Findings

The desktop remained completely unresponsive after testing with a known-good outlet and different power cable.

The symptoms were consistent with a hardware failure affecting the system's ability to power on.

Because the affected user was a Customer Support agent, the replacement needed to use the appropriate **Server Imaging** configuration rather than Cloud Provisioning.

---

## Root Cause

The desktop had experienced a hardware-level power failure.

The simulator indicates that a machine showing no lights, fan activity, or beep after testing a known-good outlet and power cable should be replaced.

The specific failed hardware component was not identified.

---

## Resolution

The issue was resolved by:

1. Confirming the desktop remained completely dead using a known-good outlet and power cable.
2. Confirming that the affected device was a desktop.
3. Building a replacement desktop using **Server Imaging**.
4. Confirming the replacement appeared on the PC Shelf.
5. Obtaining the user's shipping address.
6. Selecting the replacement desktop in Ship Manager.
7. Including a prepaid return label.
8. Shipping the replacement using **Rush Priority (Instant)**.
9. Arranging for the failed desktop to be returned.

**Final Status:** ✅ Resolved

---

## What I Learned

* A computer showing no lights, fan activity, or beep after basic power checks should be treated as a potential hardware failure rather than repeatedly restarting it.
* Troubleshooting should begin by eliminating simple external causes such as a faulty outlet or power cable.
* The user's role can determine which system configuration is required for a replacement device.
* Customer Support agents require **Server Imaging** because of their legacy softphone and on-premises device policies.
* Replacement hardware should be shipped with a return label so failed equipment can be recovered.
* When an issue directly prevents a user from performing their primary job function, restoring access quickly is an important service-desk priority.

---

## Security Considerations

Hardware replacement also involves protecting organizational data and maintaining device-management controls.

The replacement workstation must use the organization's approved deployment configuration rather than an alternative provisioning method that may not provide the required security policies or applications.

The failed workstation should also be returned to the organization using the provided return process so that the device can be handled according to the organization's hardware and asset-management procedures.

Shipping information should be handled through the approved service-desk workflow and should not be stored unnecessarily in portfolio documentation.

---

## Tools Used

| Tool                  | Purpose                                            |
| --------------------- | -------------------------------------------------- |
| ServiceDesk Simulator | Ticket environment and investigation               |
| Company Chat          | User communication and troubleshooting             |
| Computer Deployment   | Build the replacement workstation                  |
| Server Imaging        | Deploy the required Customer Support configuration |
| PC Shelf              | Locate the completed replacement computer          |
| Ship Manager          | Prepare and ship replacement hardware              |
| Return Label          | Facilitate return of the failed workstation        |

---

## References

* ServiceDesk Simulator
* Documentation → Hardware & Assets → Choosing a PC Setup
