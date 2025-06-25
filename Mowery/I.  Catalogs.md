# ➕ Create Catalogs

You can create multiple catalogs (price books), each with its own effective date, to support future pricing changes.

### Steps

1. Navigate to **System Defaults → Catalog**.
2. Click **New Catalog**.
3. Fill out the catalog form:
   - **Effective Date** — Specifies when the pricing should take effect.
   - **Title**
   - **Revision**
   - Any other required fields
4. Click **Add Catalog**.
5. A confirmation dialog appears that the creation process has started. Click **OK** to confirm.
6. The system creates a new catalog (price book) associated with the specified effective date.
7. After the process completes, a success or failure message appears.
8. Click the catalog name to open it.
9. Verify that the number of items matches the number of active products.

> 📌 You can create multiple catalogs with different effective dates to plan future price changes in advance.

# 🌀 Duplicate a Catalog (Manual Edits Are Preserved)


You can duplicate a catalog without losing any manually entered values. Custom prices, descriptions, and other edits will be retained—auto-filled fields won’t overwrite your data.

---
## 📋 How to Duplicate a Catalog

1. Go to **System Defaults → Catalog**.

2. Click the white area of the catalog you want to duplicate.

3. Click **Duplicate Catalog**.

4. Update the catalog info if needed.

5. Click **Duplicate Catalog** again to confirm.

6. When prompted, click **OK** to continue.

7. After processing, you’ll see a success or failure message.

8. Click the duplicated catalog to open it.

9. Confirm the number of items matches the original catalog.

---
## ✅ What You Should Know

- Manually entered values (like prices) are **kept**.

- System-generated values **won’t overwrite** your changes.

- This ensures your edits are safe when duplicating catalogs.

---

## 🔍 Quick Check

Want to be sure?

1. Change some fields manually in a catalog.

2. Duplicate it.

3. Open the new catalog and confirm your changes are still there.

---
## 🛠️ Need Help?

If you notice your edits didn’t copy over, contact support or your system admin.

# 📚 Viewing and Searching Catalog Items

## View a Catalog

1. Go to **System Defaults → Catalog**.
2. Select a catalog from the list and click the **leftmost button** next to the **Code** of the catalog to open the **Catalog Info** and **Price Settings**. 

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_search_catalog_items.png" width="350" height="230">

3. You can now modify pricing fields, tax rates, and other catalog details as needed.
4. To display the catalog item, click **View Catalog**. 

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_2_view_catalog_items.png" width="350" height="230">

---

## 🔍 Search Catalog Items

Follow these steps to search for a specific catalog item.

---

### 📍 Steps

1. Go to **System Defaults → Catalog**.
2. Select a catalog by clicking on the **Catalog Title** from the list.
3. In the **Catalog Items** section, use the **search bar** at the top of the list.
   - Enter a **keyword**, **product code**, or **phrase** related to the catalog item you're looking for.
4. Press:
   - **Enter** (Windows)  
   - **Return** (Mac)

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_search_catalog_items.png" width="350" height="230">

---

### ℹ️ Search Results

- If no matching results are found, a message will appear saying **"no results found"**.
- The full list of catalog items will still remain visible for browsing.


# Task Codes

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

