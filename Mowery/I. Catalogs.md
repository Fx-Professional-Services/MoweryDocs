# ➕ Create and Manage Catalogs

You can create multiple catalogs (price books) with effective dates to support future pricing changes. This guide explains how to create catalogs, duplicate them, search catalog items, and manage task codes.

---

## **Quick Links**

- [Create a Catalog](#create-a-catalog)
- [Duplicate a Catalog (Manual Edits Are Preserved)](#duplicate-a-catalog-manual-edits-are-preserved)
- [View and Search Catalog Items](#view-and-search-catalog-items)
- [Task Codes (Reordering Items)](#task-codes-reordering-items)

---

## Create a Catalog

You can create multiple catalogs with different effective dates to plan future price changes.

### Steps

1. Go to **System Defaults → Catalog**.
2. Click **New Catalog**.
3. Fill out the catalog form:
   - **Effective Date** — Specifies when the pricing takes effect.
   - **Title**
   - **Revision**
   - Any other required fields.
4. Click **Add Catalog**.
5. When prompted, click **OK** to confirm.
6. The system creates a new catalog associated with the specified effective date.
7. After processing, a success or failure message appears.
8. Click the catalog name to open it.
9. Verify the number of items matches the number of active products.

> 📌 You can create multiple catalogs with different effective dates to prepare for future price changes.

---

## Duplicate a Catalog (Manual Edits Are Preserved)

You can duplicate a catalog without losing manually entered values. Custom prices, descriptions, and other edits are retained—system auto-filled fields will not overwrite your data.

### How to Duplicate a Catalog

1. Go to **System Defaults → Catalog**.
2. Click the white space of the catalog you want to duplicate.
3. Click **Duplicate Catalog**.
4. Update the catalog details if needed.
5. Click **Duplicate Catalog** again to confirm.
6. When prompted, click **OK**.
7. After processing, a success or failure message appears.
8. Click the duplicated catalog to open it.
9. Confirm the number of items matches the original catalog.

### What You Should Know

- Manually entered values (such as prices) are **kept**.
- System-generated values will **not overwrite** your changes.
- Your edits are safe when duplicating catalogs.

### Quick Check

Want to confirm your edits were preserved?

1. Change some fields manually in a catalog.
2. Duplicate the catalog.
3. Open the new catalog and confirm your changes are still present.

### Need Help?

If your edits didn’t copy over, contact support or your system administrator.

---

##  View and Search Catalog Items

You can view and modify catalog details, or search for specific items within a catalog.

### View a Catalog

1. Go to **System Defaults → Catalog**.
2. Select a catalog and click the **leftmost button** next to the **Code** to open **Catalog Info** and **Price Settings**.

   ![View Catalog Button](https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_search_catalog_items.png)

3. Modify pricing fields, tax rates, and other catalog details as needed.
4. To display catalog items, click **View Catalog**.

   ![View Catalog Items](https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_2_view_catalog_items.png)

---

###  Search Catalog Items

Follow these steps to search for specific items:

1. Go to **System Defaults → Catalog**.
2. Click the **Catalog Title** to open the catalog.
3. In the **Catalog Items** section, use the **search bar** at the top.
   - Enter a **keyword**, **product code**, or **phrase**.
4. Press:
   - **Enter** (Windows)
   - **Return** (Mac)

   ![Search Catalog Items](https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_search_catalog_items.png)

### Search Results

- If no results are found, a **"no results found"** message appears.
- The full catalog item list remains available for browsing.

---

## Task Codes (Reordering Items)

Task Codes control the sequence of items within a product catalog. You can adjust these numeric values to reorder items manually.

### Functionality Overview

- **Reordering Tasks**: Task codes define the display order within each category and subcategory.
- **Automatic Sequencing**: New items are automatically assigned the next task code in sequence.
- **Immediate Display Updates**: Changes to task codes update the catalog order in real-time.

---

### Manual Overrides

To reorder items manually:

1. Go to **System Defaults → Catalog**.
2. Select the catalog by clicking its name.
3. Find the item you want to reorder.
4. Click its **Code** field.
5. Enter a new numeric value to adjust its position.
6. The catalog updates automatically.

> **Tip**: Use gaps in task codes (e.g., 10, 20, 30) to simplify inserting new items later.

---

### Catalog-Level Task Code Behavior

When creating a new catalog:

- Task codes continue as long as **Category Code** and **Subcategory Code** remain unchanged.
- If **Category Code** or **Subcategory Code** changes, task codes reset to **1** for the new group.

**Example**:

| Category | Subcategory | Task Code Sequence |
|----------|-------------|-------------------|
| A        | A           | 1, 2, 3...        |
| A        | B           | 1, 2...           |
| A        | A           | 4, 5...           |

This structure ensures task codes stay meaningful and organized within each catalog group.

---
