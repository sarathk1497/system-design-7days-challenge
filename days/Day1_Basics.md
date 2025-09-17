💻 Coding keeps you busy. System design keeps you unstoppable. ⚡

Welcome to Day 0 of my 7-day System Design beginner journey! Today, we’re covering the fundamentals — what system design is, its core components, requirements, and the approach.

1. What is System Design?

System design is planning how a software system works behind the scenes.
It’s about making sure the system:

•	Handles growth (scalable)

•	Keeps running even when things fail (reliable)

•	Performs well under load (efficient)

•	Think of it as designing the invisible architecture that makes your favorite apps work seamlessly.

2. How Do We Start Designing a System?

Every design starts by understanding the requirements:

•	Functional requirements: what the system should do (e.g., users can place orders)

•	Non-functional requirements: how well it should do it (e.g., handle millions of users, respond quickly)

These requirements set the foundation for every design decision.

3. What Do We Need to Design a System?

A system isn’t just code. Its building blocks include:

•	Clients: web or mobile users sending requests

•	API Gateway / Web Servers: first point of entry for requests

•	Application Servers: handle business logic

•	Database Layer: stores and retrieves data (SQL & NoSQL)

•	Cache: speeds up frequent queries (Redis, Memcached)

•	Load Balancers: distribute traffic across servers

•	Message Queues / Streaming: handle async communication (Kafka, RabbitMQ)

•	CDN: deliver static content fast globally (Cloudflare, Akamai)

•	Monitoring & Logging: track performance and detect issues

4. High-Level Design (HLD)

HLD is the big picture:

Shows main components of the system

How these components communicate

Storage and service choices
It’s like drawing the map of the system before building it.

5. Low-Level Design (LLD)

LLD dives into the details:

Class diagrams and methods

Database schema and relationships

APIs and service contracts
It’s about how each piece works and connects to others.

6. How to Approach a System Design Question

A step-by-step method makes it simple:

•	Clarify the problem

•	Estimate scale and load

•	Design the system (HLD → LLD)

•	Refine and consider trade-offs

•	Review for scalability, reliability, and performance

✅ In short:

Functional requirements = what the system does

Non-functional requirements = how well it does it

HLD = big picture architecture

LLD = detailed design
