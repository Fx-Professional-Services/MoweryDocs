
# ✏️ Edit Product Pricing

You can manually update the pricing fields for a product in the **Current Pricing** section. These updates are reflected in the **Price History Tracking** panel.

### Steps

1. From the menu, go to **System Defaults → Products**.
2. Select a product by clicking the **leftmost button** next to its name.
3. In the **Current Pricing** section, update any of the following fields:
   - **Standard Rate** – The default price used for regular sales.
   - **Value Rate** – A rate used for value-based pricing.
   - **Commercial Rate** – A rate applied to commercial or bulk transactions.

4. When you edit a field:
   - A **reset icon** (rounded arrow) appears next to it, indicating the value has been manually changed.
   - Click the **reset icon** to revert the field to its original system-calculated value.

> **Note**: Changes made here are saved at the product level and automatically apply to any catalogs that use this product.

The updated values will be recorded in the **Price History Tracking** panel, located at the upper right of the product detail page.

## 🔁 Automatic Price Rounding

To simplify displayed pricing, the system automatically rounds applicable pricing fields to the **nearest whole dollar**. This affects only the visual display in the UI; internal calculations may still use the original decimal values.

## Price Fields Affected by Rounding:

- **Standard Rate**  

  _Example: $349.25 → **$349**_

- **Value Rate**  

  _Example: $289.80 → **$290**_

- **Add-On Standard**  

  _Example: $59.49 → **$59**_

- **Add-On Value**  

  _Example: $45.51 → **$46**_ 

---
## 🔎 Notes
- Rounding uses **standard rules**:

  - `.50` and above rounds **up**

  - Below `.50` rounds **down**

- Rounding affects **only the displayed value**, not backend accounting.

- All price changes are logged in the **Price History Tracking** panel at the upper right of the product detail page.

---
## 📞 Need Help?

If rounding does not behave as expected or if you need help editing pricing, contact your system administrator or support team.
