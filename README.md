## 🎓 My Thesis Project - Wireshark MCP server

![Status](https://img.shields.io/badge/Status-Work%20in%20Progress-yellow)

> **Thesis:** An MCP server (Node.js) where an AI autonomously translates natural language into dynamic `tshark` commands for pcap analysis.

### 💡 Project Motivation
This project **extends the `analyze_pcap_files` tool** found in the [WireMCP](https://github.com/0xKoda/WireMCP) project.

While WireMCP provides an excellent foundation for MCP-based analysis, its default tool is limited to basic 5-tuple fields (e.g., `ip.src`, `ip.dst`, `tcp.srcport`). This is insufficient for the more demanding queries required by academic scenarios (like the **Jim Kurose Wireshark Labs**), which need access to a wide variety of specific protocol fields (e.g., `http.host`, `dns.cname`).


### ✨ My Solution
The core of my project is an MCP server where the **AI client autonomously translates** a user's natural language question (e.g., "Find all CNAMEs for `www.mit.edu`") into the *exact* `tshark` display filters (`-Y`) and fields (`-e`) needed to get the answer.

This moves beyond fixed queries and allows for truly dynamic and deep packet analysis.

* **Repository:** The code is currently in a private repository pending completion and review.

### 🎓 Academic Info
* **Author:** Anastasia Dourou
* **Institution:** University of Crete
* **Department:** Computer Science Department
* **Supervisor:** Xenofontas Dimitropoulos
