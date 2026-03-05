# Bug Report: Ticket not transferred to Tracemate when Tourtyp = "Graffiti 1"

## Summary

Tickets created on the Graffiti Board are not transferred to Tracemate when the field **"Tourtyp und Fahrzeug"** is set to **"Graffiti 1"**.  
However, the transfer works correctly when other values (e.g. "Kontrolle") are used.

---

## Environment

- Environment: QA
- System: Graffiti Board
- Integration: Jira ↔ Tracemate interface
- Browser: Any

---

## Preconditions

- User has access to the Graffiti Board
- Jira – Tracemate integration is active

---

## Steps to Reproduce

1. Open the Graffiti Board
2. Create a new ticket
3. Set the ticket status to **"Stadtreinigung"**
4. Set the field **"Tourtyp und Fahrzeug"** to **"Graffiti 1"**
5. Save the ticket

---

## Expected Result

The ticket should be successfully transferred to **Tracemate**.

---

## Actual Result

The ticket is **not transferred to Tracemate**.

---

## Additional Observations

- When the field **"Tourtyp und Fahrzeug"** is set to **"Kontrolle"**, the transfer works correctly.
- This suggests a possible issue in the **mapping or validation logic** for the value **"Graffiti 1"**.

---

## Possible Root Cause

The integration logic may not correctly handle the value **"Graffiti 1"** during the data transfer process.

---

## Severity

Medium – prevents specific ticket types from being processed through the integration.