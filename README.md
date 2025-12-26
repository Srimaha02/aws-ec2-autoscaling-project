# AWS EC2 Auto Scaling Project 🚀

**Repository:** https://github.com/Srimaha02/aws-ec2-autoscaling-project

---

## 🧠 Project Overview

This project demonstrates a **working Amazon EC2 Auto Scaling setup** using AWS.  
Auto Scaling automatically ensures that the right number of EC2 instances are running to handle demand — healing itself when instances fail.

You will see:
✔ Launch Template created  
✔ Auto Scaling Group created  
✔ Running EC2 instance  
✔ Auto-healing by terminating an instance  
✔ Replacement instance launched automatically

---

## 🛠 Tools & Technologies

| Cloud Service | Purpose |
|---------------|---------|
| AWS EC2 | Virtual servers in cloud |
| EC2 Auto Scaling | Automatically maintain instance count |
| Launch Template | Template for launching EC2 instances |
| AWS Console | Management UI |
| GitHub | Project documentation |

---

## 📊 Architecture (Diagram)

> *Add your architecture diagram below once created.*

+------------------------+
| Auto Scaling Group |
| (Min=1, Max=2) |
| |
| +----------------+ |
| | EC2 Instance | |
| | (Running) | |
| +----------------+ |
+------------------------+

yaml
Copy code

---

## 🚀 Step-by-Step Setup

### 1. **Create Key Pair**
- AWS Console → EC2 → Key Pairs → Create
- Download `.pem` file for SSH if needed later

### 2. **Create Launch Template**
- EC2 → Launch Templates → Create
- Use Amazon Linux 2 (Free Tier)
- Select instance type: `t2.micro`
- Attach key pair

### 3. **Create Auto Scaling Group**
- EC2 → Auto Scaling Groups → Create
- Select Launch Template
- Select subnets (at least 2 for high availability)
- Set capacity: Min=1, Desired=1, Max=2

---

## 📸 Project Screenshots

### ✔ Launch Template Created


### ✔ Auto Scaling Group Created

### ✔ Running Instance

### ✔ Auto-Healing in Action

---

## 🧪 Auto-Healing Test

To test if Auto Scaling works:
1. Select the EC2 instance
2. Click **Instance state → Terminate**
3. Wait ~2 minutes
4. Auto Scaling launches a new instance automatically

This proves self-healing behavior ✨

---

## 🧹 Cleanup Instructions

To avoid charges:
1. Delete Auto Scaling Group
2. Delete Launch Template
3. Terminate any remaining EC2 instances
4. Check for leftover volumes

You kept your key pair for reuse.

---

## 🎓 Learnings & Conclusion

This project helped demonstrate:
✔ Creation of cloud infrastructure  
✔ Auto-scaling basics  
✔ Fault tolerance and self-healing  
✔ AWS Console navigation

You now have a foundational cloud project for your portfolio!

---

## 🔮 Future Enhancements

Next steps you could implement:
⭐ Add a Load Balancer (ALB)  
⭐ Scale based on CPU/traffic  
⭐ Deploy a web app using user-data  
⭐ Monitor with CloudWatch dashboards

---

## 👤 Author

**Srimahalakshmi R**  
Cloud Enthusiast | AWS Beginner  
LinkedIn: https://www.linkedin.com/in/sri-mahalakshmi-922901336

