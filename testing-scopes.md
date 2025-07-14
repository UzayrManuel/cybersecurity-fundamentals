# 🎯 Penetration Testing Scopes

There are three primary scopes when testing an application or service.  
Your understanding of the target will determine the **depth and style** of the penetration test.  
These scopes are:

---

## ⚫ Black-Box Testing

- **No internal knowledge** of the application or system is provided.
- The tester behaves like a **normal user**, interacting with the system externally.
- Focus is on functionality, UI behavior, and visible inputs/outputs.
- **No programming knowledge is required.**
- **Time-consuming** during the reconnaissance and enumeration phases due to the unknown nature of the system.
- Simulates a **real-world external attacker** scenario.

> Example: Clicking buttons on a web app and observing behavior without knowing what's running on the backend.

---

## ⚪ White-Box Testing

- The tester has **full knowledge** of the application, including source code, architecture, and logic.
- Often performed by **developers or internal security teams**.
- Tests internal components, functions, logic, and performance.
- **Very thorough** — all areas of the application can be validated.
- Requires **strong programming knowledge** and an understanding of system behavior.
- **Time-intensive**, but yields maximum coverage of vulnerabilities.

> Example: Reviewing source code and testing internal logic paths for input sanitization.

---

## ⚫⚪ Grey-Box Testing

- A **blend of black-box and white-box** testing approaches.
- The tester is given **limited knowledge** about the system or app (e.g. credentials, architectural diagrams).
- Simulates an attacker with **partial insider knowledge** (like a disgruntled employee).
- Saves time during recon while still providing valuable insights.
- Often used in **realistic penetration testing scenarios** for mature or well-hardened systems.

> Example: A tester knows the login mechanism and user roles but not the backend code.

---

## ✅ Summary Table

| Scope       | Knowledge Level     | Simulates                | Ideal For                         |
|-------------|---------------------|--------------------------|------------------------------------|
| Black-Box   | None                | External attacker        | Real-world unauthorized testing    |
| Grey-Box    | Limited             | Insider or semi-informed | Balanced, efficient pen testing    |
| White-Box   | Full                | Developer/internal team  | Thorough validation of all logic   |
