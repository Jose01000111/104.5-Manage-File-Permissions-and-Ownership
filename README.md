# 📁 104.5: Manage File Permissions and Ownership

## ✅ What I did in this lab
I used commands like chmod, chown, chgrp, and umask to manipulate file permissions and ownership. I also applied special permissions to test how they affect file and directory access behavior.

I’ve included some helpful links to guide you through the lab and for studying afterward:

[OBJECTIVE 104.5](https://www.lpi.org/our-certifications/exam-101-102-objectives/#104.5_Manage_file_permissions_and_ownership)

[OBJ.104.5 NOTES](https://1drv.ms/w/c/354f1c8d534fbced/EdsMbFqWo6pEsHiAnk3O8zoBsagjVHEmUxLQL_d9BrwHLA?e=0dBjQo)

[OBJ.104.5 LAB](https://1drv.ms/w/c/354f1c8d534fbced/ESZfNUcJ31tEmLcpycr2BzcB-UPnEyrIYev3Eeoxk-QUGg?e=iuj16M)

---

1️⃣ Understanding and Modifying Basic File Permissions

🔹 Create a sample file and check its permissions

![W9kTJzZ](https://github.com/user-attachments/assets/843144cd-212e-4d42-b8d8-f24a5c33fc9a)

🔹 Use chmod to set specific permissions

![Pu5QhGR](https://github.com/user-attachments/assets/c75fd13c-7595-48d5-82c8-b426aea9e6ff)

🔹 Use symbolic notation to modify permissions

![bWYbpH1](https://github.com/user-attachments/assets/450286a8-e66a-4e5f-a19c-94b33240ae73)

2️⃣ Working with File Ownership

🔹 Check file ownership

🔹 Change the file owner

![M9V8C7o](https://github.com/user-attachments/assets/c5d634da-10aa-4364-89c4-ff7341c81e23)

🔹 Change the group ownership

![zKqryGv](https://github.com/user-attachments/assets/f4466056-98ae-499c-a12e-276582332b32)

3️⃣ Understanding and Using Special Permissions (suid, sgid, sticky bit)

🔹 Set the suid bit on an executable (for user inheritance)

![9txBcDy](https://github.com/user-attachments/assets/bc8acaf8-0b93-4de4-9f55-ac9fdb22f4aa)

![05BKCMW](https://github.com/user-attachments/assets/427a03fc-16c0-40de-b30b-f9053a864a6b)

🔹 Set the sgid bit on a directory (for group inheritance)

![05BKCMW](https://github.com/user-attachments/assets/f446f78a-f33a-4ddb-83df-d093d28327a7)

🔹 Set the sticky bit on a directory (like /tmp)

![UQTQUgY](https://github.com/user-attachments/assets/1b6779cf-2e01-49c3-a804-b651fc3e9f96)

4️⃣ Using and Understanding umask

🔹 Check the current umask value

![NLUDQSl](https://github.com/user-attachments/assets/a0320eb6-626b-413a-9cb0-c9ff180cf76f)

🔹 Create a file and check its default permissions

![dlp5KBy](https://github.com/user-attachments/assets/eaa9df2b-71ad-41ce-8208-909db86489ab)

🔹 Set a new umask and create another file

![dlp5KBy](https://github.com/user-attachments/assets/b02813bb-1678-4cdf-b4f7-aa8ee97abd26)

5️⃣ Using Groups to Manage Access

🔹 Add users to a group

![bGUXUMb](https://github.com/user-attachments/assets/76e7c24e-0b10-438c-ba22-fb2c35cda0a8)

![IATxPXD](https://github.com/user-attachments/assets/7fd381b3-864b-445e-8bf2-37ad37c8b9a7)

🔹 Change the group ownership of a file

![yREeM99](https://github.com/user-attachments/assets/d84e1785-fc74-42bc-80d2-db5c6adb955b)

🔹 Set group permissions on the file

![B0atbXO](https://github.com/user-attachments/assets/4e8d4cbe-77c5-49fc-8271-1aac8c4e2693)

---

## 📘 What I learned
🔸 I learned how to manage file and directory permissions using both numeric and symbolic modes.

🔸 I now understand how special permission bits affect file behavior and security.

🔸 I practiced using umask to control default permissions for newly created files.

🔸 I also saw how group ownership and group permissions can streamline team-based access to shared resources.
