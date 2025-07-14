# 🌐 TCP/IP Model

The **TCP/IP model** is, in many ways, very similar to the **OSI model**. It’s older and serves as the foundation for real-world networking. The TCP/IP model consists of **four layers**:

- 🖥️ **Application**
- 🚦 **Transport**
- 🌍 **Internet**
- 🔌 **Network Interface**

Together, these layers cover the same functions as the seven layers of the OSI model.

---

## 📚 Layers of the TCP/IP Model

| Layer Name        | Description                                  |
|-------------------|----------------------------------------------|
| 🖥️ Application       | Interface for network applications            |
| 🚦 Transport         | Provides end-to-end communication control    |
| 🌍 Internet          | Handles routing of packets between networks  |
| 🔌 Network Interface | Manages hardware addressing and physical transmission |

> ⚠️ **Note:** Some sources split the Network Interface layer into **Data Link** and **Physical** layers (like the OSI model). This 5-layer version is popular but *not officially defined* (original 4-layer model is in [RFC 1122](https://tools.ietf.org/html/rfc1122)). Both versions are valid!

---

## ❓ Why Learn Both TCP/IP and OSI Models?

You might wonder: *If OSI isn’t used much in real networks, why learn it?*

- The OSI model is **more detailed and rigid**, making it great for learning networking theory.
- The TCP/IP model is **more practical and condensed**, used in real-world networks.

---

## 🔄 Comparing TCP/IP and OSI Models

| TCP/IP Layer       | OSI Layer Equivalent(s)             |
|--------------------|------------------------------------|
| 🖥️ Application        | Application, Presentation, Session |
| 🚦 Transport          | Transport                         |
| 🌍 Internet           | Network                          |
| 🔌 Network Interface  | Data Link, Physical              |

---

## 🛡️ Encapsulation & De-encapsulation

The process of wrapping data with protocol info (headers) works the same in both models:

- At **each layer**, a **header** is **added** during encapsulation.
- On receiving, headers are **removed** during de-encapsulation.

---

## 📖 TCP/IP: More Than Just a Model — A Suite of Protocols

TCP/IP isn’t just a model; it’s a **suite of protocols** — rules for communication.

Two main protocols give it its name:

- 🔄 **Transmission Control Protocol (TCP):** manages reliable data flow.
- 📦 **Internet Protocol (IP):** handles addressing and routing.

There are many others we will explore later.

---

## 🔗 TCP: Connection-Based Communication

TCP is a **connection-based protocol**. Before sending data, a **three-way handshake** forms a stable connection:

1. Your computer sends a **SYN** (synchronize) request.
2. The server replies with **SYN + ACK** (acknowledgement).
3. Your computer sends back an **ACK** confirming the connection.

After this, data flows reliably! Any lost or corrupted data is re-sent.

> 🧠 **Mnemonic:** *Frank Syn-acktra* — a fun way to remember SYN, SYN-ACK, ACK  
> *(Thanks to Kieran Smith, Abertay University)*

---

## 📜 History of TCP/IP and OSI Models

- Before standardization, different manufacturers had incompatible protocols.
- In 1982, the US Department of Defense introduced TCP/IP as a **universal standard**.
- The OSI model was later introduced by ISO as a **learning tool**.
- Today, TCP/IP is the **foundation of modern networking**.

