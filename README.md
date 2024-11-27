# url-shortener

# TASK

We need to build a **URL Shortener**. The goals are to create an application that will shorten any URL and allow navigation via the short equivalent. 

### Views Overview:
1. **Login View**
2. **Short URLs Table View**
3. **Short URL Info View**
4. **About View**

Adding some Unit tests will be a huge plus.

---

## LOGIN VIEW

- You should be able to log in using **Login** and **Password** fields.
- Authorization is required to differentiate between **Admin** and **ordinary users**.

---

## SHORT URLS TABLE VIEW

- Displays a table of all URLs and their shortened equivalents.
- **Features:**
  - **Delete records:** Only available to authorized users.
  - **Details view:** Click to navigate to the **Short URL Info View** using the correct ID.
  - **Add new URL:** Authorized users can enter a URL to convert it to a short representation. 
    - If the URL already exists, an error message should be displayed.
    - The new short URL should appear in the table automatically without page reload.

- **Access Permissions:**
  - **Authorized Users**: 
    - Can add new records.
    - Can delete records they created (URLs are unique per user).
  - **Admin Users**: 
    - Can add new records.
    - Can delete all records.
  - **Anonymous Users**:
    - Can only view the table.

- This page should be implemented with **Angular**.

---

## SHORT URL INFO VIEW

- **Access:** Not accessible to anonymous users.
- Displays detailed information about the URL:
  - **CreatedBy**
  - **CreatedDate**
  - Any other relevant fields.

---

## ABOUT VIEW

- Contains a description of your URL Shortener algorithm.
- **Access Permissions:**
  - **Everyone**: Can view this page.
  - **Admin Users**: Can edit and submit changes.

- This is a simple **Razor page** with a submit action.

---

## GUIDELINES

- Spend no more than **two days** on this task.
- If there is a technical interview, we will focus on enhancing this application and discussing your problem-solving process.
- Prioritize **refactoring** over implementing all features if needed. We value clean, clear, and well-structured code.
- Use appropriate **data structures** and **design patterns**.
- Showcase your **style** and **best practices**.
