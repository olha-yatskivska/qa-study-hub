
# ⚖️ Verification vs Validation

This summary focuses on the difference between building the product right and building the right product, illustrating why "bug-free" software can still fail.

---


| Feature | **Verification** | **Validation** |
| :--- | :--- | :--- |
| **Main Question** | "Are we building the product **right**?" | "Are we building the **right** product?" |
| **Focus** | Conformance to **specified requirements**. | Fulfillment of **user/stakeholder needs**. |
| **Target** | Technical specifications & Design docs. | The operational environment & End-users. |
| **Evaluation** | Are we following the plan? | Does the plan actually solve the problem? |
| **Testing Principles** | Early testing saves time and money | [Absence-of-Defect Fallacy](#-principle-absence-of-defects-fallacy) |
| **Testing Objectives** | Verifying whether specified requirements have been fulfilled | Validating whether the test object is complete and works as expected by the [Stakeholders](#-stakeholders-who-are-they-and-why-do-they-care) |
| **Stakeholders** | Internal Stakeholders | External Stakeholders |

---

## ⚠️ Principle: Absence-of-Defects Fallacy
> **Definition:** It is a misconception to expect that software verification will ensure the success of a system. 
> Even with 0 bugs found, the system may still fail if it doesn't fulfill business goals.

---

## 👥 Stakeholders : Who are they and why do they care?

#### Internal Stakeholders (The Team)
* **Developers:** Need to know if their code works and where it fails.
* **Business Analysts (BAs):** Want to ensure the software matches the requirements they gathered.
* **Product Owners (POs) / Project Managers:** Need information to decide if the product is ready for release.

#### External Stakeholders (The Business & Users)
* **End-Users:** Want a product that is easy to use and solves their problems (e.g., your Farmer or 55+ user).
* **Customers (The ones paying):** Care about business goals and return on investment (ROI).
* **Regulatory Bodies:** Care about compliance (laws, security standards, GDPR).

--- 

### 💡 Contextual Examples 

#### 🚜 Case 1: The "Fuel-less" Petrol Site (Validation Failure)
* **The Situation:** A petrol management site built for farmers.
* **Verification:** Passed. The code is clean, the database is fast, and it matches every technical bullet point in the specs.
* **Validation:** **FAILED**. Due to a misunderstanding of the farmer's daily workflow, the system doesn't actually help them get petrol in the field.
* **Result:** The software is technically perfect but provides **zero value**.

#### 👴 Case 2: UI for 55+ Users (Context Failure)
* **The Situation:** A modern app developed with "hype" technologies and minimalist design (tiny fonts, complex gestures).
* **Verification:** Passed. All UI elements work according to the design mockups.
* **Validation:** **FAILED**. The target audience (users 55+) finds the interface unusable due to low readability and non-intuitive navigation.
* **Result:** High technical quality, but **zero accessibility**.

#### ⌛ Case 3: The "Hype" Trap
* **The Situation:** Focusing on building exactly what was requested years ago using outdated or overly complex "hype" tech.

