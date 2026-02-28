# 🌍 Indian States REST API

A simple **Express.js REST API** to manage Indian states data like population, literacy rate, GDP, and annual budget.

Built for learning **CRUD operations**, routing, and REST concepts.

---

## 🚀 Setup

```bash
npm install
node index.js
```

Server runs on:

```
http://localhost:5000
```

---

## 📦 State Object Structure

```json
{
  "id": 1,
  "name": "Gujarat",
  "population": 63872399,
  "literacyRate": 78.03,
  "annualBudget": 243965,
  "gdp": 21000000
}
```

---

# 🔗 API Routes

## 🟢 GET Routes (Read Data)

### 1️⃣ Get all states

```
GET /states
```

Returns complete list of states.

---

### 2️⃣ Get state by ID

```
GET /states/:id
```

Returns a single state using its ID.

---

### 3️⃣ Get state with highest GDP

```
GET /state/highest-gdp
```

Returns the state having maximum GDP.

---

## 🔵 POST Route (Create Data)

### 4️⃣ Add new state

```
POST /states
```

Adds a new state record.

**Body Example**

```json
{
  "name": "New State",
  "population": 1000000,
  "literacyRate": 80,
  "annualBudget": 50000,
  "gdp": 2000000
}
```

---

## 🟡 PUT Routes (Replace Data)

### 5️⃣ Replace entire state

```
PUT /states/:id
```

Replaces full state object.

---

### 6️⃣ Update annual budget only

```
PUT /states/:id/budget
```

**Body**

```json
{
  "annualBudget": 300000
}
```

---

### 7️⃣ Replace population value

```
PUT /states/:id/population
```

**Body**

```json
{
  "population": 5000000
}
```

---

## 🟠 PATCH Routes (Partial Update)

### 8️⃣ Update literacy rate

```
PATCH /states/:id/literacy
```

---

### 9️⃣ Update GDP

```
PATCH /states/:id/gdp
```

---

### 🔟 Update any fields

```
PATCH /state/:id
```

Updates any provided properties dynamically.

---

## 🔴 DELETE Routes

### 1️⃣1️⃣ Delete state by ID

```
DELETE /states/:id
```

---

### 1️⃣2️⃣ Delete state by name

```
DELETE /states/name/:stateName
```

---

### 1️⃣3️⃣ Delete states with low literacy rate

```
DELETE /states/low-literacy/:percentage
```

Deletes all states where literacy rate is below given value.

---

## 🛠 Tech Stack

* Node.js
* Express.js
* CORS
* REST API

---

## 🎯 Purpose

* Learn REST APIs
* Practice CRUD operations
* Understand Express routing
* Work with JSON data

---
Deployed Api Url on Render:https://state-statistics-management-api-zaas.onrender.com/states

-----------------------
Api documentation on postman:https://documenter.getpostman.com/view/50869229/2sBXcHiJmJ

⭐ Feel free to fork, modify, or improve.
