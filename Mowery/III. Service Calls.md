# 🖨️ Print to Parts from a Service Call

You can generate a printed parts list directly from a **Service Call** record using the **Print to Parts** feature.

---
### ✅ What Happens When You Click "Print to Parts"

When the **dispatcher** clicks the **Print to Parts** button:

- The system automatically populates the **Printed to Parts** field with:

  - The **name of the dispatcher** (account name) who clicked the button.

  - The **date and time** the button was clicked.

> 📌 This field serves as a log and helps track print activity for accountability.

---
### 🔄 Steps to Use Print to Parts

1. From the main menu, go to **Service Call**.

2. In the **rightmost column** (highlighted in fluorescent blue), click a service card. This opens the **Customer Property** or **Service Call** data entry screen.

3. Scroll to the **bottom right** of the page (Step 4 section).

4. Click the **Print to Parts** button:

   - A **print layout** will appear.

   - If you see a **"Printer not found"** error, you can ignore it. This usually means a printer isn't connected to your network.

5. After clicking the button:

   - The **Printed to Parts** field (bottom left) is updated automatically with:

     - Your **account name** (dispatcher).

     - The **timestamp** of the print action.

---
### 🛠️ Default Printer Behavior

- When you click **Print to Parts**, the system sends the print job to the **default parts printer**.

- You don't need to manually select a printer.

#### Benefits

- 🕒 Saves time  

- ✅ Reduces user errors  

- 🚀 Improves dispatch efficiency
---
## 📘 Definitions

### **Service Call**

A *Service Call* is a scheduled or on-demand visit by a technician to a customer location for maintenance, repair, installation, or inspection. It contains job details, service address, technician assignment, and materials used.

### **Print to Parts**

The *Print to Parts* feature enables dispatchers or technicians to print a parts list directly from the Service Call record. This printed list includes items used or required for the job.

### **Printed to Parts Field**

A read-only log that automatically captures:

- The dispatcher’s **account name**

- The **timestamp** of the Print to Parts action.

Used for traceability and accountability.

### **Default Parts Printer**

A designated printer that the system automatically uses for printing parts lists. It ensures:

- Consistent output location  

- No need for manual selection  

- Faster dispatch processing

# Send Text Message from Service Calls 

You can send a text message directly to a customer from the **Service Call** screen using the integrated messaging feature powered by Twilio. The message includes details about the technician and a public-facing webpage link to help build trust and transparency.

## Pre-send checklist

Before sending a text message, verify the following:

1. **Check the customer record in Master Property List**  
   - From the main menu, go to **Master Property List**.  
   - Locate the customer’s record.  
   - Verify the phone number is valid and saved correctly.  
   - Confirm the number is marked as **preferred**.

2. **Check the Service Call record**  
   - From the main menu, go to **Service Calls**.  
   - Open the corresponding service call record for the same customer.  
   - Confirm the **Accept Text Message** checkbox is checked for the phone number.

3. **Validate the phone number format**  
   - Ensure the phone number format conforms to U.S. standards (e.g., 10 digits, area code included).

---

## How to send a text message

1. **Open the Service Calls menu**  
   From the main menu, select **Service Calls** to view the list of service call records.

2. **Select a service call record**  
   Find and open the specific service call record for the customer you want to message.

3. **Verify contact method**  
   In the **Contact** section of the service call record:  
   - Confirm that **Text** is selected as the contact method. This enables the text messaging feature.

4. **Confirm the customer’s phone number details**  
   Check the phone number information associated with the customer:  
   - Ensure a **valid U.S. cellphone number** is saved in the customer’s record.  
   - Confirm this phone number is marked as **preferred** (the primary number used for communication).  
   - Make sure the **Accept Text Message** checkbox is **checked** for this number.

5. **Locate the Send Text Message icon**  
   Next to the **Preferred Number** field, find the **Send Text Message** icon, shown in blue.

6. **Click the Send Text Message icon**  
   Click the icon to initiate sending the text message.

