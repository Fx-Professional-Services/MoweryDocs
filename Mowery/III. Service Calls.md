# 🧾 Service Call Features: Printing, Messaging, and Dispatching

This guide explains how to use key features in the **Service Call** module. It covers how to:

- Print a parts list using **Print to Parts**
- Send technician updates via SMS
- Handle automatic logout after inactivity
- Assign HVAC service calls from the dispatch board

These tools improve operational efficiency, data tracking, and communication with customers.

---

## 🔗 Quick links

- [Print to Parts from a Service Call](#print-to-parts-from-a-service-call)
- [Send Text Message from Service Calls](#send-text-message-from-service-calls)
- [Automatic Logout After Inactivity](#automatic-logout-after-inactivity)
- [Assign Calls on the Dispatch Board](#assign-calls-on-the-dispatch-board)

---

# Print to Parts from a Service Call

You can generate a printed parts list directly from a service call using the **Print to Parts** feature.

## What happens when you click "Print to Parts"

When the dispatcher clicks the **Print to Parts** button:

- The system updates the **Printed to Parts** field with:
  - The dispatcher's account name
  - The date and time the button was clicked

> 📌 Use this field as a log to track print activity.

## How to print to parts

1. From the main menu, go to **Service Calls**.
2. In the rightmost column (highlighted in blue), click a service card.
3. Scroll to the bottom-right of the screen.
4. Click **Print to Parts**:
   - A print layout appears.
   - If you see a “Printer not found” message, you can ignore it.
5. The **Printed to Parts** field automatically updates with your name and timestamp.

## Default printer behavior

- The print job is sent to the **default parts printer**.
- You don't need to select a printer manually.

### Benefits

- Saves time  
- Reduces user errors  
- Improves dispatch efficiency  

## Definitions

- **Service Call**: A scheduled visit for maintenance, repair, or inspection.
- **Print to Parts**: A function that prints a parts list from a service call.
- **Printed to Parts field**: A read-only log showing who printed and when.
- **Default parts printer**: A pre-set printer the system uses automatically.

---

# Send Text Message from Service Calls

You can send a text message from a service call using Twilio. The message includes technician details and a public-facing profile link to build customer trust.

## Pre-send checklist

Before sending a message:

1. **Check the customer record**  
   - Go to **Master Property List**.  
   - Make sure the phone number is valid and marked as preferred.

2. **Check the service call record**  
   - Go to **Service Calls**.  
   - Confirm the **Accept Text Message** checkbox is selected.

3. **Validate the phone number**  
   - Format must follow U.S. standards (10 digits, with area code).

## How to send a text message

1. From the main menu, go to **Service Calls**.
2. Open the appropriate service call.
3. In the **Contact** section:
   - Confirm that **Text** is selected as the contact method.
   - Make sure the number is valid, preferred, and has **Accept Text Message** checked.
4. Click the **Send Text Message** icon (blue) next to the preferred number.
5. The system displays a success or error message.

## Requirements

- Valid U.S. cellphone number  
- Phone number is marked as preferred  
- **Accept Text Message** is checked  
- Contact method is set to **Text**

## Error messages

| Condition                                    | Error message                                              |
|---------------------------------------------|------------------------------------------------------------|
| No preferred number                         | `A preferred phone number is required to send a message.`  |
| Number is missing but checkbox is checked   | `Cell number is required if Accept Text Message is checked.` |
| Invalid number                              | `Invalid US Number.`                                       |
| Twilio failure                              | `Failed to deliver.`                                       |
| Other errors                                | Twilio’s error message is shown directly                   |

## Success message

If the message sends successfully, a confirmation message appears.

## Message contents

Messages include:

- Technician name(s)  
- Customer address  
- Public profile link  
- Friendly message from the technician

### Sample message

Hello [Customer Name], [Technician Name(s)] from Mowery is on the way to [Customer Address].  
Click here for more details: [Technician Profile Webpage Link]

Hi, my name is [Technician Name]. I’ll be your technician today. [Short Technician Bio]  
If you have any questions, I’m here to help. Thank you for choosing Mowery!


## Template variables

| Variable                             | Description                                |
|--------------------------------------|--------------------------------------------|
| `[Customer Name]`                   | Full name of the customer                  |
| `[Technician Name(s)]`              | Name(s) of assigned technician(s)          |
| `[Customer Address]`                | Service address from the call              |
| `[Technician Bio]`                  | Introduction text from the technician      |
| `[Technician Profile Webpage Link]` | Public link to the technician’s profile    |

## Message behavior

- Can be sent manually or automatically from a service call.
- Links to a secure webpage showing:
  - Technician name, photo, and bio  
  - Estimated time of arrival  
  - Optional appointment confirmation

---

# Automatic Logout After Inactivity

To protect data, the system logs users out after 2 hours of inactivity.

## Overview

If no activity is detected for 2 hours:

- A warning appears:  
  > “No activity detected. The file will close unless you click Cancel.”

- If no action is taken, FileMaker automatically closes the session.

## Who this applies to

All users in FileMaker are affected, regardless of access level.

## Tips to stay logged in

- Click **Cancel** when prompted to extend your session.
- Save your work regularly.
- If logged out, reopen the file and log in again.

> ℹ️ This feature helps protect data by closing unattended sessions.

---

# Assign Calls on the Dispatch Board

You can assign technicians to unassigned service calls using the **HVAC Schedule Board**.

## How to assign a technician

1. From the main menu, go to **Service Calls**.
2. The **Schedule Board** appears.
3. In the **leftmost column**, locate unassigned HVAC calls (highlighted in peach).
4. Click a call to open the **Service Call Detail** screen.
5. In **Step 2: Assign Technician**, click **New**.
6. Click the down arrow next to the technician field.
7. Choose a technician from the dropdown list.

> 📌 Only configured technicians appear in the dropdown.

## What is HVAC?

**HVAC** stands for **Heating, Ventilation, and Air Conditioning**. These calls involve heating or cooling equipment and are managed through the **HVAC Dispatch Board**.

