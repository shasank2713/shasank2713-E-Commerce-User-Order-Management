# 🛒 E-Commerce API Testing Simulation – ReqRes API

This project simulates testing of an E-Commerce backend using **ReqRes** dummy APIs.  
It includes **manual + automated testing** for user and order flow using Postman, Newman, Jenkins, and Jira.

---

## 📦 Modules Covered

1. ✅ User Registration  
2. ✅ User Login  
3. ✅ Product Browsing  
4. ✅ Add to Cart  
5. ✅ Place Order  
6. ✅ Cancel Order  

---

## 🧪 What We Tested

- Positive & Negative Test Scenarios  
- Status Codes (200, 201, 204, 400, 404)  
- Token Generation (Login)  
- Request Body Validation  
- Response Data Structure  
- Automation using Newman & Jenkins  
- Bug Tracking in Jira  
- Test Cases maintained in Excel Sheet (.xlsx)

---

## 🛠️ Tools Used

| Tool         | Purpose                    |
|--------------|----------------------------|
| Postman      | API Manual Testing         |
| Newman       | API Automation             |
| Jenkins      | CI/CD for API Testing      |
| Jira         | Bug Tracking               |
| Excel Sheet (.xlsx) | Test Case Documentation    |

---

## 🌐 API Endpoints Mapping

| Module            | Method | Endpoint                        | Description                          |
|-------------------|--------|----------------------------------|--------------------------------------|
| User Registration | POST   | /api/register                    | Register new user                    |
| User Login        | POST   | /api/login                       | User login with token response       |
| Product Browsing  | GET    | /api/users?page=2                | Simulate product browsing            |
| Add to Cart       | POST   | /api/users                       | Add product to cart (dummy)          |
| Place Order       | POST   | /api/users                       | Place order simulation               |
| Cancel Order      | DELETE | /api/users/2                     | Cancel placed order (simulate)       |

---

## ✅ How to Run Automation Tests

1. Export your Postman collection and environment.
2. Use Newman to run via CLI:

```bash
newman run "E-Commerce API Testing.postman_collection.json" -e "E-Commerce Test Env.postman_environment.json"
```

3. Jenkins job (Freestyle or Pipeline) can be configured to run Newman automatically.

---

## 🐞 Bug Tracking

Bugs found during negative test scenarios were logged in **Jira** with:
- Steps to reproduce  
- Expected vs Actual Result  
- Screenshots (if needed)

---

## 📊 Test Case Format (Maintained in Excel)

| Testcase_ID | Title           | Precondition       | Steps                            | Expected Result            | Actual Result | Status |
|-------------|------------------|---------------------|-----------------------------------|-----------------------------|----------------|--------|
| REG_01      | Valid Registration| User not registered | Send POST to /api/register        | Status 200 OK + token       | As expected    | Pass   |
| LOGIN_02    | Missing password  | Email only          | Send POST to /api/login           | Status 400 Bad Request      | As expected    | Pass   |

---

## 👨‍💻 Author

**Shasank Sinha**  
Role: QA Support & API Tester  
Tools: Postman | Newman | Jenkins | Jira | Excel

---

## 📎 License

This is a **dummy testing simulation project** for learning and portfolio purposes. No real e-commerce backend is used.
