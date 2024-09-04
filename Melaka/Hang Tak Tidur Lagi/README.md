# Hang Tak Tidur Lagi? 🕸️

## 🧾 Challenge Description
> **Points:** 100   
>  
> Hang Tuah digambarkan sebagai seorang pahlawan yang berjaga malam, hanya tidur sedikit untuk mempersiapkan dirinya untuk tugas yang besar. Tetapi, semasa ke Istana untuk bertemu dengan Pembesar Berempat yang lain, Hang Tuah telah tidur kerana kepenatan berfikir.
>
> **Challenge URL:** https://fc9044a5b6.bahterasiber.my/
>
> **Category:** Web 🕸️
 

## 🔍 Analysis
- **Initial Thoughts:**  
Upon inspecting the page, I notice a commented username and password both set to *tuah*. My first thought was to use Burp Suite to intercept the web request, where I discovered a decoded URL parameter: **role=JRAUWU2BJVAU4QI=**. After decoding it using a [Base 32 Decoder](https://emn178.github.io/online-tools/base32_decode.html), I found that the plaintext for **JRAUWU2BJVAU4QI=** is **LAKSAMANA**, one of the *Pembesar Berempat Melaka*.
![image](https://github.com/user-attachments/assets/56ea84b0-8de0-44bc-a75a-a9092d4126f5)
![image](https://github.com/user-attachments/assets/2791d189-3c35-4ecd-83f9-a72b50f8b38a)


## 🛠️ Solution
- So, all I have to do now is to encode *Bendahara, Penghulu Bendahari, and Temenggung* using [Base 32 Encoder](https://cryptii.com/pipes/base32)
  
| POSITION   | ENCODED   | 
|-------------|-------------|
| BENDAHARA | IJCU4RCBJBAVEQI= | 
|PENGHULU BENDAHARI | KBCU4R2IKVGFKICCIVHEIQKIIFJES=== | 
| TEMENGGUNG | KRCU2RKOI5DVKTSH | 

- Changing the roles reveals different parts of the flag, and when combined, they form the complete flag!
![image](https://github.com/user-attachments/assets/df11c6bf-db5a-40de-aa10-f87911c8af2c)
![image](https://github.com/user-attachments/assets/7d27f832-9f34-4ed4-8268-2a8d7f604c42)
![image](https://github.com/user-attachments/assets/9d77cf25-65e6-4049-b431-22a8b18cbe94)
3108{1d0R_s4nGa7l4h_Bah4y4!}

## 🧰 Tools Used
- BurpSuite
- Google Search


