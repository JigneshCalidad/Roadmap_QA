# Exercise 1: Testing Approaches in Practice

## Purpose

These exercises help you understand and apply different testing approaches (Black Box, White Box, Gray Box). The goal is to develop **intuition** for when to use each approach and how they complement each other.

---

## Exercise 1.1: Black Box Testing Practice

### Task

You're testing a login feature. You have:
- Requirements document
- Access to the application
- **No access to code**

1. **Design Black Box Tests**:
   - Based only on requirements
   - From user perspective
   - Test functionality, not implementation
   - Create 10-15 test cases

2. **Test Design Techniques**:
   - Use Equivalence Partitioning (valid/invalid inputs)
   - Use Boundary Value Analysis (edge cases)
   - Use Decision Tables (different combinations)
   - Document which technique you used

3. **Execute Tests**:
   - Run your test cases
   - Document results
   - Note what you can and can't verify

### Reflection

- What can you test without code knowledge?
- What can't you test?
- How does user perspective help?
- What are the limitations of black box testing?

---

## Exercise 1.2: White Box Testing Practice

### Task

You're testing a function that calculates discount:

```java
public double calculateDiscount(double price, int quantity, boolean isMember) {
    double discount = 0;
    
    if (isMember) {
        discount = 0.10; // 10% for members
    }
    
    if (quantity >= 10) {
        discount += 0.05; // Additional 5% for bulk
    }
    
    if (price > 100) {
        discount += 0.02; // Additional 2% for high value
    }
    
    return price * quantity * discount;
}
```

1. **Analyze Code Structure**:
   - Identify all branches
   - Identify all conditions
   - Map decision points

2. **Design White Box Tests**:
   - Test each branch
   - Test each condition
   - Test edge cases in code
   - Aim for 100% branch coverage

3. **Create Test Cases**:
   - Document inputs and expected outputs
   - Cover all code paths
   - Test boundary conditions in code

### Reflection

- How does code knowledge change your testing?
- What defects can you find with white box that black box might miss?
- What are the limitations of white box testing?
- When is code coverage useful vs. misleading?

---

## Exercise 1.3: Gray Box Testing Practice

### Task

You're testing an API endpoint:
- You have API documentation
- You know the request/response structure
- You have some understanding of implementation
- But you don't have full code access

**API**: `POST /api/users`
- Request: `{ "name": "string", "email": "string", "age": number }`
- Response: `{ "id": number, "name": "string", "email": "string" }`

1. **Design Gray Box Tests**:
   - Use API documentation (black box perspective)
   - Use implementation knowledge (white box perspective)
   - Test both behavior and structure
   - Create comprehensive test cases

2. **Test Scenarios**:
   - Valid requests (black box)
   - Invalid requests (black box)
   - Edge cases based on implementation (white box)
   - Integration points (gray box)

3. **Compare Approaches**:
   - What did you test from black box perspective?
   - What did you test from white box perspective?
   - How did combining both help?

### Reflection

- How does gray box combine benefits of both?
- What makes gray box practical?
- When is gray box the best approach?
- How do you balance both perspectives?

---

## Exercise 1.4: Choosing the Right Approach

### Task

For each scenario, decide which approach is best and why:

1. **Scenario A**: Testing a mobile app's UI
   - Black Box, White Box, or Gray Box?
   - Why?

2. **Scenario B**: Testing a complex algorithm
   - Black Box, White Box, or Gray Box?
   - Why?

3. **Scenario C**: Testing an API
   - Black Box, White Box, or Gray Box?
   - Why?

4. **Scenario D**: Testing database queries
   - Black Box, White Box, or Gray Box?
   - Why?

5. **Scenario E**: Acceptance testing
   - Black Box, White Box, or Gray Box?
   - Why?

### Reflection

- What factors determine which approach to use?
- Can you use multiple approaches for the same feature?
- How do constraints (time, access, knowledge) affect choice?

---

## Exercise 1.5: Combining Approaches

### Task

Pick a feature to test (e.g., user registration):

1. **Black Box Testing**:
   - Test from user perspective
   - Use requirements only
   - Document what you test

2. **White Box Testing** (if you have code):
   - Test code structure
   - Test all branches
   - Document what you test

3. **Gray Box Testing**:
   - Combine both perspectives
   - Use API/docs + some code knowledge
   - Document what you test

4. **Compare Results**:
   - What did each approach find?
   - What overlaps?
   - What's unique to each?
   - Which was most effective?

### Reflection

- How do approaches complement each other?
- What's the value of using multiple approaches?
- How do you decide when to use which?
- What's the most practical combination?

---

## Exercise 1.6: Testing Levels and Approaches

### Task

Map testing approaches to testing levels:

1. **Unit Testing**:
   - Which approach? (Black/White/Gray)
   - Why?
   - Who typically does it?

2. **Integration Testing**:
   - Which approach?
   - Why?
   - Who typically does it?

3. **System Testing**:
   - Which approach?
   - Why?
   - Who typically does it?

4. **Acceptance Testing**:
   - Which approach?
   - Why?
   - Who typically does it?

### Reflection

- How do approaches map to testing levels?
- Why does the approach change at different levels?
- How does this help you plan testing?

---

## Exercise 1.7: Real-World Application

### Task

Think about a project you're working on (or have worked on):

1. **Current Approach**:
   - What testing approach do you primarily use?
   - Why?
   - What are the limitations?

2. **Alternative Approaches**:
   - How could you incorporate other approaches?
   - What would you gain?
   - What are the constraints?

3. **Improvement Plan**:
   - How would you add other approaches?
   - What would you test differently?
   - How would you measure improvement?

### Reflection

- How can you apply multiple approaches in your work?
- What prevents you from using certain approaches?
- How can you overcome constraints?
- What's the most practical mix for your situation?

---

## 🎯 Self-Assessment

After completing these exercises, ask yourself:

1. Can I explain the difference between black box, white box, and gray box?
2. Do I know when to use each approach?
3. Can I design tests from each perspective?
4. Do I understand how approaches complement each other?
5. Can I apply the right approach in real projects?

---

## 💡 Key Insights to Carry Forward

- **Black box tests behavior** - User perspective, no code knowledge
- **White box tests structure** - Code perspective, full knowledge
- **Gray box combines both** - Practical, realistic approach
- **Context determines approach** - Use the right tool for the situation
- **Effective testing uses all** - Different levels, different approaches
- **Approaches complement** - Not mutually exclusive

---

**Next Steps**: Once comfortable with testing approaches, move to Module 4: SDLC Models to understand how development models affect testing strategy.

