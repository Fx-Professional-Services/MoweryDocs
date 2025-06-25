# ✏️ Edit Product Pricing

You can manually update pricing fields for a product in the **Current Pricing** section. Updates are tracked in the **Price History Tracking** panel.

---

## **Quick Links**

- [Edit Product Pricing](#edit-product-pricing)
- [Automatic Price Rounding](#automatic-price-rounding)

---

## Edit Product Pricing

### Steps

1. Go to **System Defaults → Products**.
2. Select a product by clicking the **leftmost button** next to its name.
3. In the **Current Pricing** section, update any of the following fields:
   - **Standard Rate** — Default price used for regular sales.
   - **Value Rate** — Rate used for value-based pricing.
   - **Commercial Rate** — Rate applied to commercial or bulk transactions.

4. When you edit a field:
   - A **reset icon** (rounded arrow) appears next to it, indicating the value has been manually changed.
   - Click the **reset icon** to revert the field to its original system-calculated value.

> **Note:**  
> Changes made here are saved at the product level and automatically apply to any catalogs using this product.

The updated values are recorded in the **Price History Tracking** panel located at the upper right of the product detail page.

---

## Automatic Price Rounding

To simplify displayed pricing, the system rounds applicable price fields to the **nearest whole dollar**. This affects only the displayed value in the UI—internal calculations continue using precise decimal amounts.

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

### Notes on Rounding

- Rounding follows **standard rules**:
  - `.50` and above rounds **up**
  - Below `.50` rounds **down`
- Rounding affects only the displayed value, not backend accounting or calculations.
- All price changes are logged in the **Price History Tracking** panel on the product detail page.

---

### 📞 Need Help?

If rounding does not work as expected or you need assistance editing pricing, contact your system administrator or support team.
