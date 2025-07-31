# 📘 AWS Fundamentals Log – IAM Setup & Free Tier Issues  
🗓️ Date: July 30, 2025

---

## 🧠 What I Did

- Created **two IAM users** from my AWS Root account:
  - `iamadmin`: for everyday non-critical operations and learning
  - `iamadmin_PRODUCTION`: reserved for critical or future project-related tasks
- Configured **Multi-Factor Authentication (MFA)** on both IAM accounts to improve account security
- Assigned **custom permission policies** to each IAM account based on role-specific needs

---

## 🛠️ What Went Wrong (Real Talk)

- I did **not** receive AWS Free Tier access, which was a huge roadblock during initial setup.
- Discovered that using an existing email or previously linked Amazon account can **disqualify you from the Free Tier.**
- This led to wasted time and frustration until I understood that AWS treats account eligibility with strict requirements tied to new root user creation.

---

## 💡 What I Learned

- **NEVER use the root account for daily activity.** It should be locked down with MFA and used only for account management tasks.
- **IAM accounts should be role-based**, not catch-alls. Segmentation of responsibilities helps future-proof infrastructure and improve security posture.
- **MFA should be enabled immediately** for all users, even for personal learning environments.
- AWS Free Tier eligibility is **not guaranteed** if the account email has prior history or services attached. Clean, brand-new emails are essential.

---

## 🔮 Next Steps

- Create IAM **Groups and Roles** to manage policies more efficiently
- Start **hands-on S3 practice**, including bucket creation and object permissions
- Log common **permission errors and fixes** for future reference
- Consider setting up a second AWS account solely for Free Tier testing with a clean root email

---

## 🚀 Reflection

This was frustrating but eye-opening. I was expecting AWS setup to be more "plug and play," but now I realize it's more like "secure and structure first, then play." This whole experience reminded me that in cloud engineering, **structure, roles, and security come before speed.**

---

🔗 _This entry is part of my ongoing AWS learning journey. More lessons, configs, and troubleshooting logs to follow._

<img width="1908" height="920" alt="Screenshot 2025-07-30 180044" src="https://github.com/user-attachments/assets/7eaae27d-9471-41c8-a8f1-aae317d873a8" />

<img width="951" height="908" alt="Screenshot 2025-07-30 175948" src="https://github.com/user-attachments/assets/ac6704e4-6341-4ae0-8a1c-bb5eed5d6516" />
