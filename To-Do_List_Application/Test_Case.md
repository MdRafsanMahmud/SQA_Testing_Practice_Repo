# ✅ Test Cases - To-Do List Application

## 📌 Project Information  
- **Project Name:** To-Do List Application  
- **Version:** 1.0  
- **Date:** 02 March, 2025  
- **Test Plan Author:** Md Rafsan Mahmud  

## 📖 Introduction  
This document provides detailed **test cases** for the **To-Do Application**. The application allows users to manage their daily tasks by offering functionalities such as **creating, updating, deleting, and marking tasks as completed**.  

The primary objective is to ensure that all **functional and non-functional requirements** are tested to verify the application's **reliability, usability, and performance**. These test cases include **manual testing covering both positive and negative scenarios** to identify defects and validate expected behavior.  

---

## ✅ **Functional Test Cases**  

### **User Registration**  
**Test Case ID:** TC001  
**Test Case:** Verify that users can register with their email and password.  
**Preconditions:** None  
**Test Steps:**  
1. Navigate to the registration page.  
2. Enter a valid email address and password.  
3. Confirm the password.  
4. Click 'Register' button.  
**Expected Result:** User should receive a confirmation message and account should be created.  
**Postconditions:** The new user should be able to log in with their credentials.  

---

### **User Login**  
**Test Case ID:** TC002  
**Test Case:** Verify that users can log in with their registered email and password.  
**Preconditions:** User must be registered.  
**Test Steps:**  
1. Navigate to the login page.  
2. Enter registered email and password.  
3. Click 'Login' button.  
**Expected Result:** User should be successfully logged in and redirected to the dashboard.  
**Postconditions:** The user should remain logged in until they log out.  

---

### **Invalid Email Registration**  
**Test Case ID:** TC003  
**Test Case:** Verify that users cannot register with an invalid email format.  
**Preconditions:** None  
**Test Steps:**  
1. Navigate to registration page.  
2. Enter an invalid email.  
3. Click 'Register' button.  
**Expected Result:** System should display an error message for invalid email format.  
**Postconditions:** The user should not be registered.  

---

### **Incorrect Login Credentials**  
**Test Case ID:** TC004  
**Test Case:** Verify that users cannot log in with incorrect credentials.  
**Preconditions:** User must be registered.  
**Test Steps:**  
1. Navigate to login page.  
2. Enter incorrect email or password.  
3. Click 'Login' button.  
**Expected Result:** System should display an 'Invalid credentials' error message.  
**Postconditions:** The user should not be logged in.  

---

### **Resetting Password**  
**Test Case ID:** TC005  
**Test Case:** Verify that the user can reset their password if they forget it.  
**Preconditions:** User must be registered.  
**Test Steps:**  
1. Navigate to the home page.  
2. Click "Forget Password".  
3. Enter registered email address.  
4. Click the “Reset Password” button.  
**Expected Result:** User should receive a password reset email.  
**Postconditions:** User should be able to reset their password using the recovery link in the email.  

---

### **Title and Description Validation**  
**Test Case ID:** TC006  
**Test Case:** Verify that users cannot create a task without a title and description.  
**Preconditions:** User must be logged in.  
**Test Steps:**  
1. Navigate to dashboard.  
2. Click 'Add Task' button.  
3. Leave fields empty.  
4. Click 'Save'.  
**Expected Result:** System should display an error prompting user to enter a title and description.  
**Postconditions:** No task should be created.  

---

### **Create a New Task**  
**Test Case ID:** TC007  
**Test Case:** Verify that users can create a new task.  
**Preconditions:** User must be logged in.  
**Test Steps:**  
1. Navigate to dashboard.  
2. Click 'Add Task' button.  
3. Enter task details and title.  
4. Click 'Save'.  
**Expected Result:** New task should appear in the task list.  
**Postconditions:** The task should be visible in the dashboard.  

---

### **Update an Existing Task**  
**Test Case ID:** TC008  
**Test Case:** Verify that users can update an existing task.  
**Preconditions:** User must be logged in and have at least one task.  
**Test Steps:**  
1. Navigate to dashboard.  
2. Select a task.  
3. Click 'Edit Task'.  
4. Update details.  
5. Click 'Save' button.  
**Expected Result:** Task should reflect updated details immediately.  
**Postconditions:** The updated task should be saved in the system and remain visible with the new details in the task list.  

---

### **Delete a Task**  
**Test Case ID:** TC009  
**Test Case:** Verify that users can delete a task.  
**Preconditions:** User must be logged in and have at least one task.  
**Test Steps:**  
1. Navigate to dashboard.  
2. Select a task.  
3. Click 'Delete Task'.  
4. Confirm deletion.  
**Expected Result:** Task should be removed from the list.  
**Postconditions:** The task should no longer be visible in the dashboard.  

---

### **Task Completion Marking**  
**Test Case ID:** TC010  
**Test Case:** Verify that users can mark a task as completed.  
**Preconditions:** User must be logged in and have at least one task.  
**Test Steps:**  
1. Navigate to dashboard.  
2. Select a task.  
3. Click 'Mark as Completed'.  
**Expected Result:** Task should move to the completed tasks section and no longer appear in the active list.  
**Postconditions:** The task should no longer appear in the active task list and should be marked as completed.  

---

## 🔹 **Non-Functional Test Cases**  

### **Performance Testing - Dashboard Load Time**  
**Test Case ID:** TC011  
**Test Case:** Verify that the dashboard loads within 3 seconds.  
**Preconditions:** User must be logged in.  
**Test Steps:**  
1. Navigate to the login page.  
2. Enter valid credentials and log in.  
3. Measure the time taken for the dashboard to fully load.  
**Expected Result:** The dashboard should load within 3 seconds.  
**Postconditions:** The dashboard is displayed within the specified time.  

---

### **Usability Testing – Navigation Intuitiveness**  
**Test Case ID:** TC012  
**Test Case:** Verify that users can navigate the application easily.  
**Preconditions:** None.  
**Test Steps:**  
1. Ask a new user to perform tasks like Registering, Logging in, Creating, Updating, Deleting, and Completing tasks.  
2. Observe if the user can complete tasks without confusion.  
3. Ask the user to rate the ease of navigation.  
**Expected Result:** Users should be able to complete all actions without needing external help.  
**Postconditions:** Users can navigate all functionalities smoothly.  

---

### **Security Testing - Data Encryption & Protection**  
**Test Case ID:** TC013  
**Test Case:** Verify that user data is encrypted and protected.  
**Preconditions:** None.  
**Test Steps:**  
1. Register a new user account.  
2. Inspect the storage of user credentials (ensure encryption).  
3. Attempt unauthorized login.  
4. Try accessing another user’s data.  
**Expected Result:**  
- User credentials should be stored in encrypted form.  
- Unauthorized logins should be denied.  
- Unauthorized access should not be possible.  
**Postconditions:** User data remains secure and protected.  

---
