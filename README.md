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

bash
Copy
Edit
touch myfile.txt  
ls -l myfile.txt  

🔹 Use chmod to set specific permissions

bash
Copy
Edit
chmod 764 myfile.txt  
ls -l myfile.txt  

🔹 Use symbolic notation to modify permissions

bash
Copy
Edit
chmod u+x myfile.txt  
chmod g-w myfile.txt  
ls -l myfile.txt  

2️⃣ Working with File Ownership

🔹 Check file ownership

bash
Copy
Edit
ls -l myfile.txt  

🔹 Change the file owner

bash
Copy
Edit
sudo chown anotheruser myfile.txt  

🔹 Change the group ownership

bash
Copy
Edit
sudo chgrp anothergroup myfile.txt  

3️⃣ Understanding and Using Special Permissions (suid, sgid, sticky bit)

🔹 Set the suid bit on an executable (for user inheritance)

bash
Copy
Edit
sudo chmod u+s /usr/bin/example_executable  
ls -l /usr/bin/example_executable  

🔹 Set the sgid bit on a directory (for group inheritance)

bash
Copy
Edit
sudo mkdir shared_dir  
sudo chmod g+s shared_dir  
ls -ld shared_dir  

🔹 Set the sticky bit on a directory (like /tmp)

bash
Copy
Edit
sudo mkdir sticky_dir  
sudo chmod +t sticky_dir  
ls -ld sticky_dir  

4️⃣ Using and Understanding umask

🔹 Check the current umask value

bash
Copy
Edit
umask  

🔹 Create a file and check its default permissions

bash
Copy
Edit
touch umask_test.txt  
ls -l umask_test.txt  

🔹 Set a new umask and create another file

bash
Copy
Edit
umask 027  
touch restricted_file.txt  
ls -l restricted_file.txt  

5️⃣ Using Groups to Manage Access

🔹 Add users to a group

bash
Copy
Edit
sudo usermod -aG projectgroup username  

🔹 Change the group ownership of a file

bash
Copy
Edit
sudo chgrp projectgroup shared_doc.txt  

🔹 Set group permissions on the file

bash
Copy
Edit
chmod 660 shared_doc.txt  
ls -l shared_doc.txt  

---

## 📘 What I learned
🔸 I learned how to manage file and directory permissions using both numeric and symbolic modes.

🔸 I now understand how special permission bits affect file behavior and security.

🔸 I practiced using umask to control default permissions for newly created files.

🔸 I also saw how group ownership and group permissions can streamline team-based access to shared resources.
