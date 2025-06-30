# 💵 Managing Product Pricing

This guide explains how to update product pricing and how the system applies automatic price rounding. It also describes how to track pricing changes using the **Price History Tracking** panel.

You can:

- Manually edit product pricing fields  
- Revert changes using the reset icon  
- Understand how rounding affects pricing display  
- Track all price updates in the **Price History Tracking** panel  

These tools help ensure pricing is accurate and consistent across your product catalog.

---

## 🔗 Quick Links

- [Edit Product Pricing](#edit-product-pricing)
- [Automatic Price Rounding](#automatic-price-rounding)

---

## Edit Product Pricing

You can manually update pricing fields for a product in the **Current Pricing** section. All updates are tracked in the **Price History Tracking** panel.

### Steps to Edit Pricing

1. From the main menu, go to **System Defaults → Products**.  
2. Select a product by clicking the **leftmost button** next to its name.  
3. In the **Current Pricing** section, update any of the following fields:
   - **Standard Rate** — The default price used for regular sales.  
   - **Value Rate** — The rate applied for value-based pricing.  
   - **Commercial Rate** — The price used for commercial or bulk transactions.  

4. When you change a field:
   - A **reset icon** (rounded arrow) appears next to the field.
   - Click the reset icon to revert the value to the system-calculated default.

> **Note:**  
> Changes made here are saved at the product level and automatically apply to any catalogs using this product.

The updated values are recorded in the **Price History Tracking** panel, located in the upper-right of the product detail page.

---

## Automatic Price Rounding

To simplify displayed pricing, the system automatically rounds certain price fields to the **nearest whole dollar**. Rounding affects only the displayed value in the user interface—internal calculations continue using precise decimal amounts.

### Price Fields Affected by Rounding

- **Standard Rate**  
  _Example:_ `$349.25 → $349`  

- **Value Rate**  
  _Example:_ `$289.80 → $290`  

- **Add-On Standard**  
  _Example:_ `$59.49 → $59`  

- **Add-On Value**  
  _Example:_ `$45.51 → $46`  

---

### Rounding Details

- The system uses **standard rounding rules**:
   - Values `.50` and above round **up**  
   - Values below `.50` round **down**  

- Rounding affects only the displayed price, not backend calculations or accounting values.  
- All price changes are logged in the **Price History Tracking** panel on the product detail page.

---

## 📞 Need Help?

If price rounding does not behave as expected or you need assistance updating product pricing, contact your system administrator or support team.

