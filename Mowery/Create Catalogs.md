## ➕ Create a Catalog (Price Book)

To create a new catalog (price book) in Mowery:

1. Go to **System Defaults** → **Catalog**.
2. Click **New Catalog**.
3. In the catalog form, enter the required details:
   - **Effective Date**
   - **Title**
   - **Revision**
   - Any other required fields
4. Click **Add Catalog**.
5. A dialog appears confirming that the catalog creation is in progress. Click **OK**.
6. After processing, a second dialog confirms whether the catalog was created successfully or not.
7. Click the catalog name to open it.
8. Verify that the number of catalog items matches the number of active products.

> 📘 **Note**: In Mowery, catalogs are also referred to as **price books**. Each catalog lists product pricing that becomes effective on the specified date.

<img src="https://github.com/Fx-Professional-Services/MoweryDocs/blob/1e36d159fcf3d5d763fe6d3b338c804a0fb539c6/Mowery/1_add_catalog.png" width="350" height="230">

## How Effective Date Works

- The **Effective Date** field is **required**. You can't leave it blank.
- The entered effective date must be **unique**. It shouldn't duplicate the date used in previous catalogs.
- When a catalog is created, its effective date is **automatically copied** to all related catalog items.
- If the effective date in the catalog is changed later:
  - All catalog items update automatically to match the new date.
  - If the new date is **the same** as the existing date in the catalog items, no updates are made.
  - If the new date is **different**, it **replaces** the date in all catalog items.
