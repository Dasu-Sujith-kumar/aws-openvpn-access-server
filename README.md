# PRIVACY SHIELD: A User-Friendly VPN Client

This project demonstrates how to deploy a secure, user-accessible VPN using **OpenVPN Access Server** hosted on **AWS EC2**, offering encrypted internet access for remote clients.

## 🔐 Features
- Secure VPN via OpenVPN Access Server
- Hosted on AWS EC2 (Free Tier eligible)
- Admin and Client web interfaces
- DNS routing and subnet access control
- Scalable and cost-effective infrastructure

## ☁️ Tools & Technologies
- **AWS EC2**
  - OpenVPN Access Server AMI
  - Security Groups, Key Pairs
- **OpenVPN Access Server**
- **Ports Used**:
  - TCP 443 (VPN tunnel)
  - TCP 943 (Admin and Client UI)
- **Key Pair**: `vpn-key.pem`

## 🚀 Implementation Steps
1. **Launch EC2 Instance** with OpenVPN Access Server (t2.micro).
2. **Connect to EC2** via Instance Connect.
3. **Run Configuration Wizard** on first login:
   - Accept EULA, choose interfaces, set admin credentials.
4. **Access Admin UI** at: `https://<public-ip>:943/admin`
5. **Access Client UI** at: `https://<public-ip>:943`

## 🛠 Admin Panel
- Manage connected clients
- Monitor traffic and usage
- Configure protocols and routing
- Block/unblock users

## 👤 Client Access
- Download `.ovpn` config files
- Use OpenVPN Connect to establish connection
- Routes all traffic through VPN

## ✅ Testing
- Verified IP tunneling to AWS region
- DNS routing and encryption confirmed

## 📌 Conclusion
This setup demonstrates a secure and scalable way to deploy OpenVPN in the cloud using AWS Free Tier, offering encrypted connections, privacy, and simple user management.

## 📸 Screenshots
(Add screenshots of Admin UI, Client UI, and test results here)
