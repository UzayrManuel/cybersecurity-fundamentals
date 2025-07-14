# 🔍 Nmap Intro

When we are given an IP (or multiple IP addresses) to perform a security audit on, before we do anything else, we need to get an idea of the **“landscape”** we are attacking.

---

## 🌐 Understanding the Landscape

We need to establish which **services** are running on the targets. For example:

- One may be running a **web server**
- Another may act as a **Windows Active Directory Domain Controller**

To build this “map” of the network landscape, we begin with **port scanning**.

---

## 🧱 What Are Ports?

When a computer runs a network service, it opens a **port** to receive connections. Ports are essential for:

- Handling multiple network requests  
- Running multiple services simultaneously  

> 🧠 **Example:** When you load several web pages at once in your browser, your computer uses different **local ports** for each connection.

Network connections are made between:
- A **listening port on the server**
- A **random high-numbered port on your machine**

📌 **Example:** Your computer might use port `49534` to connect to a server’s port `443` (HTTPS).

Your computer opens up a new, random high-numbered port for each new connection.

---

## 🔢 Total Available Ports

Every computer has a total of **65,535 ports**, but many are standardized for specific services.

| 🔢 Port | 📡 Service                          |
|--------:|-------------------------------------|
| `80`    | HTTP (Web service)                  |
| `443`   | HTTPS (Secure web service)          |
| `139`   | Windows NETBIOS                     |
| `445`   | SMB (Windows File Sharing)          |

⚠️ In CTFs or hardened environments, services may run on **non-standard ports**, making **proper enumeration critical**.

---

## 🚀 Why Scanning Matters

If we don’t know which ports are open, we have **no way of interacting with services** — which means we can’t attack or assess them.

📍 That’s why we **always begin with a port scan**.

---

## 🛠️ Enter Nmap

**Nmap** is the go-to tool for port scanning and network enumeration.

It can perform many different types of scans, but the basic idea is:

> Nmap checks each port on the target to see how it responds.

---

### 📊 Common Port States

| 🔎 State      | 💡 Description                                          |
|--------------|---------------------------------------------------------|
| `Open`       | A service is actively listening on the port             |
| `Closed`     | No service is listening, but the port is reachable      |
| `Filtered`   | Port is blocked (often by a firewall)                   |

Once we know which ports are **open**, we can begin **enumerating services** — either manually, or with Nmap’s built-in service/version detection.

---

## ✅ Summary

- Begin every assessment with **port scanning**.
- Know how **ports** and **network services** work.
- Use **Nmap** to identify which ports are open and what services are running.
- Never assume default ports — always **enumerate** thoroughly.

🧰 **Nmap is an essential tool for initial enumeration and should be in every hacker's toolkit.**
