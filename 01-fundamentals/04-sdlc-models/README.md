# Module 4: SDLC Delivery Models

## 🌱 Why This Module Matters

Understanding Software Development Life Cycle (SDLC) models isn't just academic—it determines **when and how** you test. Different models require different testing strategies, and understanding these models helps you adapt your QA approach.

This module explores major SDLC models and their implications for testing. The goal is to understand **how development approach affects testing strategy**.

---

## 📚 Learning Objectives

By the end of this module, you will understand:

1. **Waterfall Model** - Sequential development
2. **V-Model** - Verification and validation parallel
3. **Agile Model** - Iterative, adaptive development
4. **Testing Implications** - How each model affects testing
5. **Choosing the Right Model** - Context matters

---

## 🧩 Conceptual Overview

### Waterfall Model

**What it is**: Sequential phases, each must complete before next begins.

**Phases**:
```
Requirements → Design → Implementation → Testing → Deployment → Maintenance
```

**Characteristics**:
- Linear, sequential
- Each phase has deliverables
- Changes are expensive (hard to go back)
- Testing happens late in cycle

**Testing perspective**:
- ✅ Clear phases, easy to plan
- ✅ Well-defined requirements
- ❌ Testing happens late (defects found late)
- ❌ Changes are expensive
- ❌ May not meet user needs (requirements set early)

**When to use**: Well-understood requirements, stable projects, regulated industries.

**Testing strategy**: 
- Plan tests during requirements/design
- Execute during testing phase
- Focus on verification (meets requirements)

---

### V-Model

**What it is**: Each development phase has corresponding testing phase.

**Structure**:
```
Requirements → System Testing
    Design → Integration Testing
Implementation → Unit Testing
```

**Characteristics**:
- Testing planned from start
- Each phase verified before moving on
- Parallel development and testing activities
- Still sequential overall

**Testing perspective**:
- ✅ Testing planned early
- ✅ Each level has corresponding tests
- ✅ Verification at each stage
- ❌ Still sequential, changes expensive
- ❌ May be overkill for simple projects

**When to use**: Safety-critical systems, regulated industries, when verification is critical.

**Testing strategy**:
- Plan tests parallel to development
- Test at each level (unit, integration, system)
- Focus on verification and validation

---

### Agile Model

**What it is**: Iterative, collaborative, adaptive development.

**Core values** (Agile Manifesto):
- Individuals and interactions over processes
- Working software over documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

**Characteristics**:
- Iterative (sprints/iterations)
- Collaborative (cross-functional teams)
- Adaptive (responds to change)
- Customer-focused (frequent feedback)

**Testing perspective**:
- ✅ Testing integrated throughout
- ✅ Continuous feedback
- ✅ Testers part of team
- ✅ Test-driven development possible
- ✅ Early and frequent testing
- ❌ Requires discipline
- ❌ Can be chaotic without structure

**When to use**: Rapidly changing requirements, customer-focused projects, most modern software.

**Testing strategy**:
- Test continuously in every sprint
- Test early (TDD, BDD)
- Collaborate with developers
- Focus on working software
- Adapt to changes

**Key insight**: In Agile, testing isn't a phase—it's **integrated throughout**.

---

### Comparing Models

| Aspect | Waterfall | V-Model | Agile |
|--------|-----------|---------|-------|
| **Flexibility** | Low | Low | High |
| **Testing Timing** | Late | Parallel | Continuous |
| **Change Cost** | High | High | Low |
| **Documentation** | Heavy | Medium | Light |
| **Customer Feedback** | Late | Late | Continuous |
| **Best For** | Stable, regulated | Critical systems | Dynamic, customer-focused |

---

### Testing Implications

**Waterfall**:
- Test planning during requirements
- Test execution during testing phase
- Focus on requirements verification
- Formal test documentation

**V-Model**:
- Test planning parallel to development
- Test execution at each level
- Focus on verification and validation
- Traceability important

**Agile**:
- Test planning in each sprint
- Test execution continuously
- Focus on working software
- Lightweight documentation

**Key principle**: Adapt your testing approach to the development model.

---

## 🎯 Key Takeaways

1. **SDLC models determine testing strategy** - Different models, different approaches
2. **Waterfall tests late** - Sequential, formal
3. **V-Model tests parallel** - Verification at each level
4. **Agile tests continuously** - Integrated, adaptive
5. **Context matters** - Choose model (and testing approach) based on project

---

## 📝 Exercises

See `exercises/` folder for hands-on practice.

---

## 🔗 Connections to Other Modules

- **Module 5**: Agile frameworks (Scrum, Kanban) detail Agile implementation
- **Module 6**: Test planning adapts to SDLC model
- **Module 15**: Automation strategy depends on model

---

**Reflection Question**: How does your project's SDLC model affect how you plan and execute testing?

