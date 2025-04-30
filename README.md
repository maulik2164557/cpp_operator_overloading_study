# C++ Operator Overloading  
# Complex Cases
## Member vs Friend Function Behavior

👨‍💻 Author: Maulik N. Patoliya  
🎓 Branch: Computer Engineering | Semester: 02 | 
📘 Subject: Operator Overloading – Complex Cases  
📍 Material: [Operator_Overloading_(Member + Friend Function Behavior)](#)

---

### 🔍 Overview

This repository presents a **deep comparative study** of how C++ handles operator overloading when **both member and friend functions** are defined with different argument types (`const`, non-const, reference, value). 

Through **14+ test cases**, this study explores:
- Ambiguity resolution by the compiler
- Rules of overload resolution
- Common pitfalls developers face
- Best practices to avoid errors

---

### 🧪 Test Case Structure

Each test case includes:
- Source code (with `Complex` class)
- Member and friend operator overloads
- Output behavior or ambiguity error
- Explanation of compiler's choice

---

### 🧾 Summary Table (Highlights)

---

### 🧠 Key Learnings

- If **both overloads use pass-by-reference**, and are non-const, ambiguity occurs.
- If **one uses const**, and the other doesn’t, the compiler chooses the better match.
- When **both use pass-by-value**, ambiguity occurs — const makes no difference.
- **Best practice**: Use **const reference** for both member and friend — or define only one.

---

### 💡 Final Recommendation

> ✅ Define **only one** overload (preferably member), and pass by `const reference`.

---
