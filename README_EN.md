# INTRODUCE
---
***There are no two identical fingerprints in the world***

The fingerprint is generated from the generation request of the order number. In the e-commerce business, the order number is a landmark transaction, so the generation rules of the order number have high requirements in terms of performance, uniqueness, and high availability. In our actual business, if our unique ID service is oriented to our microservices or just our own applications, then there is no problem. We can achieve this by using UUID/redis/mysql, etc., but These methods will have some problems. Fingerprint is currently used as a distributed ID generation system, a highly available globally unique ID generator. It has been verified by many companies/institutions/schools.

# Design document
---

//TODO

# SLA
---

In the internal network environment, the general configuration of the container monomer can reach 10W/s
