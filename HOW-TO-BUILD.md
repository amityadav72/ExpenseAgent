# 🛠️ How to Build and Run ExpenseAgent on Azure AI Studio

This guide helps you set up the **ExpenseAgent** using Microsoft Azure AI Foundry.

---

## 1. Sign in to Azure AI Studio
- Visit: [https://portal.azure.com/](https://portal.azure.com/)
- Use your Microsoft or organizational account.

  ### 1 a. Go to Azure AI Foundry
![image](https://github.com/user-attachments/assets/73f4ca7b-7614-4736-9986-d6bf7a367a84)

### 1 b. Create a resource

![image](https://github.com/user-attachments/assets/2c59841e-4797-48d6-986d-0f1460bf7b12)

### 1 c. Setup the details & Deploy it

![image](https://github.com/user-attachments/assets/10e8d9a4-f828-4164-88f9-16851a241f5c)

### 1 d. Leave everything default and create

![Screenshot 2025-06-10 133047](https://github.com/user-attachments/assets/ab16a1cd-ab62-4ba9-8310-f6cacce0ffd4)

### 1 e. wait for deployment and go to resource 

![image](https://github.com/user-attachments/assets/230f5308-2145-4a22-9087-9d7230c40287)

---

## 2. Create a Project
- Click **"New Project"**
- Name: `ExpenseAgent`
- Description: Corporate Expense Tracking Assistant

---

## 3. Create an Agent
- Inside your project, go to **Agents** > **New Agent**
- Name it: `ExpenseAgent`
- Paste the contents of `agent-instructions.md` into the agent's instruction box

---

## 4. Attach Corporate Policy
- Copy content from `expense-policy.md`
- Paste this into the **knowledge** or **documents** section (or use as a reference in prompt)

---

## 5. Test the Agent
- Go to **Playground**
- Example: `Log a $200 travel expense for Project X with receipt.`
- Agent should:
  - Categorize it as "Travel"
  - Check if it follows budget
  - Ask for clarification if something is missing

---

## 6. Output Generation
- Ask: `Generate monthly expense summary`
- Agent will provide analysis and a downloadable format (see `output.md`)

---

## 7. Share or Customize
- Publish this repo or fork it.
- Customize instructions for your own organization's policy.
