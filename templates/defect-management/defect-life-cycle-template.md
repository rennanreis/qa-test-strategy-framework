# Defect Life Cycle Template

## Overview

The defect life cycle (bug life cycle) is the process a defect goes through from its discovery to its closure. Each stage has a specific purpose and responsible party.

## Stages

1. **New**  
   - The defect is reported and logged in the tracking system.
   - Status: New

2. **Assigned**  
   - The defect is reviewed and assigned to a developer for investigation and fixing.
   - Status: Assigned

3. **Open**  
   - The developer starts working on the defect.
   - Status: Open

4. **Fixed**  
   - The developer resolves the defect and marks it as fixed.
   - Status: Fixed

5. **ReTest**  
   - QA/tester retests the application to verify the fix.
   - Status: ReTest

6. **Verified**  
   - If the defect is fixed, QA marks it as verified.
   - Status: Verified

7. **Closed**  
   - The defect is considered resolved and closed.
   - Status: Closed

8. **Reopened** (if necessary)  
   - If the defect persists, it is reopened and the cycle continues.
   - Status: Reopened

## Example Table

| Status    | Description                                 | Responsible      | Action/Next Step           |
|-----------|---------------------------------------------|------------------|----------------------------|
| New       | Defect reported and logged                  | Tester           | Assign for triage          |
| Assigned  | Defect assigned to developer                | Project Manager  | Developer investigates     |
| Open      | Developer working on defect                 | Developer        | Fix the defect             |
| Fixed     | Defect fixed, pending verification          | Developer        | QA retests                 |
| ReTest    | QA retests the defect                       | QA               | Mark as Verified/Rejected  |
| Verified  | Defect fix confirmed                        | QA               | Close defect               |
| Closed    | Defect fully resolved                       | QA/Manager       | Archive defect             |
| Reopened  | Defect not fixed, cycle restarts            | QA               | Reassign to developer      |

## Notes

- Some organizations may include additional statuses like **Rejected**, **Duplicate**, or **Deferred**.
- The cycle may vary depending on the project, tool, or methodology.