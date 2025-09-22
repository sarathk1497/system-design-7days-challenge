# ⚡ Day 1 - Non-Functional Requirements: Scalability & Load Balancing

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

Types of Scalability:

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

- Single server is upgraded to handle more requests  
- Simple approach but limited by hardware capacity  

---

## 🔹 Step 4: Diagram - Horizontal Scaling with Load Balancer

             ┌─────────────┐
             │   Client    │
             └─────┬──────┘
                   │
           ┌───────▼────────┐
           │ Load Balancer  │
           └───────┬────────┘
       ┌───────────┼───────────┐
       │           │           │
  ┌────▼────┐ ┌────▼────┐ ┌────▼────┐
  │ Server 1│ │ Server 2│ │ Server 3│
  │  Cache  │ │  Cache  │ │  Cache  │
  └─────────┘ └─────────┘ └─────────┘

- Client requests go to Load Balancer  
- Load Balancer distributes requests across multiple servers  
- Each server may have a cache for faster responses  
- Horizontal scaling allows **adding servers as traffic grows**  

---

## 🔹 Step 5: Why it Matters

- **Vertical Scaling** → simple, short-term solution  
- **Horizontal Scaling + Load Balancer** → scalable, reliable, and used in production systems  
- Ensures smooth user experience even with **millions of users**  

---

✅ **Quick Recap**:

- **Functional requirements** = what the system does  
- **Non-functional requirements** = how well it does it  
- **Scalability** = grow without breaking  
- **Load Balancer** = distribute traffic smartly for reliability and performance  

## 🔹 Step 3: Diagram - Vertical Scaling (Scale-Up)

