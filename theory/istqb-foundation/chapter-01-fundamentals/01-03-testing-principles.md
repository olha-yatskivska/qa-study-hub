# 7 Testing Principles
## 🔍 1. Testing shows the presence, not the absence of defects
* Testing can show that defects are present in the test object, but it cannot prove that there are no defects.
* **Practical view:** Following a defined strategy and coverage level reduces the probability of a user encountering a bug, but never guarantees a 100% bug-free system.

## ♾️ 2. Exhaustive testing is impossible
* Testing everything (all combinations of inputs and preconditions) is not feasible except in trivial cases.
* **Solution:** Use test techniques, prioritization, and risk-based testing to focus efforts where they matter most.

## ⏱️ 3. Early testing saves time and money
* **The Cost of Quality:** Finding bugs early in the SDLC (Software Development Life Cycle) is much cheaper than fixing them in production.
* **Shift-Left Approach:** Start both static testing (reviews of requirements/design) and dynamic testing as soon as possible.

## 🎯 4. Defects cluster together (Pareto Principle)
* A small number of modules usually contain the majority of defects (the 80/20 rule).
* **Risk-based testing:** Focus more effort on these "hotspots."
* **Retro Analysis:** Use sprint statistics to identify high-risk features for future planning.

## 🧴 5. Tests wear out (Pesticide Paradox)
* If the same tests are repeated over and over, they will eventually stop finding new defects.
* **Mitigation:**
* Regularly review and update test cases.
* In automated testing, use randomization (Data-Driven Testing) instead of hardcoded values.
* Write diverse smoke and regression tests to cover different paths.
* High-level checklists instead of detailed test cases where applicable.

## 🗺️ 6. Testing is context-dependent
* Testing is performed differently in different contexts.
* Factors include:
       * Domain (e.g., medical software vs. a simple landing page).
       * Methodology (Agile vs. Waterfall).
       * Customer expectations and market situation.
       * Team seniority and process maturity.

## 💡 7. Absence-of-defects fallacy
* Finding and fixing defects is useless if the system is unusable or doesn't fulfill user needs.
* Validation vs. Verification: It’s not just about "building the thing right" (no bugs), but "building the right thing" (meeting user requirements).

## Importance for a Test Analyst
* **Managing Expectations:** Principle #1 and #7 help you explain why you can't guarantee a bug-free launch and why "no bugs" doesn't always mean "good product."
* **Efficiency:** Principle #2 and #4 justify why you aren't testing everything and why you are focusing on specific complex modules.
* **Strategic Planning:** Principle #3 and #6 allow you to advocate for early involvement in requirements (Shift-Left) and to tailor your test plan based on the specific project context (e.g., a banking app needs more security testing than a blog).
* * 
