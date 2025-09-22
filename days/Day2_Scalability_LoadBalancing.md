# ⚡ Day 2 - Non-Functional Requirements: Scalability & Load Balancing

💻 Coding solves problems.  
⚡ System design ensures those problems don’t break the system at scale.

---

## 🔹 Step 1: Non-Functional Requirements Recap

Non-Functional Requirements (NFRs) define **how well** a system should perform:

- **Scalability** – handle growth in users/data/traffic  
- **Availability** – system stays up and running  
- **Reliability** – consistent and fault-tolerant  
- **Performance** – fast response under load  
- **Maintainability** – easy to extend and update  
- **Security** – protects data and users  

---

## 🔹 Step 2: Scalability & Load Balancing

### What is Scalability?

Scalability = **ability to handle increasing load without breaking**.

**Types of Scalability:**

1. **Vertical Scaling (Scale-Up)** – add more CPU, RAM, storage to a single server  
2. **Horizontal Scaling (Scale-Out)** – add more servers to share the load  

### What is Load Balancing?

Load Balancer = **distributes traffic across multiple servers** to prevent overload and improve performance.

---

       ┌─────────────┐
       │   Client    │
       └─────┬──────┘
             │
       ┌─────▼──────┐
       │   Server   │
       │  ↑ CPU     │
       │  ↑ RAM     │
       │  ↑ Storage │
       └────────────┘
