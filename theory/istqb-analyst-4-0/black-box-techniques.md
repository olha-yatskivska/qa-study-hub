# Black-Box Techniques


  ## Data-Based Test Techniques

  * Domain Testing

       * equivalence partitions
       * boundary values analysis

   * Combinatorial Testing

       * pairwise
       * classification tree

   * Random Testing

       * guided random
       * adaptive random

  ## Behavior-Based Test Techniques

  * CRUD Testing
  * State Transition Testing
  * Scenario-Based Testing


  ##  Rule-Based Test Techniques

   * Decision Table Testing
   * Metamorphic Testing

```mermaid
graph TD
    %% Main Header
    Main[Black-Box Techniques]
    
    %% --- DATA-BASED BRANCH ---
    Main --> Data[<b>Data-Based Test Techniques</b>]
    
    Data --> DT[Domain Testing]
    DT --> EP[Equivalence Partitions]
    DT --> BVA[Boundary Values Analysis]
    
    Data --> CT[Combinatorial Testing]
    CT --> PW[Pairwise]
    CT --> CTA[Classification Tree]
    
    Data --> RT[Random Testing]
    RT --> GR[Guided Random]
    RT --> AR[Adaptive Random]

    %% --- BEHAVIOR-BASED BRANCH ---
    Main --> Beh[<b>Behavior-Based Test Techniques</b>]
    
    Beh --> CRUD[CRUD Testing]
    Beh --> STT[State Transition Testing]
    Beh --> SBT[Scenario-Based Testing]

    %% --- RULE-BASED BRANCH ---
    Main --> Rule[<b>Rule-Based Test Techniques</b>]
    
    Rule --> DTT[Decision Table Testing]
    Rule --> MT[Metamorphic Testing]

    %% Minimalist Styling for Readability
    style Main fill:#fff,stroke:#000,stroke-width:2px
    style Data fill:#f9f9f9,stroke:#333
    style Beh fill:#f9f9f9,stroke:#333
    style Rule fill:#f9f9f9,stroke:#333
    
    %% Link styling to make them look cleaner
    linkStyle default stroke:#555,stroke-width:1px,fill:none
