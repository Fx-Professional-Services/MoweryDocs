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
    
- [Automatic Price Rounding](#automatic-price-rounding-and-manual-overrides)
    
- [View Product Price History](#view-product-price-history)

* [Terminology Reference](#terminology-reference)
    

---

##  Edit Product Pricing

You can manually update product pricing in the **Current Pricing** section. All updates are tracked in the **Price History Tracking** panel.

### ✏️ How to Edit Pricing

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
## Automatic Price Rounding and Manual Overrides

The system simplifies displayed pricing by rounding certain fields to the **nearest whole dollar**. However, when you manually override a price, your exact entered value is preserved without rounding.

---
### 🎯 Price Fields Affected by Rounding

|Field|Example|
|---|---|
|**Standard Rate**|`$349.25 → $349`|
|**Value Rate**|`$289.80 → $290`|
|**Add-On Standard**|`$59.49 → $59`|
|**Add-On Value**|`$45.51 → $46`|

**Rounding Rules:**

- `.50` and above rounds **up**
    
- Below `.50` rounds **down**
    
- Rounding applies only to the displayed price. Backend calculations use the precise decimal value.
    
- All price changes appear in the **Price History Tracking** panel.
    

---
### Manual Price Overrides

If you manually override a price in the system, the exact value you enter is preserved. The rounding function does **not** apply to manual price entries.

For example:

- If you enter `$42.50` as a manual price, the system displays `$42.50` without rounding.
    
- This ensures manual entries, such as diagnostic fees, remain accurate and are not altered by automatic rounding.
    
> **Note:** Manual price entry does not interfere with existing markup calculations for other pricing fields.
---

## View Product Price History

You can view a record of all price changes for a product using the **Price History Tracking** panel.

### 🕘 How to View Price History

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

## Terminology Reference

|Term|Meaning|
|---|---|
|**Standard Rate**|The default product price used for regular sales.|
|**Value Rate**|Discounted or promotional product price, often for special offers.|
|**Commercial Rate**|Price applied to business, wholesale, or bulk purchases.|
|**Add-On Standard**|Price for optional add-ons or services under standard pricing.|
|**Add-On Value**|Price for optional add-ons when the product uses value-based pricing.|
|**Catalog**|Also called a **Price Book**; a product price list with an effective date.|
|**Effective Date**|Date when a new price or catalog becomes active.|
|**Reset Icon**|A button (circular arrow) to undo manual pricing changes.|
|**Price History Tracking**|A record showing all pricing updates made to a product.|


## 📞 Need Help?

If price rounding behaves unexpectedly or you need assistance updating pricing, contact your system administrator or support team.