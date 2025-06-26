# Task Codes

## 🔢 Override the Task Code

Task Codes are used to control the sequence of tasks within the product catalog. You can override these codes to manually reorder tasks as needed.

### 💡 Functionality Overview

- **Reordering Tasks**: Task codes determine the display order of items. You can update the code to move a task up or down in the sequence.
- **Automatic Sequencing**: When new items are added, task codes automatically increment or follow a predefined sequence.
- **Reflective Display**: Any changes made to a task code are instantly reflected in the user interface—especially in the product catalog and category structure.

### 🛠️ Manual Overrides

You can manually override a task code to customize the task order:

## 🔢 Override the Task Code

Task Codes are used to control the sequence of tasks within the product catalog. These numeric values define the order in which items appear and can be manually adjusted for custom ordering.

---

### 💡 Functionality Overview

- **Reordering Tasks**: Task codes determine the display order of items within their respective category and subcategory. You can update the code to move a task up or down.
- **Automatic Sequencing**: When new items are added, task codes automatically increment and continue the expected sequence.
- **Reflective Display**: Any updates to a task code are immediately reflected in the UI—especially in the product catalog and its category structure.

---

### 🛠️ Manual Overrides

You can override a task code to manually control the order of items:
1. From the main menu, go to **System Defaults → Catalog**.
2. Select the catalog you want to edit by clicking on its name.
3. Locate the item you want to reorder and click on its **Code** field.
4. Enter a new numeric value to adjust its position.
5. The layout updates in real-time to reflect your changes.

> **Tip**: Use numeric gaps in task codes (e.g., 10, 20, 30) to make it easier to insert new items later without renumbering everything.

---

### 🧭 Catalog-Level Task Code Behavior

When a **new catalog** is created, the system applies the following logic for task code sequencing:

- Task code numbering **continues** as long as the **Category Code** and **Subcategory Code** remain the same.
- If there is a **change** in either the **Category Code** or **Subcategory Code**, the task code **resets back to 1** for that new group.
- This ensures task codes remain grouped and ordered correctly within each section of the catalog.

> **Example**:  
> - Items in Category A → Subcategory A will have task codes: 1, 2, 3...  
> - If the next item is in Category A → Subcategory B, the sequence resets: 1, 2...  
> - If another item returns to Category A → Subcategory A, the next task code continues from the last in that group.

---

This structure ensures that task codes reflect meaningful order within each catalog group, making the catalog easier to manage and navigate.
