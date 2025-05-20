
# 🚀 CassOnKube: Cassandra on Kubernetes (Minikube)

**CassOnKube** is a tool that helps you quickly deploy an Apache Cassandra cluster on your **local Kubernetes setup (Minikube)** using either **VirtualBox** or **KVM** as the virtualization backend.

---

## 🔧 Features

- Automated setup of multi-node Cassandra clusters
- Works with Minikube on your local machine
- Easy customization of number of nodes and virtualization method
- Simple cleanup and monitoring tools

---

## 📦 Prerequisites

Make sure you have the following installed:

- Python 3
- pip
- Minikube
- VirtualBox or KVM
- kubectl

---

## 🛠️ Installation

```bash
git clone https://github.com/CodeMaxx/CassOnKube.git
cd CassOnKube
pip3 install -r requirements.txt
```

---

## 🚦 Usage

Start a Cassandra cluster with 4 nodes using KVM:

```bash
sudo ./main.py -s 4 -v kvm
```

**Flags:**
- `-s`: Number of Cassandra nodes (default: 3)
- `-v`: Virtualization backend (`virtualbox` or `kvm`)

To see all options:

```bash
./main.py --help
```

---

## 📁 Project Structure

- `main.py` - Orchestrates the full deployment
- `cassandra/` - Kubernetes configs for Cassandra
- `scripts/` - Helper scripts for setup and monitoring

---

## 🧹 Clean Up

To delete the Minikube cluster:

```bash
minikube delete
```

---

## 🙌 Credits

Developed by [Akash Trehan](https://github.com/CodeMaxx)  
MIT License

---

Let me know if you want a version with more advanced configuration or contribution guidelines!
