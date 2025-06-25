# 🖨️ Print to Parts and Service Call Messaging Guide

This guide explains how to use the **Print to Parts** feature, send technician text messages from a **Service Call**, and how the system handles automatic logout after inactivity.

---

## **Quick Links**

- [Print to Parts from a Service Call](#print-to-parts-from-a-service-call)
- [Send Text Message from Service Calls](#send-text-message-from-service-calls)
- [Automatic Logout After Inactivity](#automatic-logout-after-inactivity)

---

# Print to Parts from a Service Call

You can generate a printed parts list directly from a **Service Call** using the **Print to Parts** feature.

---

## ✅ What Happens When You Click "Print to Parts"

When the **dispatcher** clicks the **Print to Parts** button:

- The system updates the **Printed to Parts** field with:
  - The **name of the dispatcher** who clicked the button.
  - The **date and time** of the action.

> 📌 This field serves as a log for tracking print activity.

---

## 🔄 Steps to Use Print to Parts

1. Go to **Service Call** from the main menu.
2. In the **rightmost column** (highlighted in blue), click a service card to open the **Customer Property** or **Service Call** screen.
3. Scroll to the **bottom right** of the page.
4. Click **Print to Parts**:
   - A print layout will appear.
   - If you see a **"Printer not found"** message, you can ignore it. It means a printer isn’t connected to your network.
5. After clicking:
   - The **Printed to Parts** field updates with your account name and the timestamp.

---

## 🛠️ Default Printer Behavior

- The system sends the print job to the **default parts printer**.
- No manual printer selection is required.

**Benefits**:

- 🕒 Saves time  
- ✅ Reduces user errors  
- 🚀 Improves dispatch efficiency  

---

## 📘 Definitions

**Service Call**  
A scheduled visit by a technician for maintenance, repair, or installation. Contains job details, service address, assigned technician, and materials used.

**Print to Parts**  
Allows dispatchers or technicians to print a parts list directly from a Service Call record.

**Printed to Parts Field**  
A system log showing the dispatcher’s account name and timestamp when the Print to Parts action was performed.

**Default Parts Printer**  
The designated printer used for printing parts lists automatically.

---

# Send Text Message from Service Calls

You can send a text message to a customer directly from the **Service Call** screen using the integrated messaging feature powered by Twilio. The message includes technician details and a secure public webpage link to build trust with customers.

---

## 📝 Pre-send Checklist

Before sending a message:

1. **Check the Master Property List**  
   - Go to **Master Property List**.  
   - Verify the customer’s phone number is valid and marked as **preferred**.  

2. **Check the Service Call Record**  
   - Go to **Service Calls**.  
   - Open the record for the customer.  
   - Ensure **Accept Text Message** is checked for the phone number.  

3. **Validate Phone Number Format**  
   - Confirm it follows U.S. standards (10-digit number with area code).

---

## ✉️ How to Send a Text Message

1. Go to **Service Calls** from the main menu.
2. Select the specific service call record.
3. In the **Contact** section:
   - Confirm **Text** is selected as the contact method.
4. Verify:
   - A **valid U.S. cellphone number** is saved.  
   - The number is marked as **preferred**.  
   - The **Accept Text Message** checkbox is checked.  
5. Locate the **Send Text Message** icon (in blue) next to the **Preferred Number**.
6. Click the icon to send the message.
7. The system provides feedback:
   - **Success message** confirms the text was sent.
   - **Error message** explains why sending failed.

---

## ⚠️ Requirements

- A valid U.S. cellphone number is required.  
- The **Accept Text Message** checkbox must be checked.  
- The number must be marked as **preferred**.  
- **Text** must be selected as the contact method.

---

## 🚫 Error Messages

| Condition                                    | Error Message                                      |
|----------------------------------------------|---------------------------------------------------|
| No preferred number                          | `A preferred phone number is required to send a message.` |
| Accept Text checked, but number is blank     | `Cell number is required if Accept Text Message is checked.` |
| Invalid phone number                         | `Invalid US Number.`                              |
| Twilio delivery failure                      | `Failed to deliver.`                              |
| Other errors from Twilio                     | Displays exact error message from Twilio          |

---

## ✅ Success Message

A confirmation message appears when the text is sent successfully.

---

## 📨 Message Contents

The system sends a personalized message with:

- Technician name(s)  
- Customer address  
- Public technician profile link  
- Short greeting from the technician  

### Example Message

Hello [Customer Name], [Technician Name(s)] from Mowery is on the way to [Customer Address].  
Click here for more details: [Technician Profile Webpage Link]

Hi, my name is [Technician Name]. I’ll be your technician today. [Short Technician Bio]  
If you have any questions, I’m here to help. Thank you for choosing Mowery!


---

## 🔧 Template Variables

| Variable                       | Description                                     |
|---------------------------------|-------------------------------------------------|
| `[Customer Name]`               | Full name of the customer                       |
| `[Technician Name(s)]`          | Assigned technician name(s)                     |
| `[Customer Address]`            | Service address from the Service Call           |
| `[Technician Bio]`              | Short introduction from the technician          |
| `[Technician Profile Webpage Link]` | Secure link to technician details           |

---

## 🌐 Message Behavior

- Sent automatically or manually from the **Service Call** screen.
- Includes a secure webpage with:
  - Technician photo, bio, and name  
  - Estimated arrival time  
  - Appointment confirmation options (if applicable)  
- Designed to build trust and enhance communication.

---

# Automatic Logout After Inactivity

The system automatically logs out inactive users to protect data and improve security.

---

## 📋 Overview

If there is no activity for 2 hours, the system displays:

> “No activity detected. The file will close unless you click Cancel.”

If no action is taken, FileMaker automatically closes the session.

---

## 🔔 How It Works

- After **2 hours of inactivity**, the logout warning appears.  
- Click **Cancel** to stay logged in and reset the timer.  
- If no response, the system closes automatically.

---

## 👤 Who This Applies To

All **FileMaker users**, regardless of role or access level.

---

## ✅ Tips to Stay Logged In

- Click **Cancel** when prompted to extend your session.  
- Save work frequently in case the file closes.  
- If logged out, reopen the FileMaker file and log in again.

---

> ℹ️ This feature prevents unattended sessions from remaining open and protects system data.


