# Module 19: Security Testing

## 🌱 Why This Module Matters

Security testing isn't optional—it's **essential**. In an era of data breaches and cyber attacks, ensuring software security protects users, businesses, and reputations.

This module explores security testing from a QA perspective: understanding threats, testing for vulnerabilities, and ensuring software is secure. The goal is to develop a **security mindset** alongside your testing mindset.

---

## 📚 Learning Objectives

By the end of this module, you will understand:

1. **Security Testing Basics** - What and why
2. **OWASP Top 10** - Common vulnerabilities
3. **Authentication & Authorization** - Access control
4. **Attack Vectors** - How systems are attacked
5. **Vulnerability Scanning** - Finding security issues
6. **Secrets Management** - Protecting sensitive data

---

## 🧩 Conceptual Overview

### What is Security Testing?

**Definition**: Testing to identify vulnerabilities and ensure software is secure.

**Goals**:
- **Confidentiality**: Data is protected
- **Integrity**: Data isn't tampered with
- **Availability**: System is accessible when needed
- **Authentication**: Users are who they claim
- **Authorization**: Users can only access allowed resources

**Key insight**: Security testing is about **finding vulnerabilities before attackers do**.

---

### OWASP Top 10

**What it is**: Top 10 most critical web application security risks.

**Current Top 10** (2021):
1. **Broken Access Control** - Users access unauthorized resources
2. **Cryptographic Failures** - Sensitive data exposure
3. **Injection** - SQL, NoSQL, Command injection
4. **Insecure Design** - Security flaws in design
5. **Security Misconfiguration** - Default/insecure configs
6. **Vulnerable Components** - Outdated dependencies
7. **Authentication Failures** - Weak authentication
8. **Software and Data Integrity** - CI/CD pipeline security
9. **Security Logging Failures** - Insufficient logging
10. **SSRF** - Server-Side Request Forgery

**Testing perspective**: Each represents a category of vulnerabilities to test for.

**Example**: Injection attacks
- SQL Injection: `' OR '1'='1` in login field
- XSS: `<script>alert('XSS')</script>` in input field
- Command Injection: `; rm -rf /` in file upload

---

### Authentication & Authorization

**Authentication**: "Who are you?"
- Verifying user identity
- Login, password, 2FA
- Session management

**Authorization**: "What can you do?"
- Permissions and access control
- Role-based access (admin, user, guest)
- Resource-level permissions

**Testing**:
- **Authentication**: Test login, password strength, session expiry
- **Authorization**: Test access control, privilege escalation, unauthorized access

**Common issues**:
- Weak passwords accepted
- Sessions don't expire
- Users can access admin functions
- Direct object references (change URL to access others' data)

---

### Attack Vectors

**What they are**: Ways attackers exploit vulnerabilities.

**Common vectors**:
1. **Input Validation**: Malicious input
2. **Authentication Bypass**: Weak login
3. **Session Hijacking**: Stolen sessions
4. **SQL Injection**: Database attacks
5. **XSS**: Script injection
6. **CSRF**: Cross-site request forgery
7. **File Upload**: Malicious files
8. **API Attacks**: Unauthorized API access

**Testing approach**: Think like an attacker. What would you try?

---

### Vulnerability Scanning

**What it is**: Automated tools that scan for known vulnerabilities.

**Types**:
- **Static Analysis (SAST)**: Scan source code
- **Dynamic Analysis (DAST)**: Scan running application
- **Dependency Scanning**: Check libraries for vulnerabilities
- **Container Scanning**: Scan Docker images

**Tools**:
- OWASP ZAP
- Burp Suite
- Snyk
- SonarQube

**Limitations**: Tools find known patterns, not all vulnerabilities. Manual testing still needed.

---

### Secrets Management

**What it is**: Protecting sensitive data (passwords, API keys, tokens).

**Best practices**:
- Never hardcode secrets
- Use environment variables
- Use secret management tools (Vault, AWS Secrets Manager)
- Rotate secrets regularly
- Don't commit secrets to Git

**Testing**:
- Verify secrets aren't in code
- Check environment variables are used
- Verify secrets are encrypted
- Test secret rotation

**Common mistakes**:
- Secrets in code repositories
- Default passwords
- Secrets in logs
- Weak encryption

---

### Security Testing Approach

**1. Threat Modeling**:
- Identify assets
- Identify threats
- Assess risks
- Plan tests

**2. Test Planning**:
- Security test cases
- Attack scenarios
- Tools needed
- Access requirements

**3. Test Execution**:
- Manual security testing
- Automated scanning
- Penetration testing (if applicable)
- Code review

**4. Reporting**:
- Document vulnerabilities
- Risk assessment
- Remediation recommendations

---

## 🎯 Key Takeaways

1. **Security is essential** - Not optional
2. **OWASP Top 10 guides testing** - Common vulnerabilities
3. **Authentication ≠ Authorization** - Both must be tested
4. **Think like an attacker** - What would you exploit?
5. **Tools help, but manual testing needed** - Not everything is automated
6. **Secrets must be protected** - Never hardcode

---

## 📝 Exercises

See `exercises/` folder for hands-on practice.

---

## 🔗 Connections to Other Modules

- **Module 2**: Security mindset builds on tester mindset
- **Module 13**: API security is part of backend testing
- **Module 18**: Security affects performance

---

**Reflection Question**: How does a security mindset complement your testing mindset?

