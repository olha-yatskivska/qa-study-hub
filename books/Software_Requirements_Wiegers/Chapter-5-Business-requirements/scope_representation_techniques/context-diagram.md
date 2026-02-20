# Context diagram

> the Context Diagram is a fundamental tool for defining the project's scope. It provides a high-level view of the system in its environment.
---

## Main Principle
The core principle of a Context Diagram is boundary definition. It treats the entire system as a single "black box" (a single process) and focuses exclusively on how that system interacts with the outside world. It does not show internal logic, data storage, or detailed workflows.

## When to Use It
**Early in the Project:** To reach a consensus with stakeholders on what is "in-scope" and "out-of-scope."

**Stakeholder Identification:** To identify all external users and systems that will interact with your software.

**Interface Clarification:** To map out the high-level data exchange between your system and external entities.

## Main Elements

| Element | Representation | Description |
| --- | --- | --- |
| **The System** | A single circle or bubble | Represents the entire software system under development |
| **External Entities** | External Entities |Rectangles | People, organizations, or other systems that provide data to or receive data from the system |
| **Data Flows** | Labeled Arrows | Represent the movement of information between the system and external entities |

## Recommended Tools
* **General Diagramming:** Lucidchart, Miro, or Microsoft Visio
* **Lightweight/Free:** Draw.io (diagrams.net)
* **Documentation-as-Code:** Mermaid.js or PlantUML (ideal for keeping diagrams inside GitHub/GitLab)
---

## Importance for a Test Analyst
* For a Test Analyst, the Context Diagram is one of the first documents you should review during the requirement analysis phase because:
* Defining Test Scope: It helps you understand the boundaries. If an entity isn't on the diagram, it's likely not your responsibility to test its internal logic, but you must test the connection to it.
* Interface Testing: It highlights every external interface. Each arrow represents a potential integration test case or an API contract that needs validation.
* Identifying Dependencies: It shows which external systems you might need to "mock" or "stub" during testing if those systems are not yet available.
* Data Integrity: By seeing what data enters and leaves the system, you can plan end-to-end scenarios to ensure data isn't corrupted as it crosses the system boundary.

> To view a practical example and the diagram code, proceed to the [Standard Context Diagram (Mermaid)]() section.
 
