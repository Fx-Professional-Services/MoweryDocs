# 🗂️ Managing Categories and Subcategories

This guide explains how to manage categories and subcategories in the system, including how to assign types such as **HVAC** or **Plumbing**.

---

## 🏷️ Specify a Type for Each Category

To create a new category and assign a type:

1. From the main menu, go to **System Defaults**.
2. From the top navigation menu, select **Category**.
3. Click **New Item** to create a new category.
4. In the **Category Name** field, enter the desired name.
5. In the **Type** field, select either:
   - `HVAC`
   - `Plumbing`

> **Note:** The **Type** field is a plain text attribute stored only in the **Category** table. It distinguishes between categories with the same name.

---

## 🧩 Use Duplicate Category Names with Different Types

The system allows multiple categories to share the same name if each has a different **Type**.

Example:

- `Miscellaneous (HVAC)` → Select the type **HVAC**
- `Miscellaneous (Plumbing)` → Select the type **Plumbing**

These categories will appear in the **Category** selection list within **Sub Category**, with the type shown in the name to help distinguish them. The underlying **Type** field remains hidden from users at the selection level.

---

## 📂 Assign Subcategories to Categories

To link a subcategory to a parent category:

1. From the main menu, go to **System Defaults**.
2. From the top navigation menu, select **Sub Category**.
3. Select the subcategory you want to edit.
4. From the **Category** dropdown, select the appropriate parent category.

> The **Category** dropdown displays the category name only.  
> Be sure you recognize the correct category based on its naming convention.  
> The subcategory automatically inherits the **Type** from its parent category.  

> **Important:** The **Type** field does not exist in the **Sub Category** table.

---

## 📦 Assign Products to a Subcategory

All products must be assigned to a subcategory.

- If no specific subcategory applies, assign the product to a `Miscellaneous` subcategory under the appropriate **Type**.  
  Examples:
  - `Miscellaneous (HVAC)`
  - `Miscellaneous (Plumbing)`
