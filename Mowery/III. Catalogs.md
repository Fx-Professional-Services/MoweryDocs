# ➕ Create and Manage Catalogs

This guide explains how to create, duplicate, delete, and manage **Catalogs** (also called **Price Books**) in Mowery. Catalogs support future pricing by allowing you to maintain product price lists with effective dates. You can also update tax rates, search catalog items, and reorder products using task codes.

---

## **Quick Links**

- [Create a Catalog (Price Book)](#create-a-catalog-price-book)
    
- [Duplicate a Catalog (Manual Edits Are Preserved)](#duplicate-a-catalog-manual-edits-are-preserved)
    
- [Delete a Catalog](#delete-a-catalog)
    
- [View and Search Catalog Items](#view-and-search-catalog-items)
    
- [Edit Catalog Tax and Add-on Rates](#edit-catalog-tax-and-add-on-rates)
    
- [Manage Task Codes (Reorder Items)](#manage-task-codes-reorder-items)

* [Terminology Reference](#terminology-reference)

---

## Create a Catalog (Price Book)

➕ To create a new catalog in Mowery:

1. Go to **System Defaults → Catalog**.
    
2. Click **New Catalog**.
    
3. Enter the required details:
    
    - **Effective Date**
        
    - **Title**
        
    - **Revision**
        
    - Other required fields
        
4. Click **Add Catalog**.
    
5. A confirmation dialog appears. Click **OK** to proceed.
    
6. After processing, a success or failure message displays.
    
7. Click the catalog name to open it.
    
8. Verify the number of catalog items matches your active product list.
    

> **Note**: In Mowery, **Catalogs** and **Price Books** are the same. Catalogs store product pricing effective on the specified date.

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/1e36d159fcf3d5d763fe6d3b338c804a0fb539c6/Mowery/1_add_catalog.png" width="350" height="230">

---

### How the Effective Date Works

- The **Effective Date** is required.
    
- It must be unique and cannot duplicate a date from another catalog.
    
- When you create a catalog, the effective date copies to all catalog items automatically.
    
- If you update the effective date later:
    
    - Catalog items update to match the new date.
        
    - No update occurs if the date remains unchanged.
        
    - If the new date differs, it replaces the date in all items.
        

---

##  Duplicate a Catalog (Manual Edits Are Preserved)

Duplicating a catalog retains your manually entered values, such as custom prices and descriptions. System-generated values do not overwrite your edits.

---

### 📄 How to Duplicate a Catalog

1. Go to **System Defaults → Catalog**.
    
2. Click the white area to the right of the catalog name to select it.
    
3. Click **Duplicate Catalog**.
    
4. In the window that appears, update the catalog information if needed.
    
5. Click **Duplicate Catalog** to start duplicating.
    
6. A dialog appears stating that duplication is in progress. Click **OK**.
    
7. Another dialog appears to inform you if duplication succeeded or failed.
    
8. Click the catalog name to open it.
    
9. Verify that the number of catalog items matches the original catalog.
    

---

### Confirm Manual Edits Are Preserved

1. Manually edit a field in an existing catalog.
    
2. Follow the steps to duplicate the catalog.
    
3. Open the duplicated catalog.
    
4. Confirm your manual changes copied over to the duplicate.
    

> **Tip:** If edits do not copy, contact support or your system administrator.
---

## Delete a Catalog

### 🗑️ To delete a catalog:

1. Go to **System Defaults → Catalog**.
    
2. Select the catalog by clicking the white area on the right.
    
3. Click **Delete Catalog** at the top-left corner.
    
4. In the confirmation dialog, click:
    
    - **Delete** to confirm.
        
    - **No** to cancel.
        

> ⚠️ **Warning**: Deleting a catalog is irreversible. Ensure it is no longer needed before deletion.

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/cf0f3e9827d27e37f9617f48879e1758843db31f/Mowery/2_delete_catalog.png" width="350" height="230">

---

##  View and Search Catalog Items

You can review catalog details or search for specific items within a catalog.

### 🔍 View a Catalog

1. Go to **System Defaults → Catalog**.
    
2. Click the leftmost button next to the catalog **Code** to open **Catalog Info** and **Price Settings**.
    

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_search_catalog_items.png" width="350" height="230">

3. Edit pricing fields, tax rates, or other details.
    
4. To view catalog items, click **View Catalog**.
    

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/e7eb1bd7f50a885c571bc5516885876c05b2b61b/Mowery/1313_2_view_catalog_items.png" width="350" height="230">

---

### Search for Catalog Items

1. Go to **System Defaults → Catalog**.
    
2. Click the catalog title to open it.
    
3. In **Catalog Items**, use the search bar at the top:
    
    - Enter a **keyword**, **product code**, or **phrase**.
        
4. Press:
    
    - **Enter** (Windows)
        
    - **Return** (Mac)
        

**Search Results:**

- If no results are found, a “no results found” message appears.
    
- The full catalog item list remains accessible for browsing.
    

---

##  Edit Catalog Tax and Add-on Rates

 You can update tax rates, labor charges, and other catalog-level pricing fields in **Catalog Price Settings**.

### 💵 How to Update Rates

1. Go to **System Defaults → Catalog**.
    
2. Select a catalog.
    
3. Click the leftmost button next to the **Code** to open catalog details.
    
4. In **Catalog Price Settings**, update fields as needed:
    
    - **Tax** — Set the tax rate (`0%` for tax-exempt catalogs).
        
    - **HVAC Labor** — Labor rate for HVAC services.
        
    - **HVAC Value** — Value-based HVAC adjustment.
        
    - **Plumbing Labor** — Labor rate for plumbing.
        
    - **Plumbing Value** — Value-based plumbing pricing.
        
    - **Flat** — Flat rate adjustment for applicable items.
        
    - **Mobile App SA Add-on Discount** — Discount for mobile app service agreements.
        
5. Click **Update Price**.
    

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/d9b56235ea4e319145c9cb9665c6e1f282f52146/Mowery/1304_edit_pricing_fields.png" width="350" height="230">

---

### Apply Price Updates

1. A dialog prompts you to select how to apply the update:
    
    - **Update prices except manually modified ones** _(default)_ — System-controlled values update; manual edits stay unchanged.
        
    - **Update all prices (overwrite manual changes)** — Applies changes to all items, including manual edits.
        
2. Click **Proceed**.
    
3. Click **OK** to close the confirmation message.
    

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/6b032d293511fe3a15afb430bca112ef42504df1/Mowery/Mowery%20Documentation/1311_apply_the_price_updates.png" width="350" height="230">

> **Tip**: To preserve manual adjustments, select the default option.

---

## Manage Task Codes (Reorder Items)

**Task Codes** control the sequence of catalog items. You can adjust task codes to reorder items manually.

---

### 🔢  How Task Codes Work

- **Reordering Items** — Task codes define item order within categories and subcategories.
    
- **Automatic Assignment** — New items get the next task code automatically.
    
- **Immediate Updates** — Catalog order updates in real time after changes.
    

---

### Manually Reorder Items

1. Go to **System Defaults → Catalog**.
    
2. Click the catalog title to open it.
    
3. Find the item to reorder.
    
4. Click the item’s **Code** field.
    
5. Enter a new numeric task code.
    
6. The catalog updates automatically.
    

> **Tip**: Use gaps between task codes (e.g., 10, 20, 30) to simplify inserting new items later.

---

### Task Code Behavior by Category

Task code sequencing depends on **Category Code** and **Subcategory Code**:

|Category|Subcategory|Task Code Sequence|
|---|---|---|
|A|A|1, 2, 3...|
|A|B|1, 2...|
|A|A|4, 5...|

**Behavior Notes**:

- Task codes continue within the same category and subcategory.
    
- Changing either resets the sequence to **1** for that group.
    
- Returning to a previous group resumes the task code sequence.
    

This structure ensures catalog order stays organized and easy to manage.

____

## Terminology Reference

|Term|Meaning|
|---|---|
|**Catalog (Price Book)**|A product price list with an effective date. Both terms are interchangeable.|
|**Effective Date**|The date when a catalog’s pricing becomes active.|
|**Task Code**|A number that controls the display order of catalog items.|
|**Category Code**|A label used to group items by type or department.|
|**Subcategory Code**|A more specific grouping within a category.|
|**Mobile App SA Add-on Discount**|Discount applied for service agreements purchased via the mobile app.|
|**Update Prices Except Manually Modified Ones**|Keeps manual price changes when updating catalog rates.|
|**Update All Prices (Overwrite Manual Changes)**|Replaces all catalog item prices, including manual edits.|
