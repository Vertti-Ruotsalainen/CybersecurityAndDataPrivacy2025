You will investigate what each role (Guest, Reserver, Administrator):

    CAN do
    CANNOT do

…based on the official application specifications and the actual behavior of the current Phase 3 implementation.

You will test all accessible pages, functions, and API endpoints and then produce:

> [!NOTE]
> As a reminder

**You are a novice penetration tester at a company. Your company should implement the following application (specs):**

1. The system is accessed via a web browser.  
2. Users can register and, after registration, log in to the system.  
3. A registered and logged-in user acts as either a resource reserver or an administrator.  
4. The administrator can add, remove, and modify resources and reservations.  
5. The administrator can delete the reserver.  
6. A reserver can book a resource if they are over 15 years old.  
7. Resources can be booked on an hourly basis.  
8. The booking system displays booked resources without requiring login, but does not show the reserver's identity
9. The client, your company, requires that the system complies with GDPR regulations.  
10. The system provider has stated that the software is developed following the Privacy by Design (PbD) principle. 

---

**Imagine that your client wants confirmation that:**

* Guests cannot access protected content
* Reservers cannot perform admin actions
* Administrators have full control but no unnecessary extra exposure
* No endpoint leaks, hidden pages, or bypasses exist
* Authorization decisions are correctly enforced at the backend



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


---

> [!NOTE]
> ✔️ Hidden pages found with Gobuster or ZAP must also be added under the correct role.
