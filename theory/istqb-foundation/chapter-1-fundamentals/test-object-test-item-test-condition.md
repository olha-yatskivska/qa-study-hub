# Work Products, Test Objects & Items

This summary covers the fundamental concepts of work products and the hierarchical relationship between the test basis, test objects, and test items according to ISTQB Foundation v4.0.

---

| Concept | **Test Object** | **Test Item** |
| :--- | :--- | :--- |
| **Definition** | The work product to be tested (the whole system/component). | A specific, identified part of the test object. |
| **Focus** | Overall quality and system-level readiness. | Isolation and verification of a specific feature or unit. |
| **Scope** | Typically Higher-level (System, Acceptance). | Typically Lower-level (Unit, Component, Integration). |
| **Traceability** | Mapped to **Test Basis** (High-level requirements). | Mapped to **Test Conditions** & **Test Cases**. |
| **Example** | The entire Mobile Banking Application. | The Biometric (FaceID) login module. |

---

## 🏗️ What is a Work Product? 

A **Work Product** is any artifact, outcome, or output material created during the Software Development Life Cycle (SDLC). 
> **Key Rule:** Test Object is the work product to be tested.

### 📋 Classification of Work Products

#### 1. Business-Oriented (The "Test Basis")
*Created during analysis/design. We use these for Static Testing (Reviews).*
* **Requirements:** BRD, URS, User Stories, Acceptance Criteria.
* **Design:** Business Process Models (BPMN diagrams), Product Risk Analysis.

#### 2. Development-Specific
*Created by developers. These are the items we evaluate during Dynamic Testing.*
* **Code:** Source Code, Executable Builds.
* **Infrastructure:** System Architecture docs, Deployment scripts, Unit Tests.

#### 3. Testing-Specific (Testware)
*Artifacts created by QA for planning, execution, and control.*
* **Planning:** Test Plan, Test Strategy, Test Risk Analysis.
* **Design/Implementation:** Test Conditions, Test Cases, Test Data, Automation Scripts.
* **Reporting:** Execution Logs, Defect Reports, Test Summary Reports (TSR).



---

## 🧪 Practical Examples

| Context | **Test Basis** (The Source) | **Test Object** (The Whole) | **Test Item** (The Part) | **Test Condition** (The Goal) |
| :--- | :--- | :--- | :--- | :--- |
| **E-Commerce** | User Story: "Guest Checkout" | Web Storefront Build | "Pay with PayPal" button | Verify redirection to PayPal login. |
| **Mobile App** | UI/UX Design (Figma) | iOS Banking App v2.1 | FaceID authentication | Verify unlock with a registered face. |
| **Embedded/IoT** | Protocol Specs | Smart Thermostat Firmware | Temperature Sensor driver | Verify reaction to > 30°C. |
| **API/Backend** | OpenAPI/Swagger Docs | Inventory Microservice | `GET /products/{id}` | Verify 404 for non-existent IDs. |

---

## 🔗 The Hierarchical Connection

The relationship between these concepts is defined by **containment** and **traceability**:

#### 1. Scope Decomposition (The "What")
The **Test Object** (e.g., Inventory System) is too big to test at once. We break it down into **Test Items** (e.g., Update Stock function). This allows for precise defect tracking.

#### 2. Traceability (The "Why")
* **Test Cases** verify **Test Items**.
* **Test Items** fulfill the **Test Basis** (Requirements).
* **Test Object** quality is the sum of all verified items.

#### 🎯 Crucial Point for the Test Analyst
When logging a defect, it must be linked to the specific **Test Item** (the component) and the specific version of the **Test Object** (the build). This ensures the development team knows exactly where the fix is needed.

---

##  Hierarchy Visualization

```mermaid
graph TD
    subgraph "Information Sources"
    A[Test Basis: Requirements/Docs]
    end

    subgraph "The Target"
    B[Test Object: The Whole System]
    C[Test Item: Specific Component/Feature]
    B --> C
    end

    subgraph "Testing Artifacts"
    D[Test Condition: What to test]
    E[Test Case: How to test]
    D --> E
    end

    A -.->|Analyzed to derive| D
    C -.->|Mapped to| D
    B -.->|Traceability| A
