# 🧱 OSI Model

The **OSI Model** (Open Systems Interconnection) is a framework that explains how data moves from one device to another across a network — in **7 layers**.

Each layer has a specific role. Together, they help standardize communication between systems, no matter what hardware, software, or operating systems they use.

---

## 🚦 How Data Flows in the OSI Model

When data is sent between two devices:

- It **goes down** through all 7 layers on the **sender's** side  
- Then it **climbs back up** through the 7 layers on the **receiver's** side

### 🧭 Step-by-Step Flow

7. **Application Layer** – The user or app creates the message (e.g. a chat message)
6. **Presentation Layer** – The data is formatted and possibly encrypted
5. **Session Layer** – A connection is opened and managed
4. **Transport Layer** – The message is broken into smaller chunks (segments)
3. **Network Layer** – Each segment is packaged with an IP address and becomes a packet
2. **Data Link Layer** – Each packet is framed and given a MAC address
1. **Physical Layer** – The frames are converted into bits and transmitted physically

---

## 7️⃣ Application Layer

Provides network services directly to the user or software applications (e.g., browsers, email clients).  
**Examples:** HTTP, FTP, SMTP, DNS

---

## 6️⃣ Presentation Layer

Responsible for data formatting, encryption, and compression so the receiving device can understand the data.  
**Examples:** SSL/TLS, JPEG, ASCII, MPEG

---

## 5️⃣ Session Layer

Manages sessions between applications — handles opening, maintaining, and closing connections.  
**Examples:** NetBIOS, PPTP

---

## 4️⃣ Transport Layer

Ensures reliable delivery of data between devices using segmentation, error correction, and port addressing.  
**Examples:** TCP, UDP

---

## 3️⃣ Network Layer

Handles routing and addressing to move data between different networks using IP addresses.  
**Examples:** IP, ICMP  
**Devices:** Routers

---

## 2️⃣ Data Link Layer

Ensures error-free transfer between two devices on the same network using MAC addressing and framing.  
**Examples:** Ethernet, ARP  
**Devices:** Switches

---

## 1️⃣ Physical Layer

Transmits raw binary data (bits) over physical media like cables or radio waves.  
**Examples:** Ethernet cables, fiber optics  
**Devices:** Hubs, modems

---

## 📋 Quick Summary Table

| Layer | Name             | Data Unit | Description                                |
|-------|------------------|-----------|--------------------------------------------|
| 7     | Application       | Data      | User interface & application protocols     |
| 6     | Presentation      | Data      | Formats, encrypts, and compresses data     |
| 5     | Session           | Data      | Manages sessions between devices           |
| 4     | Transport         | Segments  | Reliable delivery, flow & error control    |
| 3     | Network           | Packets   | Routing, IP addressing                     |
| 2     | Data Link         | Frames    | MAC addressing, error checking             |
| 1     | Physical          | Bits      | Sends raw bits over cables or air          |

---

## 🧠 Tip to Remember the Order:

> **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way  
> *(Physical, Data Link, Network, Transport, Session, Presentation, Application)*
