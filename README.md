# Alliance Health Network Architecture Design

## **Project Overview**
This project focuses on planning, designing, and implementing a structured network for **Alliance Health**, a technology-driven healthcare solutions company. The goal is to optimize network performance, security, and scalability for their **head office in Colombo** and their **new branch in Matara**.

## **Network Design Requirements**
### **Head Office (Colombo) - Floor Plan:**
- **Floor 1:**
  - Reception area
  - Sales & Marketing Department (10 employees) - Wi-Fi Access Required
  - Customer Services Area (Wi-Fi Enabled)
- **Floor 2:**
  - Administration Department (30 employees)
  - HR Department (20 employees)
  - Accounting & Finance Department (15 employees)
  - Audit Department (5 employees)
  - Business Development Department (5 employees)
- **Floor 3:**
  - Video Conferencing Room
  - IT Department (60 employees)
  - Server Room (Dedicated Subnet: **10.254.10.0/24**)

### **Branch Office (Matara) - Floor Plan:**
- **Floor 1:**
  - Reception area
  - Customer Services Area (Wi-Fi Enabled)
- **Floor 2:**
  - Administration Department (10 employees)
  - HR Department (7 employees)
  - Accounting & Finance Department (8 employees)
  - IT Department (50 employees)

## **Network Design Considerations**
- **Subnet Segmentation:** Each department will have its own **unique subnet**.
- **Wi-Fi Access:**
  - The **Customer Services Areas** in both offices will have Wi-Fi connectivity.
  - **Sales & Marketing** will require Wi-Fi access to network resources.
- **Branch Connectivity:** A direct connection between **Colombo and Matara** will be established (**VPN optional**).
- **Server Room:**
  - Assigned subnet: **10.254.10.0/24**
  - Number of servers: **To be determined based on network load**
- **IP Addressing Plan:** The network designer will determine suitable IP address classes and ranges for efficient management.

## **Implementation Strategy**
1. **Subnet Allocation:**
   - Define subnet ranges for each department.
   - Assign static IPs to critical infrastructure components.
2. **Routing & Connectivity:**
   - Implement routing protocols for inter-department and branch communication.
3. **Wi-Fi Configuration:**
   - Secure wireless access points for required departments.
4. **Server Deployment:**
   - Set up servers within the **10.254.10.0/24** subnet.
5. **Security & Scalability:**
   - Implement firewalls, VLANs, and other security measures.

## **Assumptions**
- Network security policies will be defined based on company standards.
- Scalability will be considered for future expansion.
- Hardware and infrastructure will be selected based on company budget and requirements.

## **Conclusion**
This project delivers a **scalable, secure, and efficient network architecture** for **Alliance Health**, ensuring smooth operations and connectivity between the Colombo head office and the Matara branch.

