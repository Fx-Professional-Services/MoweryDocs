# 🧾 Service Call Features: Printing, Messaging, and Dispatching

This guide explains how to use key features of the **Service Call** module in FileMaker. These tools improve communication with customers, track service activity, and streamline technician dispatch.

You will learn how to:

- Print a parts list
    
- Send a technician introduction by text message
    
- Assign technicians using the dispatch board
    
- View the **Technician Profile Page** shared with customers
    
- Understand the automatic logout process
    

---

## 🔗 Quick Links

- [Assign Technicians Using the Dispatch Board](#assign-technicians-using-the-dispatch-board)
    
- [Send a Text Message with Technician Details](#send-a-text-message-with-technician-details)
    
- [Technician Profile Page for Customers](#technician-profile-page-for-customers)
    
- [Print a Parts List from a Service Call](#print-a-parts-list-from-a-service-call)
    
- [Automatic Logout After Inactivity](#automatic-logout-after-inactivity)
    


# Managing Categories and Subcategories

This guide explains how to manage categories and subcategories in the system, including how to assign types such as **HVAC** or **Plumbing**.

---

## 🏷️ Specify a Type for Each Category

To create a new category and assign a type:

1. From the main menu, go to **System Defaults**.
2. From the top navigation menu, select **Category**.
3. Click **New Item** to create a new category.
4. In the **Category Name** field, enter the desired name.
5. In the **Type** field, select either:
   - `HVAC`
   - `Plumbing`

> **Note:** The **Type** field is a plain text attribute stored only in the **Category** table. It distinguishes between categories with the same name.

---

## 🧩 Use Duplicate Category Names with Different Types

The system allows multiple categories to share the same name if each has a different **Type**.

Example:

- `Miscellaneous (HVAC)` → Select the type **HVAC**
- `Miscellaneous (Plumbing)` → Select the type **Plumbing**

These categories will appear in the **Category** selection list within **Sub Category**, with the type shown in the name to help distinguish them. The underlying **Type** field remains hidden from users at the selection level.

---

## 📂 Assign Subcategories to Categories

To link a subcategory to a parent category:

1. From the main menu, go to **System Defaults**.
2. From the top navigation menu, select **Sub Category**.
3. Select the subcategory you want to edit.
4. From the **Category** dropdown, select the appropriate parent category.

> The **Category** dropdown displays the category name only.  
> Be sure you recognize the correct category based on its naming convention.  
> The subcategory automatically inherits the **Type** from its parent category.  

> **Important:** The **Type** field does not exist in the **Sub Category** table.

---

## 📦 Assign Products to a Subcategory

All products must be assigned to a subcategory.

- If no specific subcategory applies, assign the product to a `Miscellaneous` subcategory under the appropriate **Type**.  
  Examples:
  - `Miscellaneous (HVAC)`
  - `Miscellaneous (Plumbing)`

---

## Assign Technicians Using the Dispatch Board

The **HVAC Schedule Board** helps dispatchers assign technicians to service calls quickly.

### 📅  How to assign a technician

1. Go to **Service Calls** from the main menu.
    
2. Click **Schedule Board**.
    
3. Unassigned HVAC calls appear in peach on the left column.
    
4. Click a service call to open the details.
    
5. In **Step 2: Assign Technician**, click **New**.
    
6. Select a technician from the dropdown list.
    

> Only preconfigured technicians appear in the list.

---

### What is HVAC?

**HVAC** means **Heating, Ventilation, and Air Conditioning**. HVAC service calls cover heating, cooling, and ventilation systems. These calls are managed separately using the HVAC dispatch board.

---

## Send a Text Message with Technician Details

You can send customers a personalized text message with technician and appointment information using Twilio.

### 💬 Requirements

Before sending a message:

- The **Master Property List** phone number is:
    
    - Valid
        
    - Marked as **Preferred**
        
- In the **Service Call** record:
    
    - **Accept Text Message** is checked
        
- The phone number uses valid 10-digit U.S. format
    

---

### How to send a text message

1. Go to **Service Calls**.
    
2. Open the service call record.
    
3. In the **Contact** section:
    
    - Confirm **Text** is selected
        
    - Ensure the number is valid and marked as **Preferred**
        
    - Check **Accept Text Message**
        
4. Click the **Send Text Message** icon.
    
5. Wait for the confirmation or error message.
    

---

### Message contents

The text includes:

- Technician name(s)
    
- Customer address
    
- Secure link to the **Technician Profile Page**
    
- Technician introduction
    

**Example message:**

`Hello [Customer Name], [Technician Name(s)] from Mowery is on the way to [Customer Address].   Click here for more details: [Technician Profile Webpage Link]    Hi, my name is [Technician Name]. I’ll be your technician today. [Short Technician Bio]   If you have any questions, I’m here to help. Thank you for choosing Mowery!`

---

### Template variables

|Variable|Description|
|---|---|
|`[Customer Name]`|Full name of the customer|
|`[Technician Name(s)]`|Name(s) of assigned technician(s)|
|`[Customer Address]`|Service location|
|`[Technician Bio]`|Technician's introduction text|
|`[Technician Profile Webpage Link]`|Secure link to technician's profile|

---

### Error messages

|Condition|Message|
|---|---|
|No preferred number|`A preferred phone number is required to send a message.`|
|Number missing, checkbox checked|`Cell number is required if Accept Text Message is checked.`|
|Invalid number|`Invalid US Number.`|
|Twilio delivery failure|`Failed to deliver.`|
|Other Twilio errors|Message displayed directly from Twilio|

### Message Behavior

- Sent automatically or manually from the **Service Call** screen.
- Links to a secure webpage with:
    - Technician name, photo, and bio
    - Estimated time of arrival
    - Appointment confirmation or cancellation buttons (if applicable)
- Personal and professional tone to build trust with the customer.

---
##  Technician Profile Page for Customers

### 🌐 Technician Profile Page

This page explains what customers see when they click the **Technician Profile** link sent via text message from the Service Call system.

---
### 📋 Overview

Customers receive a secure link to a **Technician Profile Page** in their service notification text. This page provides helpful details about the upcoming appointment and the assigned technician(s).

### 👨‍🔧 What customers see

 **🛠️** **Service information:**

- Status (Scheduled, In Progress, or Completed)
    
- Appointment time
    
- Service description
    
- Service type (e.g., HVAC, Electrical)
    

**👷** **Technician details:**

- Technician name(s)
    
- Technician photos
    
- Short biography (if available)
    

---

### **🔒** Security and access

- Each link is unique and secure
    
- No login is required
    
- Customers cannot browse other profiles
    
- Mobile-friendly and easy to use
    


**By sharing this information, Mowery helps ensure a smooth, transparent, and professional experience for every customer.**

---

## Print a Parts List from a Service Call

You can print a job-specific parts list using the **Print to Parts** feature.

### 🖨️  How to print to parts

1. Go to **Service Calls** from the main menu.
    
2. Select a service call from the list (rightmost column).
    
3. Scroll to the bottom-right corner.
    
4. Click **Print to Parts**:
    
    - A print layout opens
        
    - Ignore "Printer not found" message if it appears
        
5. The **Printed to Parts** field updates automatically with:
    
    - Dispatcher’s account name
        
    - Date and time
        

---

### Default printer behavior

- The job goes to the **default parts printer**
    
- You do not need to select a printer manually
    

**Benefits:**

- Faster printing
    
- Fewer manual steps
    
- Improved workflow tracking
    

---
# 📘 Mowery FileMaker – Staff Management

This guide explains how to use the **Staff List** and **FileMaker Access** layouts in the Mowery FileMaker system to view, add, edit, and delete employee records.

---

## 📋 Overview

- The **Staff List** layout displays a read-only list of all employees.
- The **FileMaker Access** layout allows you to add, edit, or delete employee records.
- Use the **Form View** button to open employee records for editing.

---

## 👁️ View the Staff List

To view employee records:

1. From the main menu, click **Service Calls**.
2. In the **Service Calls** layout, click **Staff**.
3. The **Staff List** layout appears, showing all employees.

### Layout Behavior

- The **Staff List** layout is read-only.
- Use the **Form View** button (the number to the left of the employee’s name) to open an employee record in the **FileMaker Access** layout.

---

## ✏️ Edit an Employee Record

To edit an employee:

1. From the main menu, click **Service Calls**.
2. Click **Staff** to open the Staff List.
3. Click the **Form View** button—the number to the left of the employee’s name.
4. You will be redirected to the **FileMaker Access** layout.
5. Update the employee details as needed.
6. Changes are saved automatically.

---

## ➕ Add a New Employee

To add an employee:

1. In the **FileMaker Access** layout, click **New** in the top-right corner.
2. Enter the employee’s information.
3. The record saves automatically.

> **Note:** New employee records follow all system workflows and validation rules.

---

## 🗑️ Delete an Employee Record

You can delete employee records from either the **Staff List** layout or the **FileMaker Access** layout.

### From the Staff List Layout

1. In the **Staff List**, locate the employee’s row.
2. Under the **Account Status** column, click **Delete Account** to remove the employee’s FileMaker account.
3. To remove the employee record and their history, click the red **(X)** button next to **Delete Account**.

### From the FileMaker Access Layout

1. In the **FileMaker Access** layout, select the employee record.
2. Click the **(X)** button to the far right of the row.
3. A confirmation dialog appears. Click **Delete** to confirm or **Cancel** to exit.

_____

## Automatic Logout After Inactivity

The system protects your data by logging out inactive users.

### ⏲️  How it works

- After **2 hours** of inactivity:
    
    - A message appears: `"No activity detected. The file will close unless you click Cancel."`
        
- If no action is taken, the file closes automatically
    

**Who this applies to:**

- All FileMaker users
    

### Tips to stay logged in

- Click **Cancel** when prompted
    
- Save your work regularly
    
- Reopen the file if logged out
    

> This feature helps prevent unauthorized access to unattended sessions.

---

## Terminology Reference

| Term                        | Description                                             |
| --------------------------- | ------------------------------------------------------- |
| **Service Call**            | Scheduled visit for installation, repair, or inspection |
| **HVAC**                    | Heating, Ventilation, and Air Conditioning              |
| **Print to Parts**          | Function to print a job-specific parts list             |
| **Printed to Parts field**  | Record of who printed the parts list and when           |
| **Default parts printer**   | Preconfigured printer used for parts list printing      |
| **Technician Profile Page** | Secure webpage showing technician details for customers |
| **Accept Text Message**     | Checkbox allowing text communications to the customer   |
| **Twilio**                  | Service used to send SMS messages to customers          |
