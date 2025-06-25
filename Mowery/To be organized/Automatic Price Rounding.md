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
