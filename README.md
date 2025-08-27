# 📘 MongoDB Practice (Day 1 - Day 6)

This repository contains my **MongoDB practice programs** completed during **Day-1 to Day-6**, where I learned and implemented various database operations such as **create, insert, update, query, and delete**.

---

## 🔹 What is MongoDB?

MongoDB is a **NoSQL database** that stores data in **JSON-like documents** instead of tables (like in SQL).
It is widely used because it is:

* Flexible (schema-less)
* Scalable
* High-performance

---

## 🔹 What is MongoDB Compass?

MongoDB Compass is a **GUI tool** for MongoDB. It allows you to:

* Create databases & collections
* Insert and view documents
* Run queries visually or using the **Filter bar**
* Perform update and delete operations

---

## 🔹 How to Create Database & Collection in Compass

1. Open **MongoDB Compass** and connect to `mongodb://localhost:27017`.
2. Click **Create Database** → give **DB Name** (e.g., `myDatabase`).
3. Add a **Collection Name** (e.g., `users`).
4. Insert documents manually or by pasting JSON.

---

## 🔹 How to Run Commands in Compass

In Compass, you don’t use `db.` prefix. Instead, you select the collection and use the **Filter/Search bar** or **Aggregation Tab**.

For example:

* **Insert Document**

  * Go to your collection → Click **Insert Document** → Paste JSON:

    ```json
    { "name": "Shreyas", "age": 22 }
    ```

* **Find Documents**

  * Use **Filter Bar**:

    ```json
    { "age": { "$gt": 18 } }
    ```

* **Update Document**

  * Go to **Documents → Update** → Paste update query:

    ```json
    { "$set": { "age": 23 } }
    ```

* **Delete Document**

  * Select the document → Click **Delete**

---

## 🔹 How to Write MongoDB Queries

Queries in MongoDB are written using **JavaScript-like syntax**.

Examples:

* Create database → `use myDatabase`
* Insert document → `db.users.insertOne({ name: "Shreyas", age: 22 })`
* Find documents → `db.users.find({ age: { $gt: 18 } })`
* Update document → `db.users.updateOne({ name: "Shreyas" }, { $set: { age: 23 } })`
* Delete document → `db.users.deleteOne({ name: "Shreyas" })`

---