7. **Wait for feedback**  
   The system will process the message and display one of the following:  
   - A **success message** confirming the text was sent.  
   - An **error message** explaining why the message failed to send (see the *Error messages* section below).

---

## Requirements

Before sending a text message, ensure the following:

- The phone number is a **valid U.S. cellphone number**.  
- The **Accept Text Message** checkbox is checked for the number.  
- The phone number is marked as **preferred**.  
- **Text** is selected as the **Contact Method**.

---

## Error messages

| Condition                                    | Error Message                                      |
| -------------------------------------------- | ------------------------------------------------ |
| No preferred phone number is set             | `A preferred phone number is required to send a message.` |
| Accept Text Message is checked but number is blank | `Cell number is required if Accept Text Message is checked.` |
| Invalid U.S. phone number                     | `Invalid US Number.`                              |
| Twilio fails to deliver                       | `Failed to deliver.`                              |
| Other errors from Twilio API                  | Displays the exact error message returned by Twilio |

---

## Success message

If the message is sent successfully, a confirmation message will appear on the screen.

---

If you experience issues after following these steps, verify all requirements are met or contact your support team.
   - Confirm that **Text** is selected as the contact method.

4. **Confirm the customer’s phone number details**  
   - Ensure a **valid U.S. cellphone number** is saved in the customer’s record.  
   - Confirm the number is marked as **preferred**.  
   - Make sure the **Accept Text Message** checkbox is checked.

5. **Locate the Send Text Message icon**  
   Next to the **Preferred Number** field, find the **Send Text Message** icon (in blue).  

6. **Click the Send Text Message icon**  
   Click the icon to initiate the message.

7. **Wait for feedback**  
   The system will display a success or error message based on the result.

---

## Message contents

The system sends customers a personalized message when a technician is on the way. The message includes:

- Technician name(s)
- Customer’s address
- A link to a public-facing technician profile page
- A short introduction and friendly greeting from the technician

### Sample message

Hello [Customer Name], [Technician Name(s)] from Mowery is on the way to [Customer Address].  
Click here for more details: [Technician Profile Webpage Link]

Hi, my name is [Technician Name]. I’ll be your technician today. [Short Technician Bio]  
If you have any questions or concerns, please don’t hesitate to share them—I'm here to help!

Thank you for choosing Mowery. We look forward to seeing you soon!
___


### Template Variables

| Variable                    | Description                                               |
|----------------------------|-----------------------------------------------------------|
| `[Customer Name]`          | The full name of the customer                             |
| `[Technician Name(s)]`     | One or more technician names assigned to the service call |
| `[Customer Address]`       | Full service address from the service call                |
| `[Technician Bio]`         | A short introduction and background from the technician   |
| `[Technician Profile Webpage Link]` | A secure public-facing link to technician details |

---

### Message Behavior

- Sent automatically or manually from the **Service Call** screen.
- Links to a secure webpage with:
  - Technician name, photo, and bio
  - Estimated time of arrival
  - Appointment confirmation or cancellation buttons (if applicable)
- Personal and professional tone to build trust with the customer.

# ⏳ Automatic Logout After Inactivity

  This guide explains how the Mowery FileMaker system automatically logs users out after a period of inactivity.

---
## 📋 Overview

To help protect data and improve security, the system will automatically close your session if there is no activity for 2 hours. A warning message appears before logout, giving you a chance to continue your session.

---
## 🔔 How It Works

- If the system detects **2 hours of inactivity**, it displays this message:  

  > “No activity detected. The file will close unless you click Cancel.”

- If you do not respond, FileMaker will automatically close.

- Clicking **Cancel** keeps your session active and resets the timer.

---
## 👤 Who This Applies To

This feature applies to **all FileMaker users**, regardless of their role or access level.

---
## ✅ Tips to Stay Logged In

- Click **Cancel** when prompted to continue your session.

- Save your work regularly in case the file closes.

- If logged out, simply reopen the FileMaker file and log in again.

---

> ℹ️ This feature ensures that unattended sessions do not remain open, protecting system data.

