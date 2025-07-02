# 💵 Managing Product Pricing

This guide explains how to update product pricing, how automatic price rounding works, and how to track pricing changes using the **Price History Tracking** panel.

You can:

- Manually update product pricing fields
    
- Revert changes using the reset icon
    
- Understand how rounding affects displayed prices
    
- Track price changes in the **Price History Tracking** panel
    

These tools help maintain accurate, consistent pricing across your product catalog.

---

## 🔗 Quick Links

- [Edit Product Pricing](#edit-product-pricing)
    
- [Automatic Price Rounding](#automatic-price-rounding)
    
- [View Product Price History](#view-product-price-history)
    

---

##  Edit Product Pricing

You can manually update product pricing in the **Current Pricing** section. All updates are tracked in the **Price History Tracking** panel.

### How to Edit Pricing

1. Go to **System Defaults → Products**.
    
2. Select a product by clicking the **leftmost button** next to its name.
    
3. In the **Current Pricing** section, update any of the following fields:
    
    - **Standard Rate** — Default price for regular sales.
        
    - **Value Rate** — Price for value-based pricing.
        
    - **Commercial Rate** — Price for commercial or bulk transactions.
        
4. When a price field changes:
    
    - A **reset icon** (rounded arrow) appears next to the field.
        
    - Click the reset icon to revert to the system-calculated default.
        

> **Note:**  
> Product-level pricing changes automatically apply to any catalogs using the product.

All pricing updates are recorded in the **Price History Tracking** panel on the product detail page.

---

##  Automatic Price Rounding

The system simplifies pricing by rounding certain fields to the **nearest whole dollar**. Rounding affects only the displayed price—internal calculations continue using exact decimal values.

### Price Fields Affected

|Field|Example|
|---|---|
|**Standard Rate**|`$349.25 → $349`|
|**Value Rate**|`$289.80 → $290`|
|**Add-On Standard**|`$59.49 → $59`|
|**Add-On Value**|`$45.51 → $46`|

---

### Rounding Behavior

- The system uses **standard rounding rules**:
    
    - `.50` and above rounds **up**
        
    - Below `.50` rounds **down**
        
- Only the displayed price is rounded. Backend calculations remain precise.
    
- All price changes appear in the **Price History Tracking** panel.
    

---

## View Product Price History

You can view a record of all price changes for a product using the **Price History Tracking** panel.

### How to View Price History

1. Go to **System Defaults → Products**.
    
2. Click the **leftmost button** next to the product name.
    
3. Locate the **Price History Tracking** panel in the upper-right corner.
    

---

### What the Panel Shows

The **Price History Tracking** panel displays a list of price updates, including:

|Field|Description|
|---|---|
|**Effective Date**|Date when the price change became active.|
|**Revision**|Version number or update identifier.|
|**Standard Rate**|Price for regular sales.|
|**Value Rate**|Price for value-based pricing.|
|**Add-On Standard**|Add-on price under standard pricing.|
|**Add-On Value**|Add-on price under value pricing.|
|**Commercial**|Price for commercial or bulk sales.|

> **Note:**  
> All pricing field changes are automatically recorded for auditing and reference.

---

## 📞 Need Help?

If price rounding behaves unexpectedly or you need assistance updating pricing, contact your system administrator or support team.