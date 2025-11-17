# Module 22: CI/CD Pipelines

## 🌱 Why This Module Matters

CI/CD (Continuous Integration/Continuous Deployment) isn't just about automation—it's about **integrating testing into the development workflow**. Understanding CI/CD helps you ensure quality is built in, not tested in.

This module explores CI/CD from a QA perspective: how testing fits into pipelines, what tools are available, and how to design effective CI/CD for quality.

---

## 📚 Learning Objectives

By the end of this module, you will understand:

1. **CI/CD Concepts** - What and why
2. **Continuous Integration** - Automated builds and tests
3. **Continuous Deployment** - Automated releases
4. **Testing in CI/CD** - Where tests fit
5. **CI/CD Tools** - Jenkins, GitLab CI, GitHub Actions
6. **Pipeline Design** - Effective test pipelines

---

## 🧩 Conceptual Overview

### What is CI/CD?

**CI (Continuous Integration)**:
- Developers integrate code frequently
- Automated build and test on each integration
- Early detection of integration issues
- "Build fast, fail fast"

**CD (Continuous Deployment/Delivery)**:
- **Continuous Delivery**: Code is always deployable
- **Continuous Deployment**: Code is automatically deployed
- Automated deployment process
- Fast, reliable releases

**Key insight**: CI/CD makes quality **automatic**, not manual.

---

### Continuous Integration

**Workflow**:
1. Developer commits code
2. CI server detects change
3. Automated build
4. Automated tests run
5. Report results
6. Deploy if tests pass (CD)

**Benefits**:
- ✅ Early bug detection
- ✅ Fast feedback
- ✅ Reduced integration issues
- ✅ Confidence in code

**Testing in CI**:
- Unit tests (fast, run on every commit)
- Integration tests (medium speed)
- E2E tests (slower, may run on schedule)
- Linting, code quality checks

**Key principle**: Fast feedback loop. Fail fast, fix fast.

---

### Continuous Deployment

**What it is**: Automatically deploying code that passes tests.

**Stages**:
1. **Build**: Compile, package
2. **Test**: Run test suite
3. **Deploy to Staging**: Test environment
4. **Deploy to Production**: Live environment

**Testing at each stage**:
- **Build stage**: Compilation, linting
- **Test stage**: Unit, integration, E2E
- **Staging**: Smoke tests, sanity checks
- **Production**: Monitoring, health checks

**Safety**:
- Automated rollback on failure
- Canary deployments (gradual rollout)
- Feature flags (control releases)

---

### Testing in CI/CD

**Test Pyramid in CI/CD**:
```
        /\
       /E2E\      ← Few, slow, run on schedule
      /------\
     /Integration\ ← Some, medium, run on commits
    /------------\
   /    Unit      \ ← Many, fast, run on every commit
  /----------------\
```

**Strategy**:
- **Unit tests**: Every commit, fast feedback
- **Integration tests**: Every commit or PR
- **E2E tests**: On schedule or PR, not every commit
- **Performance tests**: On schedule
- **Security scans**: On schedule or PR

**Key principle**: Balance speed and coverage. Fast tests run frequently, slow tests run strategically.

---

### CI/CD Tools

**Jenkins**:
- Open-source, extensible
- Plugin ecosystem
- Self-hosted
- Good for complex pipelines

**GitLab CI**:
- Integrated with GitLab
- YAML-based configuration
- Built-in Docker support
- Good for GitLab projects

**GitHub Actions**:
- Integrated with GitHub
- YAML-based
- Marketplace of actions
- Good for GitHub projects

**CircleCI**:
- Cloud-based
- Fast builds
- Good for startups

**Azure DevOps**:
- Microsoft ecosystem
- Integrated tooling
- Good for .NET projects

**Choosing tool**: Depends on your stack, preferences, and requirements.

---

### Pipeline Design

**Effective pipeline structure**:

1. **Build Stage**:
   - Compile code
   - Run linters
   - Check code quality
   - Fast feedback

2. **Test Stage**:
   - Unit tests
   - Integration tests
   - Code coverage
   - Fail fast

3. **Deploy to Staging**:
   - Deploy to test environment
   - Run smoke tests
   - Run E2E tests

4. **Deploy to Production**:
   - Deploy to production
   - Health checks
   - Monitoring

**Best practices**:
- Fast feedback (fail early)
- Parallel execution (speed up)
- Conditional stages (skip if not needed)
- Artifact management (save test results)
- Notifications (alert on failure)

---

### QA Role in CI/CD

**QA Engineers**:
- Design test strategy for CI/CD
- Create automated tests
- Monitor test results
- Maintain test infrastructure
- Improve pipeline efficiency
- Ensure quality gates

**Key activities**:
- Write testable code (if doing TDD)
- Create automation tests
- Review pipeline configuration
- Analyze test results
- Improve test reliability
- Balance speed and coverage

---

## 🎯 Key Takeaways

1. **CI/CD automates quality** - Tests run automatically
2. **Fast feedback is key** - Fail fast, fix fast
3. **Test pyramid applies** - Fast tests frequently, slow tests strategically
4. **Tools vary** - Choose based on needs
5. **Pipeline design matters** - Structure affects effectiveness
6. **QA is integral** - Not separate from CI/CD

---

## 📝 Exercises

See `exercises/` folder for hands-on practice.

---

## 🔗 Connections to Other Modules

- **Module 12**: Automation tests run in CI/CD
- **Module 21**: Version control triggers CI/CD
- **Module 23**: Test results feed into test management

---

**Reflection Question**: How does CI/CD change the role of QA from "testing after" to "quality throughout"?

