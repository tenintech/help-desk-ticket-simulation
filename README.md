# Active Directory Setup Lab

## **Objective**
Build a basic corporate Active Directory environment with a domain controller and a domain-joined client computer.

---

## **Technologies / Environments Used**
- Windows Server
- Active Directory Domain Services (AD DS)
- Windows 10 / Windows 11
- Remote Desktop (RDP)
- Virtual Machines (Azure / VirtualBox / VMware)

---

## **Lab Steps**

### **Step 1 — Deploy Domain Controller VM**
- Create a Windows Server virtual machine
- Log into the server
- Rename the computer to:

```
DC01
```

- Restart the server

---

### **Step 2 — Install Active Directory Domain Services**
- Open **Server Manager**
- Click **Add Roles and Features**
- Select:
  - Active Directory Domain Services
- Install the role

---

### **Step 3 — Promote Server to Domain Controller**
- Click **Promote this server to a domain controller**
- Select:
  - Add a new forest
- Enter domain name:

```
company.local
```

- Complete installation and restart server

---

### **Step 4 — Create Organizational Units**
Open **Active Directory Users and Computers**

Create the following OUs:
- IT
- HR
- Finance
- Users

---

### **Step 5 — Join Client Computer to Domain**
- Deploy Windows 10 VM
- Open **System Settings**
- Join domain:

```
company.local
```

- Restart the client machine

---

## **Troubleshooting**
- Verified domain connectivity using ping
- Confirmed DNS settings
- Checked domain join status

---

## **Outcome**
Successfully deployed an Active Directory environment with:
- Domain Controller
- Organizational Units
- Domain-joined workstation

---

## **Screenshots**
*(Add screenshots here)*

Example:
![Domain Controller Setup](screenshot1.png)

---

## **Lessons Learned**
- How Active Directory environments are structured
- How domain joining works
- Importance of DNS configuration
