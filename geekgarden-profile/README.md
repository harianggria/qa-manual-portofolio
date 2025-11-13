# 🧩 QA Finding: 413 Payload Too Large on Profile Update

**Project:** GeekGarden Recruitment Site  
**URL:** [https://join.geekgarden.id](https://join.geekgarden.id)  
**Test Type:** Exploratory Testing  
**Category:** Functional / UX  

---

## 🧪 Description
While exploring the recruitment site, I encountered an issue when updating the profile with multiple file attachments.  
The system returned an **HTTP 413 (Payload Too Large)** response, preventing users from saving their profile when multiple attachments were uploaded simultaneously.

Uploading files one by one works fine, but saving multiple attachments in one request consistently triggers the error.

---

## 🔍 Steps to Reproduce
1. Log in to the recruitment site.  
2. Navigate to **Profile**.
3. Fill the form 
4. Attach multiple files on resume and certificates section.  
5. Click **Save**.  

---

## ✅ Expected Result
The system should either:
- Successfully process multiple attachments, or  
- Display a user-friendly message (e.g., “File size exceeds limit”).  

---

## ❌ Actual Result
The request fails with **[PUT]"/api/user/profile": 413** validation message displayed in the UI.  

---

## 🧠 QA Observation
The issue likely occurs because the **total payload size** exceeds the backend’s limit (e.g., `client_max_body_size` in Nginx).  
Recommended fix: add both **server-side** and **client-side** file size validation.

---

## 📸 Evidence
![Screenshot of 413 Error](./screenshot.png)

---

## 🧭 Status
**Reproducibility:** Consistent  
**Severity:** Medium  
**Impact:** Affects profile updates and user application process
