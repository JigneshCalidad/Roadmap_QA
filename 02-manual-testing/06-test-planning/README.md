# Module 6: Test Planning and Design

## 🌱 Why This Module Matters

Test planning isn't just documentation—it's **strategic thinking** about how to ensure quality. A good test plan guides your testing efforts, helps you communicate with stakeholders, and ensures you don't miss critical areas.

This module explores test planning from an INFJ perspective: understanding the **why** behind planning, not just the **what** to document.

---

## 📚 Learning Objectives

By the end of this module, you will understand:

1. **What is Test Planning** - Purpose and scope
2. **Test Planning Process** - How to create a plan
3. **Test Strategy** - High-level approach
4. **Test Scope** - What to test (and what not to)
5. **Risk-Based Planning** - Prioritizing effort
6. **Test Estimation** - Planning resources and time

---

## 🧩 Conceptual Overview

### What is Test Planning?

**Definition**: Document that describes the **scope, approach, resources, and schedule** of testing activities.

**Purpose**:
- **Guide testing efforts** - What to do, when, how
- **Communicate** - Share plan with team/stakeholders
- **Estimate** - Plan resources and time
- **Track progress** - Measure against plan
- **Manage risk** - Identify and address risks

**Key insight**: Test planning is **strategic thinking**, not just paperwork.

---

### Test Planning Process

**Steps**:

1. **Understand Requirements**
   - What needs to be tested?
   - What are the acceptance criteria?
   - What are the constraints?

2. **Define Test Strategy**
   - High-level approach
   - Testing levels
   - Testing types
   - Tools and techniques

3. **Define Test Scope**
   - What's in scope?
   - What's out of scope?
   - Why?

4. **Identify Risks**
   - What could go wrong?
   - What's high risk?
   - How to mitigate?

5. **Estimate Effort**
   - How long will testing take?
   - What resources are needed?
   - What's the schedule?

6. **Define Entry/Exit Criteria**
   - When to start testing?
   - When is testing complete?

7. **Plan Test Environment**
   - What environment is needed?
   - What data is needed?
   - What tools are needed?

---

### Test Strategy

**What it is**: High-level approach to testing.

**Components**:

1. **Testing Levels**:
   - Unit testing
   - Integration testing
   - System testing
   - Acceptance testing

2. **Testing Types**:
   - Functional testing
   - Non-functional testing
   - Security testing
   - Performance testing

3. **Testing Approach**:
   - Manual vs. automated
   - Black box vs. white box
   - Risk-based vs. exhaustive

4. **Tools and Techniques**:
   - Test design techniques
   - Automation tools
   - Test management tools

**Key principle**: Strategy should align with project goals and constraints.

---

### Test Scope

**What it is**: Defining what will and won't be tested.

**In Scope**:
- Features to be tested
- Testing types
- Testing levels
- Platforms/environments

**Out of Scope**:
- Features not tested (and why)
- Testing types not performed
- Platforms not covered
- Known limitations

**Why scope matters**:
- Sets expectations
- Prevents scope creep
- Helps prioritize
- Manages resources

**Example**: 
- **In scope**: Core functionality, critical paths, main browsers
- **Out of scope**: Edge cases (low priority), old browsers, performance (separate project)

---

### Risk-Based Planning

**Concept**: Prioritize testing based on risk.

**Risk = Probability × Impact**

**High-risk areas** get more testing:
- Critical functionality
- Complex code
- Frequently used features
- Areas with history of defects
- Recently changed code

**Low-risk areas** get less testing:
- Simple, stable features
- Rarely used features
- Well-tested areas

**Benefits**:
- Efficient use of resources
- Focus on what matters
- Better ROI

**Example**: E-commerce site
- **High risk**: Payment, authentication (extensive testing)
- **Medium risk**: Product search, cart (moderate testing)
- **Low risk**: About page, help (minimal testing)

---

### Test Estimation

**What it is**: Predicting effort, time, and resources needed.

**Techniques**:

1. **Expert Judgment**: Based on experience
2. **Analogous Estimation**: Based on similar projects
3. **Bottom-Up**: Estimate tasks, sum up
4. **Three-Point Estimation**: Optimistic, pessimistic, most likely

**Factors to consider**:
- Test case count
- Complexity
- Test environment setup
- Defect fixing and retesting
- Documentation
- Buffer for unknowns

**Challenges**:
- Requirements may change
- Defects found affect schedule
- Dependencies on development
- Unknown unknowns

**Key principle**: Estimation is **prediction**, not promise. Include buffer.

---

### Entry and Exit Criteria

**Entry Criteria** (When to start testing):
- Requirements are stable
- Test environment is ready
- Test data is available
- Build is available
- Test cases are ready

**Exit Criteria** (When testing is complete):
- All planned tests executed
- Critical defects fixed
- Risk is acceptable
- Test coverage achieved
- Stakeholder approval

**Purpose**: Clear boundaries prevent premature testing and ensure completion.

---

## 🎯 Key Takeaways

1. **Test planning is strategic** - Not just documentation
2. **Strategy guides approach** - High-level direction
3. **Scope sets boundaries** - What to test, what not to
4. **Risk-based planning prioritizes** - Focus where it matters
5. **Estimation is prediction** - Include buffer
6. **Entry/exit criteria provide boundaries** - Clear start and end

---

## 📝 Exercises

See `exercises/` folder for hands-on practice.

---

## 🔗 Connections to Other Modules

- **Module 1**: Planning applies QA principles
- **Module 2**: Risk-based thinking from tester mindset
- **Module 4**: Planning adapts to SDLC model
- **Module 7**: Test cases implement the plan

---

**Reflection Question**: How does thoughtful test planning make your testing more effective and efficient?

