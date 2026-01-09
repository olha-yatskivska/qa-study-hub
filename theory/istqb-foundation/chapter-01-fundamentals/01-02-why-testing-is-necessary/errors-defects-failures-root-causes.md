🐞 Errors, Defects, and Failures

## 👤 Error (Mistake)
* **Definition:** A human action that produces an incorrect result.
* **Examples:**
    * A developer misinterprets a requirement.
    * A designer uses the wrong color code.
    * A test analyst writes an incorrect test step.
## 📄Defects (Faults, Bugs)
* **Definition:** An imperfection or deficiency in a work product where it does not meet its requirements or specifications.
* **Note:** A defect is "latent" (hidden) until it is triggered.
--- 
 > ⚠️ Key Concept: Not all defects lead to failures (e.g., a typo in a comment or a hidden piece of dead code, wrong text or name of the button, wrong translate for user; wrong colour)
---
## 💥 Failure
* **Definition:** An event in which a component or system does not perform a required function within specified limits.
* **Characteristics:** Occurs only during execution (Dynamic).
* **Causes:** Failures can be caused by defects, but also by environmental conditions (radiation, magnetic fields, etc.).
* **Examples:**
   * unexpected error on the screen
   * error message
   * wrong calculations
   * can't open the page
---
##  🚩 Factors leading to Errors 
  * time pressure
  * complexity of work products (legacy)
  * processes
  * infrastucture or interactions
  * human falibility (tired)
  * lack adequate training
  * miscommunication between project participants
---
🌳 Root Cause
The fundamental source of a problem. If it is identified and removed, the occurrence of similar errors and defects in the future is prevented.

Example: If an error occurs due to a lack of adequate training, the Root Cause is a deficiency in the personnel management or onboarding process.
---
```mermaid
graph TD
    A[Root Cause] --> B(Error, Mistake (Moment))
    B --> C[Bug, Defect, Fault (Static)]
    C --> D{Failure (Dynamic, Event)}
```
 
