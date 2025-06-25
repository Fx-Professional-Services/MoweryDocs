# 🧾 Service Call Features: Printing, Messaging, and Dispatching

This guide explains how to use key features in the **Service Call** module in FileMaker. It includes instructions for:

- Printing parts lists using **Print to Parts**
- Sending SMS messages with technician information
- Understanding the **automatic logout** behavior
- Assigning technicians using the **dispatch board**
- Viewing the **Technician Profile Page** sent to customers

These tools improve communication, track service activity, and streamline dispatching workflows.

---

## 🔗 Quick Links

- [Print to Parts from a Service Call](#print-to-parts-from-a-service-call)
- [Send Text Message from Service Calls](#send-text-message-from-service-calls)
- [Automatic Logout After Inactivity](#automatic-logout-after-inactivity)
- [Assign Calls on the Dispatch Board](#assign-calls-on-the-dispatch-board)
- [Technician Profile Page](#technician-profile-page)

---

## Print to Parts from a Service Call

You can generate a printed parts list directly from a service call using the **Print to Parts** feature.

### What happens when you click "Print to Parts"

When the dispatcher clicks **Print to Parts**:

- The **Printed to Parts** field is updated with:
  - The dispatcher's account name
  - The date and time of the action

> 📌 This field logs the print action for future reference.

### How to print to parts

1. Go to **Service Calls** from the main menu.
2. Click a service card in the rightmost column.
3. Scroll to the bottom-right of the screen.
4. Click **Print to Parts**:
   - A print layout opens.
   - Ignore any "Printer not found" message.
5. The system updates the **Printed to Parts** field automatically.

### Default printer behavior

- The system sends the job to the **default parts printer**.
- No manual printer selection is needed.

**Benefits**:
- Saves time  
- Reduces errors  
- Improves workflow

### Definitions

- **Service Call**: A scheduled visit for installation, repair, or inspection.
- **Print to Parts**: A function to print a job-specific parts list.
- **Printed to Parts field**: A log showing who printed the list and when.
- **Default parts printer**: A preconfigured printer used automatically.

---

##  Send Text Message from Service Calls

You can send a personalized text message to customers directly from the Service Call screen using Twilio.

### Pre-send checklist

Before sending a message:

1. **Master Property List**:  
   - Phone number is valid  
   - Marked as **preferred**

2. **Service Call**:  
   - **Accept Text Message** is checked

3. **Phone Format**:  
   - Valid 10-digit U.S. format

### How to send a text message

1. Go to **Service Calls**.
2. Open the service call record.
3. In the **Contact** section:
   - Confirm **Text** is selected
   - Ensure number is valid and preferred
   - Check **Accept Text Message**
4. Click the **Send Text Message** icon.
5. Wait for success or error message.

### Requirements

- Valid U.S. cellphone number  
- Preferred number selected  
- **Text** set as contact method  
- **Accept Text Message** checked

### Error messages

| Condition                                  | Message                                                    |
|-------------------------------------------|------------------------------------------------------------|
| No preferred number                       | `A preferred phone number is required to send a message.`  |
| Number missing, checkbox checked          | `Cell number is required if Accept Text Message is checked.` |
| Invalid number                            | `Invalid US Number.`                                       |
| Twilio delivery failure                   | `Failed to deliver.`                                       |
| Other Twilio errors                       | Shown directly from Twilio                                 |

### Success message

- The system displays a confirmation when the message is sent successfully.

### Message contents

- Technician name(s)  
- Customer address  
- Secure technician profile link  
- Personalized greeting  

**Sample message:**

Hello [Customer Name], [Technician Name(s)] from Mowery is on the way to [Customer Address].  
Click here for more details: [Technician Profile Webpage Link]

Hi, my name is [Technician Name]. I’ll be your technician today. [Short Technician Bio]  
If you have any questions, I’m here to help. Thank you for choosing Mowery!


### Template variables

| Variable                         | Description                             |
|----------------------------------|-----------------------------------------|
| `[Customer Name]`               | Full name of the customer               |
| `[Technician Name(s)]`          | Name(s) of assigned technician(s)       |
| `[Customer Address]`            | Service address                         |
| `[Technician Bio]`              | Introduction text from technician       |
| `[Technician Profile Webpage Link]` | Secure profile link for the technician |

### Message behavior

- Sent manually or automatically from a Service Call
- Opens a secure webpage showing:
  - Technician name, photo, bio
  - Arrival time
  - Optional appointment confirmation

---

##  Automatic Logout After Inactivity

The system logs out users after a period of inactivity to protect data.

### Overview

- If inactive for **2 hours**, a message appears:
  > "No activity detected. The file will close unless you click Cancel."
- If no action is taken, the file automatically closes.

### Who this applies to

- All FileMaker users

### Tips to stay logged in

- Click **Cancel** when prompted  
- Save work regularly  
- Reopen the file to log back in if logged out

> ℹ️ This feature prevents unattended sessions from remaining active.

---

## Assign Calls on the Dispatch Board

Use the **HVAC Schedule Board** to assign technicians to service calls.

### How to assign a technician

1. Go to **Service Calls** from the main menu.
2. View the **Schedule Board**.
3. In the leftmost column, find unassigned HVAC calls (highlighted in peach).
4. Click a call to open the Service Call Detail.
5. In **Step 2: Assign Technician**, click **New**.
6. Use the dropdown to select a technician.

> 📌 Only preconfigured technicians appear in the list.

### What is HVAC?

**HVAC** stands for **Heating, Ventilation, and Air Conditioning**. HVAC calls relate to heating or cooling systems and are managed on the HVAC dispatch board.

---

## Technician Profile Page

When customers receive a text message, they are linked to a personalized **Technician Profile Page**.

### What customers see

#### Service information

- **Status** — Scheduled, In Progress, or Completed  
- **Appointment Time**  
- **Service Description**  
- **Service Type** (e.g., HVAC, Electrical)

#### Technician details

- **Technician Name(s)**  
- **Photos**  
- **Bio** (if available)

### Security and access

- Each link is unique and secure  
- No login required  
- Customers cannot browse other profiles  
- Mobile-friendly and accessible

> This improves customer confidence and transparency before a technician arrives.
