# An example of how different stakeholders participate in requirements development

```mermaid
flowchart TD
    %% Define Nodes
    subgraph Corporate_Roles [Corporate Roles]
        direction TB
        A[/"Business<br>Need"\]
    end

    subgraph Commercial_Roles [Commercial Roles]
        direction TB
        B[/"Market Need or<br>Product Concept"\]
    end

    C([Business<br>Requirements])
    D([User<br>Requirements])
    E([Functional<br>Requirements])
    F[Developer, Tester]

    %% Define Connections/Edges
    A -->|Manager| C
    B -->|Marketing| C
    
    C -->|Business Analyst<br>and User Reps| D
    C -->|Product Manager| D
    
    D -->|Business Analyst| E
    D -->|Business Analyst or<br>Product Manager| E
    
    E --> F

    %% Styling to mimic the image colors roughly
    style A fill:#f0f4f8,stroke:#333,stroke-width:1px
    style B fill:#f0f4f8,stroke:#333,stroke-width:1px
    style C fill:#fff9c4,stroke:#333,stroke-width:1px
    style D fill:#fff9c4,stroke:#333,stroke-width:1px
    style E fill:#fff9c4,stroke:#333,stroke-width:1px
```



## This diagram is specifically important for a Test Analyst:

* **Defining the Test Basis:** This flow clearly identifies the documents that serve as the "Test Basis" (the source of truth for testing):
   * UAT (User Acceptance Testing): Is based on the User Requirements node.
   * System Testing: Is primarily based on the Functional Requirements node.

* **Traceability:** This hierarchy demonstrates the "Golden Thread" of traceability. A Test Analyst must ensure every test case written (at the bottom level) can be traced back up to a specific User Requirement and, ultimately, a Business Need. If a test fails, you use this flow to determine if the software is broken or if the requirement was misunderstood upstream.

* **The "Waterfall" Risk:** The diagram shows the Tester appearing only at the very end (the bottom arrow). Fora modern Test Analyst, this highlights a risk area. You should advocate to be involved earlier - ideally during the review of "User Requirements" - to prevent defects before they reach the "Functional Requirements" stage (the concept of "Shift Left").
