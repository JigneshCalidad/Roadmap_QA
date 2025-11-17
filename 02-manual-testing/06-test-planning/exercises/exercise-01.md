# Exercise 1: Test Planning Practice

## Purpose

These exercises help you develop test planning skills. The goal is to understand test planning as **strategic thinking**, not just documentation. You'll practice creating test plans and understanding the decisions behind them.

---

## Exercise 1.1: Understanding Requirements

### Task

You're planning tests for a user registration feature:

**Requirements**:
- User can register with email and password
- Email must be valid format
- Password must be at least 8 characters
- User receives confirmation email
- User can login after registration

1. **Analyze Requirements**:
   - What needs to be tested?
   - What are the acceptance criteria?
   - What's missing or unclear?

2. **Identify Testable Items**:
   - List all testable features
   - List all testable rules
   - List all integrations

3. **Questions to Ask**:
   - What questions do you have?
   - What clarifications do you need?
   - What assumptions are you making?

### Reflection

- How do requirements quality affect test planning?
- What happens if requirements are unclear?
- How do you handle missing requirements?

---

## Exercise 1.2: Defining Test Strategy

### Task

Create a test strategy for an e-commerce website:

**Features**:
- User registration/login
- Product browsing
- Shopping cart
- Payment processing
- Order management

1. **Testing Levels**:
   - What levels will you test at?
   - Unit? Integration? System? Acceptance?
   - Why each level?

2. **Testing Types**:
   - What types of testing?
   - Functional? Performance? Security? Usability?
   - Why each type?

3. **Testing Approach**:
   - Manual vs. automated?
   - Black box vs. white box?
   - Risk-based vs. exhaustive?
   - Justify your choices

4. **Tools and Techniques**:
   - What tools will you use?
   - What test design techniques?
   - Why?

### Reflection

- How does strategy guide your testing?
- What factors influence strategy?
- How do you balance different approaches?

---

## Exercise 1.3: Defining Test Scope

### Task

You have limited time and resources. Define scope:

**All Features**:
- Core features (must test)
- Nice-to-have features (test if time)
- Edge cases (test if time)
- Legacy features (maintain)

1. **In Scope**:
   - What will you definitely test?
   - Why?
   - How thoroughly?

2. **Out of Scope**:
   - What won't you test?
   - Why?
   - What are the risks?

3. **Conditional Scope**:
   - What will you test if time permits?
   - What's the priority order?
   - How do you decide?

4. **Document Decisions**:
   - Write scope document
   - Justify inclusions/exclusions
   - Set expectations

### Reflection

- How do you make scope decisions?
- How do you communicate scope?
- What happens when stakeholders want more?
- How do you handle scope creep?

---

## Exercise 1.4: Risk-Based Planning

### Task

Assess risk for each feature:

**Features**:
1. User login
2. Product search
3. Shopping cart
4. Payment processing
5. Product reviews
6. User profile
7. Admin dashboard

1. **Assess Each Feature**:
   - Probability of failure (1-5)
   - Impact if it fails (1-5)
   - Risk = Probability × Impact

2. **Prioritize**:
   - Rank by risk
   - Which get most testing?
   - Which get least?

3. **Create Test Plan**:
   - High risk: Extensive testing
   - Medium risk: Moderate testing
   - Low risk: Minimal testing
   - Document your plan

### Reflection

- How does risk assessment help prioritize?
- What factors influence probability and impact?
- How do you justify risk-based decisions?
- What if stakeholders disagree with risk assessment?

---

## Exercise 1.5: Test Estimation

### Task

Estimate testing effort:

**Project**: E-commerce website with 10 features

1. **Break Down Work**:
   - Test planning
   - Test case creation
   - Test execution
   - Defect reporting
   - Retesting
   - Documentation

2. **Estimate Each Task**:
   - How long for each?
   - What factors affect time?
   - Use three-point estimation (optimistic, pessimistic, most likely)

3. **Account for Unknowns**:
   - What could go wrong?
   - How much buffer do you need?
   - What are the risks to schedule?

4. **Create Estimate**:
   - Total effort
   - Timeline
   - Resources needed
   - Assumptions and risks

### Reflection

- What makes estimation difficult?
- How do you handle uncertainty?
- How do you communicate estimates?
- What happens when estimates are wrong?

---

## Exercise 1.6: Entry and Exit Criteria

### Task

Define criteria for a release:

1. **Entry Criteria** (When to start testing):
   - What must be ready?
   - Requirements? Environment? Data? Build?
   - How do you verify each?

2. **Exit Criteria** (When testing is complete):
   - What must be true?
   - All tests passed? Defects fixed? Coverage achieved?
   - How do you measure?

3. **Create Checklist**:
   - Entry criteria checklist
   - Exit criteria checklist
   - Who verifies?

### Reflection

- Why are entry/exit criteria important?
- What happens if you start testing too early?
- What happens if you don't have clear exit criteria?
- How do you handle pressure to release?

---

## Exercise 1.7: Complete Test Plan

### Task

Create a complete test plan for a feature:

**Feature**: User Registration

1. **Test Plan Sections**:
   - Introduction/Overview
   - Test Strategy
   - Test Scope (in/out)
   - Test Approach
   - Test Environment
   - Test Data
   - Entry/Exit Criteria
   - Risks and Mitigation
   - Schedule and Resources

2. **Fill Each Section**:
   - Be specific
   - Justify decisions
   - Make it actionable

3. **Review**:
   - Is it complete?
   - Is it clear?
   - Can someone else execute it?

### Reflection

- What makes a good test plan?
- How detailed should it be?
- Who is the audience?
- How do you keep it maintainable?

---

## 🎯 Self-Assessment

After completing these exercises, ask yourself:

1. Can I create a test strategy?
2. Can I define test scope?
3. Can I assess risk and prioritize?
4. Can I estimate testing effort?
5. Can I define entry/exit criteria?
6. Can I create a complete test plan?

---

## 💡 Key Insights to Carry Forward

- **Test planning is strategic** - Not just documentation
- **Strategy guides approach** - High-level direction
- **Scope sets boundaries** - What to test, what not to
- **Risk-based planning prioritizes** - Focus where it matters
- **Estimation is prediction** - Include buffer
- **Entry/exit criteria provide boundaries** - Clear start and end
- **Test plan is a living document** - Update as needed

---

**Next Steps**: Once you can create test plans, move to Module 7: Test Cases and Scenarios to learn how to design effective test cases.

