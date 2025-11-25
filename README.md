# HTTP vs REST API

## 🧠 What is HTTP?

HTTP (HyperText Transfer Protocol) is the communication protocol used by the web.

It defines:
- How clients and servers talk
- Methods like GET, POST, PUT, DELETE
- How messages are sent and received

HTTP is low-level and does not tell you:
- how to structure your API
- how to name routes
- how to represent resources
- how to organize CRUD operations

### Example HTTP request:

```
GET /products
```

HTTP only defines how the GET request works — not what `/products` means.

---

## 🚀 What is a REST API?

A REST API (Representational State Transfer) is an architecture for building web APIs on top of HTTP.

REST defines:
- how to design clean, consistent URLs
- how to properly use HTTP methods
- how to structure data (usually JSON)
- how client → server communication should work
- stateless communication

REST turns raw HTTP into a well-organized API system.

### Example REST API:

| HTTP Method | REST Meaning | Example Endpoint |
|---|---|---|
| GET | Read/FETCH | `/users` |
| POST | Create | `/users` |
| PUT | Update | `/users/1` |
| DELETE | Delete | `/users/1` |

REST gives clear meaning to HTTP methods.

---

## 🆚 HTTP vs REST — The Difference

| Feature | HTTP (Protocol) | REST (API Architecture) |
|---|---|---|
| What it is | Communication protocol | Way to design APIs |
| Defines URL structure? | ❌ No | ✔ Yes |
| Defines CRUD behavior? | ❌ No | ✔ Yes |
| Uses JSON? | ❌ Not required | ✔ Common |
| Organizes data? | ❌ No | ✔ Yes |
| Predictable routes | ❌ Hard | ✔ Easy |
| Stateless? | Optional | Always |
| Used for? | Low-level communication | Web APIs, microservices |

---

## 🧩 Easy Analogy

**🛣️ HTTP = The road**
Defines rules of driving (left/right, speed, signals)

**🚗 REST = The car**
Uses the road rules but gives structure, purpose, and direction.

HTTP is the foundation. REST APIs are built on top of HTTP.

---

## 🎯 Why Use REST Instead of Raw HTTP?

### ✔ 1. Standardized API design

Everyone knows:
- GET → fetch
- POST → create
- PUT → update
- DELETE → remove

### ✔ 2. Predictable endpoints

REST encourages clear URLs:

```
/users
/users/:id
/products
/products/:id
```

### ✔ 3. JSON-based responses

REST commonly responds with JSON:

```json
{ "id": 1, "name": "Praveen" }
```

### ✔ 4. Easy to scale

Microservices communicate via REST.

### ✔ 5. Easy for frontend/mobile developers

Stable, consistent structure.

### ✔ 6. Stateless (no server memory needed)

Every request contains everything needed.

---
https://www.notion.so/REST-API-2883f465f01d80c99b2acda2b9f4cf66?source=copy_link

## 📌 Summary

- **HTTP** is a communication protocol.
- **REST** is a design pattern that uses HTTP properly.
- **REST** gives structure, conventions, predictability, and makes APIs easy to use and maintain.
- **Modern applications** use REST because raw HTTP alone is too unstructured and hard to maintain.
