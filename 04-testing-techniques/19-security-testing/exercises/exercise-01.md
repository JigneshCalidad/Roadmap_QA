# Exercise 1: Security Testing Practice

## Purpose

These exercises help you develop a **security mindset** and practice security testing techniques. The goal is to understand how to test for security vulnerabilities, not just functionality.

---

## Exercise 1.1: Understanding OWASP Top 10

### Task

Research and understand each OWASP Top 10 item:

1. **For Each Item**:
   - What is it?
   - How does it work?
   - What's the risk?
   - How do you test for it?

2. **Create Test Scenarios**:
   - Write test cases for each
   - Document how to test
   - Note what to look for

3. **Prioritize**:
   - Which are most critical for your context?
   - Which are easiest to test?
   - Which require special tools?

### Reflection

- Why is OWASP Top 10 important?
- How does it guide security testing?
- Which items are most relevant to your projects?

---

## Exercise 1.2: Authentication Testing

### Task

Test authentication on a test application (or imagine one):

1. **Valid Authentication**:
   - Test valid login
   - Test logout
   - Test session management

2. **Invalid Authentication**:
   - Wrong password
   - Non-existent user
   - SQL injection in username/password
   - XSS in input fields

3. **Security Issues**:
   - Can you bypass login?
   - Are passwords encrypted?
   - Do sessions expire?
   - Can you hijack sessions?

4. **Document Findings**:
   - What works?
   - What's vulnerable?
   - What are the risks?

### Reflection

- What makes authentication secure?
- What are common vulnerabilities?
- How do you test authentication thoroughly?

---

## Exercise 1.3: Authorization Testing

### Task

Test authorization (access control):

**Scenario**: Application with different user roles:
- Guest (no login)
- Regular User
- Admin

1. **Test Each Role**:
   - What can each role access?
   - What should each role NOT access?
   - Test accessing unauthorized resources

2. **Common Vulnerabilities**:
   - Direct object reference (change URL to access others' data)
   - Privilege escalation (user accessing admin functions)
   - Missing authorization checks

3. **Test Scenarios**:
   - Login as user, try to access admin URL
   - Try to access another user's data
   - Try to perform admin actions as user

### Reflection

- How is authorization different from authentication?
- What are common authorization flaws?
- How do you test access control?

---

## Exercise 1.4: Input Validation Testing

### Task

Test input validation on forms:

1. **SQL Injection**:
   - Try: `' OR '1'='1` in login
   - Try: `'; DROP TABLE users; --`
   - What happens?
   - Is input sanitized?

2. **XSS (Cross-Site Scripting)**:
   - Try: `<script>alert('XSS')</script>` in input
   - Try: `<img src=x onerror=alert('XSS')>`
   - Does it execute?
   - Is input escaped?

3. **Other Attacks**:
   - Command injection
   - Path traversal (`../../../etc/passwd`)
   - Buffer overflow (very long strings)

4. **Document Results**:
   - What's protected?
   - What's vulnerable?
   - What's the risk?

### Reflection

- Why is input validation critical?
- What happens if validation fails?
- How do you test input validation?

---

## Exercise 1.5: Session Management Testing

### Task

Test session security:

1. **Session Creation**:
   - How are sessions created?
   - Are session IDs predictable?
   - Are they secure (random, long)?

2. **Session Handling**:
   - Do sessions expire?
   - What happens on logout?
   - Can you reuse old sessions?

3. **Session Hijacking**:
   - Can you steal someone's session?
   - Are sessions tied to IP?
   - Are cookies secure (HttpOnly, Secure flags)?

4. **Test Scenarios**:
   - Login, copy session cookie, logout, reuse cookie
   - Check if session expires after inactivity
   - Check if multiple sessions work

### Reflection

- What makes sessions secure?
- What are common session vulnerabilities?
- How do you test session management?

---

## Exercise 1.6: Secrets Management

### Task

Review code or configuration for secrets:

1. **Find Secrets**:
   - API keys in code?
   - Passwords hardcoded?
   - Secrets in config files?
   - Secrets in version control?

2. **Assess Risk**:
   - What secrets are exposed?
   - What's the impact?
   - Who could access them?

3. **Best Practices**:
   - How should secrets be managed?
   - Environment variables?
   - Secret management tools?
   - Encryption?

### Reflection

- Why are hardcoded secrets dangerous?
- How should secrets be managed?
- How do you test for secret exposure?

---

## Exercise 1.7: Security Testing Tools

### Task

Explore security testing tools:

1. **OWASP ZAP**:
   - Download and install
   - Scan a test application
   - Review findings
   - Understand reports

2. **Burp Suite** (if available):
   - Intercept requests
   - Modify and replay
   - Test for vulnerabilities

3. **Browser DevTools**:
   - Inspect cookies
   - Check security headers
   - Monitor network requests

### Reflection

- How do tools help security testing?
- What can tools find automatically?
- What still requires manual testing?
- How do you use tools effectively?

---

## Exercise 1.8: Security Testing Strategy

### Task

Create a security testing strategy:

1. **Threat Modeling**:
   - What are the assets?
   - What are the threats?
   - What are the risks?

2. **Test Planning**:
   - What will you test?
   - How will you test it?
   - What tools will you use?

3. **Test Execution**:
   - Manual security testing
   - Automated scanning
   - Code review (if applicable)

4. **Reporting**:
   - Document vulnerabilities
   - Assess risk
   - Recommend fixes

### Reflection

- How do you approach security testing systematically?
- How does security testing differ from functional testing?
- How do you balance security and functionality?
- How do you communicate security findings?

---

## 🎯 Self-Assessment

After completing these exercises, ask yourself:

1. Do I understand OWASP Top 10?
2. Can I test authentication and authorization?
3. Can I test for common vulnerabilities?
4. Do I understand session security?
5. Can I use security testing tools?
6. Can I create a security testing strategy?

---

## 💡 Key Insights to Carry Forward

- **Security is essential** - Not optional
- **OWASP Top 10 guides testing** - Common vulnerabilities
- **Think like an attacker** - What would you exploit?
- **Tools help, but manual testing needed** - Not everything is automated
- **Security mindset complements testing mindset** - Both are important
- **Context matters** - Security requirements vary
- **Continuous process** - Security testing is ongoing

---

**Next Steps**: Once you understand security testing, integrate it into your overall testing strategy. Security should be part of every test plan.

