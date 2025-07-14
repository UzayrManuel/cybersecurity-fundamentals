# 🧱 OSI Model (Simplified)

The **OSI Model** (Open Systems Interconnection) is a 7-layer framework that describes how data moves from one device to another across a network. Each layer has a specific function and passes data to the layer above or below it.

This model is important for understanding how networking, security, and communication protocols operate.

---

## 🚦 How Data Flows in the OSI Model

When data is transmitted between devices:

- It moves **downward through all 7 layers** on the **sender’s** side.
- It moves **upward through the same 7 layers** on the **receiver’s** side.

### 📤 Sender → Receiver Flow

1. **Application Layer** – App creates the message  
2. **Presentation Layer** – Data is formatted/encrypted  
3. **Session Layer** – Session is established  
4. **Transport Layer** – Data is broken into segments  
5. **Network Layer** – IP address added (routing begins)  
6. **Data Link Layer** – MAC address added (framing begins)  
7. **Physical Layer** – Bits sent over wire or air  
➡ Data reaches the destination and climbs back up the stack in reverse

---

## 🔼 Layer 7: Application Layer

Provides **networking services to software applications**. This is where apps like browsers, email clients, or messengers interact with the network.  
It passes data down to the presentation layer for processing.

- 📎 Examples: HTTP, FTP, SMTP, DNS

---

## 🔁 Layer 6: Presentation Layer

**Formats and translates data** from the application layer into a standard format for transmission. Also handles:

- 🛡️ Encryption / decryption  
- 📦 Compression / decompression

This ensures the receiving system can understand and properly interpret the data.

- 📎 Examples: SSL/TLS, JPEG, ASCII, MPEG

---

## 🔗 Layer 5: Session Layer

**Establishes and manages communication sessions** between devices. Ensures that sessions are maintained, synchronized, and properly closed.

- Handles multiple sessions at once (e.g. multiple browser tabs)
- If a session can’t be created, it returns an error

- 📎 Examples: NetBIOS, PPTP

---

## 🚚 Layer 4: Transport Layer

**Ensures reliable end-to-end delivery** of data. It:

- Selects between protocols:
  - TCP (connection-oriented, reliable)
  - UDP (connectionless, faster but no guarantee)
- Splits data into:
  - **Segments** (TCP)
  - **Datagrams** (UDP)
- Adds source and destination **port numbers**
- Handles retransmission and flow control (for TCP)

- 📎 Examples: TCP, UDP

---

## 🌍 Layer 3: Network Layer

Responsible for **routing packets** across different networks using IP addresses.

- Uses **logical addressing** (e.g. IPv4: 192.168.1.1)
- Finds the most efficient route to the destination
- Converts segments into **packets**

- 📎 Examples: IP, ICMP  
- 🖧 Devices: Routers

---

## 🧱 Layer 2: Data Link Layer

Provides **node-to-node delivery** within the same local network.

- Adds **MAC addresses** to frames for physical addressing
- Formats packets into **frames** for transmission
- Checks for **errors in transmission** using checksums

- 📎 Examples: Ethernet, ARP  
- 🖧 Devices: Switches, NICs

---

## ⚙️ Layer 1: Physical Layer

The **hardware level** — this layer sends raw bits (0s and 1s) as electrical, optical, or radio signals.

- Responsible for physical transmission through cables or wireless
- Converts signals into data and vice versa

- 📎 Examples: Ethernet cables, fiber optics, radio  
- 🖧 Devices: Hubs, modems, repeaters

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

## 🧠 Tip to Remember the Layers (Top to Bottom):

> **A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing  
> *(Application, Presentation, Session, Transport, Network, Data Link, Physical)*

