# Notes for Computer Networking: A Top-down Approach

## Table of Contents

1. [Computer Networks and the Internet](#computer-networks-and-the-internet)
2. [Application Layer](#application-layer)
3. [Transport Layer](#transport-layer)
4. [Network Layer: Data Plane](#network-layer-data-plane)
5. [Network Layer: Control Plane](#network-layer-control-plane)
6. [The Link Layer and LANs](#the-link-layer-and-lans)
7. [Wireless and Mobile Networks](#wireless-and-mobile-networks)
8. [Security in Computer Networks](#security-in-computer-networks)
9. [Multimedia Networking](#multimedia-networking)

---

## 1. Computer Networks and the Internet

### 1.1 What is the Internet?

#### 1.1.2 A Services Description

The 'Internet' is a computer network that connects billions of computing devices globally:

- All devices connected to the internet are called "hosts" or "end systems"
- End systems provide a **socket interface** that specifies how programs running should communicate with the Internet infrastructure to deliver data to destination programs on other end systems

> **Socket Interface**: The interface between the application layer and the transport layer (set of rules that an application must follow to use the transport layer) — more on this in the Application Layer chapter

**Simple analogy:**

Suppose Alice wants to send a letter to Bob using postal service. Steps Alice will take:

1. Write letter
2. Put letter in envelope
3. Write Bob's address on envelope
4. Put stamp on envelope
5. Put letter in mailbox
6. Postal service picks up letter
7. Postal service delivers letter to Bob

In this case, postal service has its own "postal service interface"/set of rules that Alice has to follow.
Similarly, the Internet has a socket interface that a program sending data has to follow in order to deliver the data to the endpoint.

#### 1.1.3 What is a Protocol?

**A Human Analogy:**

Suppose you want to ask a stranger for the time of day, a protocol would be:

1. You greet stranger
2. Stranger either greets you back or ignores you
3. You ask for time
4. Stranger tells you time
5. You thank stranger

In this protocol, there are specific messages sent and specific actions we take in response to the received replies or actions. If people use different protocols (e.g., if one person has manners but the other doesn't), the protocols will fail and you get nowhere (no work is done).

Similarly, in computer networking, it takes two or more communicating entities using the same protocol to accomplish a task.

**Network Protocols:**
Similar to human protocol analogy, except entities exchanging messages and taking actions are hardware/software components of an end system or network.
