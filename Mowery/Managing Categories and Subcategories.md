
# 🗂️ Managing Categories and Subcategories

This guide explains how to manage categories and subcategories in the system, including how to assign types such as HVAC or Plumbing.

---
## 🏷️ Specify a Type for Each Category

To create a new category and assign it a type:

1. From the main menu, go to **Service Calls**.

2. From the top navigation menu, go to **Category**.

3. Click **New Item** to create a new category.

4. In the **Category Name** field, enter the desired name.

5. In the **Type** field, enter either `HVAC` or `Plumbing`.

> **Note**: The **Type** field is a plain text attribute that exists only on the **Category** table. It helps distinguish between categories with the same name.

---
## 🧩 Use Duplicate Category Names with Different Types

The system allows multiple categories to share the same name if each has a different **Type**.

**Examples:**

- `Miscellaneous` (Type: HVAC)

- `Miscellaneous` (Type: Plumbing)

These are treated as distinct categories in the system.

---
## 📂 Assign Subcategories to Categories

To link a subcategory to a parent category:

1. From the main menu, go to **Service Calls**.

2. From the top navigation menu, click **Sub Category**.

3. Select the subcategory. 

4. From the **Category** dropdown, select the appropriate category that this subcategory belongs to.

> The category dropdown includes the category name only. You should be aware of each category’s type when making a selection.  

> The subcategory automatically inherits the **Type** from its parent category.  

> **Important**: The **Type** field is not used in the **Subcategory** table.

---

## 📦 Assign Products to a Subcategory

All products must be assigned to a subcategory.

- If no specific subcategory applies, assign the product to a `Miscellaneous` subcategory under the appropriate category **Type** (e.g., *Miscellaneous (HVAC)* or *Miscellaneous (Plumbing)*).
