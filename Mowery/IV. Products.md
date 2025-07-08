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

## View Product List and Details

### Open the Product List

1. From the main menu, go to **System Defaults → Products**.
    
2. The **Product List** screen appears, showing all available products.
    

### 📦 View a Product’s Details

1. Locate the product you want to review.
    
2. Click the **leftmost button** in the product row to open the **Product Detail** page.
    

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

|Field|Example|
|---|---|
|**Standard Rate**|`$349.25 → $349`|
|**Value Rate**|`$289.80 → $290`|
|**Add-On Standard**|`$59.49 → $59`|
|**Add-On Value**|`$45.51 → $46`|

### How It Works

- `.50` and above rounds **up**
    
- Below `.50` rounds **down**
    
- Only **displayed values** are rounded
    
- Exact values are stored and used for calculations
    

All changes appear in the **Price History Tracking** panel.

---

## View Product Price History

Track price updates in the **Price History Tracking** panel.

### 🕘 Steps

1. Go to **System Defaults → Products**.
    
2. Select a product.
    
3. Find the **Price History Tracking** panel (upper-right corner).
    

### What You’ll See

|Field|Description|
|---|---|
|**Effective Date**|Date when pricing was updated|
|**Revision**|Version number|
|**Standard Rate**|Regular sale price|
|**Value Rate**|Value-based sale price|
|**Add-On Standard**|Standard price for add-ons|
|**Add-On Value**|Value-based price for add-ons|
|**Commercial**|Commercial pricing|

> **Note:** All pricing updates are automatically logged for auditing.

---

##  Terminology Reference

|Term|Definition|
|---|---|
|**Standard Rate**|Default price used in regular sales|
|**Value Rate**|Discounted or promotional price|
|**Commercial Rate**|Bulk or wholesale price|
|**Add-On Standard**|Add-on pricing under the standard rate|
|**Add-On Value**|Add-on pricing under the value rate|
|**Catalog**|Product price list with an effective date (also called **Price Book**)|
|**Effective Date**|Date when pricing becomes active|
|**Reset Icon**|Circular arrow used to undo manual changes|
|**Price History Tracking**|Section that logs pricing changes|

---

##  Need Help?

📞 If price rounding seems incorrect or you need help updating prices, contact your system administrator or support team.