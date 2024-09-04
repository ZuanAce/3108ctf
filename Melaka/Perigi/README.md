# Perigi 🔍

## 🧾 Challenge Description
> **Points:** 100   
>  
> Perigi ni selalu kena racun... Sampai saya lupa negara mana yang racun perigi ni untuk kali kedua...
>
> **Challenge Material:** flag.rar
>
> **Category:** OSINT 🔍  

## 🔍 Analysis
- **Initial Thoughts:**  
Visiting the website gives us a 403 Forbidden. However, I discover that the website expects the User-Agent header to be set to curl after watching [**This YouTube Video**](https://www.youtube.com/watch?v=m3-m89YntHs). Making a request with curl gives us a 200 OK.
![image](https://github.com/user-attachments/assets/cda55b96-8caf-4c21-8a70-5ab93c3f7467)


## 🛠️ Solution
- So, I just visit the links, modify the request by setting the User-Agent header to curl and forward the request via BurpSuite, and FLAGGGG at one of the pages!!!
![image](https://github.com/user-attachments/assets/0357cb2b-5c7f-4010-b6af-d55231cfe910)
3108{S3lang0r_temp4t_kelahiran_ku}

## 🧰 Tools Used
- BurpSuite
