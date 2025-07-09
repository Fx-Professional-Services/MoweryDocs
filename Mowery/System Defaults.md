# ⚙️ System Defaults: Catalogs, Products, and Configuration Settings

The **System Defaults** section allows administrators to manage foundational settings in the Mowery system. This includes creating and maintaining product catalogs, editing product pricing, and configuring dropdown values such as employee lists.

> 🔒 Access to this section requires login.

---

## 📘 Contents

- [Catalog Management](#catalog-management)  
  - [Create a Catalog (Price Book)](#create-a-catalog-price-book)  
  - [Duplicate a Catalog (Manual Edits Are Preserved)](#duplicate-a-catalog-manual-edits-are-preserved)  
  - [Delete a Catalog](#delete-a-catalog)  
  - [View and Search Catalog Items](#view-and-search-catalog-items)  
  - [Edit Catalog Tax and Add-on Rates](#edit-catalog-tax-and-add-on-rates)  
  - [Manage Task Codes (Reorder Items)](#manage-task-codes-reorder-items)  
- [Product Pricing](#product-pricing)  
  - [View Product Details](#view-product-details)  
  - [Edit Product Pricing](#edit-product-pricing)  
  - [Automatic Price Rounding](#automatic-price-rounding)  
- [Configure Dropdown Lists](#configure-dropdown-lists)  
  - [Employee List](#employee-list)  
- [Terminology Reference](#terminology-reference)  


---

## 📦 Catalog Management

_This section explains how to manage catalogs or price books. Catalogs define effective pricing and include features for duplication, item searching, and item reordering._


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

# Products 
# 💵 Managing Product Pricing

This guide explains how to update product pricing, how automatic price rounding works, and how to track pricing changes using the **Price History Tracking** panel.

Use this guide to:

- Manually update product pricing
    
- Revert changes using the reset icon
    
- Understand how rounding affects displayed prices
    
- Track changes using the **Price History Tracking** panel
    

These tools help maintain accurate and consistent pricing across your product catalog.

---

## 🔗 Quick Links

- [View Product List and Details](#view-product-list-and-details)
    
- [Edit Product Pricing](#edit-product-pricing)
    
- [Automatic Price Rounding](#automatic-price-rounding)
    
- [View Product Price History](#view-product-price-history)
    
- [Terminology Reference](#terminology-reference)
    
- [Need Help?](#-need-help)
    

---

# 💵 Product Pricing

The **Products** section allows you to manage default pricing for every product in the system. Changes here affect all catalogs that use these products unless manually overridden.

---

## 📦 View Product Details

1. Go to **System Defaults → Products**.
2. Click the button on the far left of a product row to open the **Product Detail** screen.

3.  Click the **leftmost button** in the product row to open the **Product Detail** page.
    

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/d47c689033db43bc54721ff19a8efbdcc1891ab6/Mowery/1315_viewing_product_list_and_details.png" width="350" height="230">

---

## 🧾 Understand the Product Detail Sections

Each product has several sections:

### I. Product Info

Basic product classification and description.

|Field|Description|
|---|---|
|**Type**|High-level classification (e.g., HVAC, Plumbing)|
|**Category**|General function or use (e.g., Refrigerant Repairs)|
|**Subcategory**|Specific variant or application (e.g., R410A)|
|**Description**|Short summary of the product/service|
|**Savings**|Any predefined value or benefit|
|**Active**|Indicates if the product is available|

> **Purpose:** Ensures products are correctly described and easy to find during sales and service.

---

### II. Product Price Attributes

Details about how pricing is calculated.

|Field|Description|
|---|---|
|**Cost**|Base cost of the product|
|**Estimated Hours**|Labor time estimate|
|**Add-On Rate**|Rate when the product is added to another job|
|**Commercial Rate**|Rate for commercial jobs|

---

### III. Current Pricing

Displays current prices under different pricing structures.

|Field|Description|
|---|---|
|**Revision**|Pricing version|
|**Effective Date**|Date pricing was activated|
|**Standard**|Base retail price|
|**Value**|Discounted or adjusted rate|
|**Commercial**|Commercial application rate|
|**Add-On Standard**|Add-on base price|
|**Add-On Value**|Discounted add-on price|

---

### IV. Pricing Tracking and History

Shows a record of pricing updates in the **Price History Tracking** panel (top-right corner).

> **Purpose:** Allows historical review of pricing changes and version control.

---

### V. Developer Settings Tip

Enable auto-entry of **Add-On** and **Commercial** rates for new products in Developer Settings.  
This applies when using the **New Product** button.

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/d47c689033db43bc54721ff19a8efbdcc1891ab6/Mowery/1315_1_view_product_list_and_details.png" width="350" height="230">

---

### VI. Category and Subcategory

|Term|Description|
|---|---|
|**Category**|A top-level group, identified by name and type (e.g., HVAC, Plumbing). Categories can share names if their types differ.|
|**Subcategory**|Specific group under a category. Inherits its parent category's type. Required for product assignment.|

---

##  Edit Product Pricing

Manually update product pricing in the **Current Pricing** section. Updates are tracked in the **Price History Tracking** panel.

### ✏️ Steps

1. Go to **System Defaults → Products**.
    
2. Select a product.
    
3. In the **Current Pricing** section, update any of the following:
    
    - **Standard Rate**
        
    - **Value Rate**
        
    - **Commercial Rate**
        
4. When a price changes:
    
    - A **reset icon** (circular arrow) appears.
        
    - Click it to revert to the default value.
        

> **Note:** Changes automatically apply to any catalogs using the product.

---

##  Automatic Price Rounding

The system rounds displayed prices to the nearest whole dollar. Internal calculations remain precise.

### 🔁 Affected Fields

| Field             | Example          |
| ----------------- | ---------------- |
| **Standard Rate** | `$349.25 → $349` |
|                   |                  |
# FileMaker Access

## 👥 Add a New Employee (FileMaker Access)

To add a new employee in the FileMaker system:

1. From the main menu, go to **System Defaults**.

2. Click **FileMaker Access** from the top-left menu.

3. Click **New** in the upper-left corner.

   > 🆕 A new entry field will appear at the **top of the employee list**.

4. Enter the employee’s details in the new row.

5. Exit the employee file once you're done.

   > 🔄 The system will **automatically sort** the list **alphabetically by first name** after exiting the employee record.

> ✅ Use this process when onboarding new technicians or administrators into the system.

## ⚙️ Configure Dropdown Lists

Use this section to customize system dropdowns, such as the list of employees available for assignment.

### 👥 Employee List

To add a new employee:

1. From the main menu, go to **System Defaults → FileMaker Access**.
2. Click **New** in the top-left corner.
3. Enter the employee’s details in the new row at the top.
4. Exit the record. The system will automatically sort the list alphabetically by first name.

> ✅ Use this for onboarding new technicians or administrators.

---
# 📖 Terminology Reference

| Term | Description |
|------|-------------|
| **Catalog / Price Book** | A collection of product prices effective on a specific date. Also includes tax and labor settings. |
| **Effective Date** | The start date when a catalog’s prices become valid. Must be unique per catalog. |
| **Task Code** | A number that determines the order of items within a catalog. Often spaced (10, 20, 30) to allow future reordering. |
| **Product Detail** | A screen showing full information about a product, including pricing, cost, history, and classification. |
| **Standard Rate** | The typical customer-facing price for a product. |
| **Value Rate** | A discounted rate, often used for customers with agreements or promotions. |
| **Commercial Rate** | Pricing used for commercial or large-scale clients. |
| **Manual Override** | A custom price manually entered by an admin that replaces the system-calculated price. |
| **Flat Rate** | A fixed labor cost applied to a task, regardless of actual time spent. |
| **Add-On Rate** | An extra cost for value-added services, often calculated or set manually. |
| **Mobile App SA Add-On Discount** | A discount applied when a Service Agreement is purchased via the mobile app. |
| **Catalog Price Settings** | A section where labor, tax, and pricing rules are configured per catalog item. |
| **Price History** | A record of all pricing changes made to a product, showing timestamps and user activity. |
| **Update Prices Except Manually Modified Ones** | Applies new pricing rules to system-calculated prices only, preserving manual overrides. |
| **Update All Prices (Overwrite Manual Changes)** | Applies new pricing to all items, including those with manual overrides. |
| **Dropdown List** | A selectable list used throughout the system (e.g., employees). |
| **FileMaker Access** | A configuration screen used to manage system users and employees listed in dropdowns. |