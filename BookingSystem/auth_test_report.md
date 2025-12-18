
### 🧑‍🦲 **Guest**

---

**✅ Can do**



* Can view public resource list -- "/"
* Can acces login and register form -- "/login"
* Can view registered reservation witohut identity -- "/" (spec 8)
* Can view registered accounts, token, role etc with "/api/users"
* Can view "/api/resources"
* So literally guest can see everything

---

**❌ Cannot do**



* Cannot access "/reservation" ( The process failed. Unauthorized )
* Cannot POST "/api/reservations"
* Cannot access admin pages (i think there is none
* Cannot acces reserver profile page


---

### 🧑‍💼 **Reserver**

---

**✅ Can do**



* Can book new resource -- "/reservation" 
* Can list new resoure /resources
* Can change  own reservation reserver from registered accounts
* Has access to other accounts reservation using browers with changing reservation?id= (for example reservation?id=2) can edit those and after that can delete reservation (admin form)
* Can view registered accounts, token, role etc with "/api/users"
* Can view "/api/resources"
* Can create access to edit and delete resources -- "/resources?id=*"

---

**❌ Cannot do**

List actions a *Reserver* is correctly blocked from.

* Cannot delete users



---

### 🧑‍💼🛡️ **Administrator**

---

**✅ Can do**

List actions an *Administrator* can perform.

* Can add a resource
* Can manage all reservations
* Can view all users -- /api/users

---

**❌ Cannot do**

List prohibited behaviors, if any, or incorrect implementation issues.

* cannot delete users

---



