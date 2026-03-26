## 🚀 FA-SEAL: Forensic Analysis on Encrypted Audit Logs

FA-SEAL is a system that enables **forensic investigation directly on encrypted audit logs**, exposing only minimal, attack-relevant data.

Designed for scenarios where audit logs must remain confidential (e.g., cloud environments, outsourced incident response).

### ⚡ Key Highlights
- Processes ~30GB/day logs in ~90 minutes (single core)
- Discloses only **0.68% of sensitive data**
- Supports forward & backward attack tracing
- Designed for **privacy-preserving, scalable security analytics**

## ❓ Why FA-SEAL?

Traditional forensic analysis requires full access to audit logs, exposing sensitive data.

FA-SEAL solves this by:
- Keeping logs encrypted
- Revealing only attack-relevant information
- Enabling secure collaboration with external investigators

## 🏗️ System Overview

FA-SEAL follows a client–server architecture with a dedicated analysis component. FA-SEAL consists of:
- **Client**: log ingestion and encryption  
- **Server**: encrypted log storage  
- **Investigator**: query and forensic analysis  

![FA-SEAL Architecture](overview.png)

### 🔍 End-to-End Workflow

1. Logs are collected and encrypted on the client  
2. Encrypted logs are stored on the server  
3. Investigator issues queries (e.g., trace process execution)  
4. FA-SEAL reveals only relevant data for analysis  

## ⚙️ Quick Start

To get started, clone the repository and follow the setup instructions in [instruction.md].

```bash
git clone https://github.com/BasantaChaulagain/faseal
```

## 📊 Performance

- 30GB logs processed in ~90 minutes (single core, experimental setup)
- 0.68% data exposure during investigation
- Efficient forward and backward attack tracing

![Result](result.png)

## 📄 Publication

**FA-SEAL: Forensically Analyzable Symmetric Encryption for Audit Logs**. Published at *ACSAC 2024*  

🔗 [Read the paper](https://ieeexplore.ieee.org/document/10917745)

### 📌 Citation

```
@article{Chaulagain2024FASEAL,
  title={FA-SEAL: Forensically Analyzable Symmetric Encryption for Audit Logs},
  author={Basanta Chaulagain and Kyu Hyung Lee},
  journal={2024 Annual Computer Security Applications Conference (ACSAC)},
  year={2024},
  pages={716-732},
  url={https://ieeexplore.ieee.org/document/10917745}
}
```