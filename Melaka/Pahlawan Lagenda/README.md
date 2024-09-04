# Pahlawan Lagenda 🕵🏻‍♀️

## 🧾 Challenge Description
> **Points:** 100   
>  
> Penyerang telah mencuba merosakkan dan menyembunyikan sesuatu di dalam data hikayat Hang Tuah yang sangat besar pada masa lalu, mungkin mereka masih melakukannya. Muat turun data di sini.
>
> **Category:** Forensic 🕵🏻‍♀️  

## 🔍 Analysis
- **Initial Thoughts:**  
Running the command *strings Tuah.flag.txt* produces a large amount of text. My first instinct is to use *grep "3108"* to check if there was any flag.

![image](https://github.com/user-attachments/assets/8ebc56a6-c165-43d6-8964-6f4df3bf1f0b)


## 🛠️ Solution
- So, using the command *strings Tuah.flag.txt | grep "3108"* reveals the flag!!
  
![image](https://github.com/user-attachments/assets/4664b0ce-a4a7-4cd1-a5aa-c8c7a049da23)

3108{gr3p_15_@w3s0m3_l4ks4m4n4}

## 🧰 Tools Used
- Linux CLI
