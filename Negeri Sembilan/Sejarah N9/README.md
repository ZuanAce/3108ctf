# Sejarah N9 🧩 + 🧮

## 🧾 Challenge Description
> **Points:** 100   
>  
> Negeri Sembilan secara rasminya ditubuhkan pada 1889, suku di negeri sembilan ada 12 dan daerah di Negeri Sembilan ada 7. Setiap peristiwa pasti tersingkap padanya angka sejarah. Momen terbesar sebelum peristiwa2 di atas ada pada kod id bawah. Boleh baca?
>
> 2097119120211115191514712116114
> 
> **Category:** Trivia + Misc + Cryptography 🧩 + 🧮


## 🔍 Analysis
- **Initial Thoughts:**  
Use [Cipher Idendifier](https://www.dcode.fr/cipher-identifier) to determine the type of algorithm used for encrypting the plaintext.

![image](https://github.com/user-attachments/assets/5c66af05-5e1f-44e0-b8ba-f618ddf015b7)


## 🛠️ Solution
- By simply using [Letter Number Code (A1Z26) Decoder](https://www.dcode.fr/letter-number-cipher), to brute force the ciphertext, the readable strings *KOSONG* and *LAPAN* appear. Using CTRL+F to search for these strings leads to the final result: **TIGASATUKOSONGLAPAN**.
  
![image](https://github.com/user-attachments/assets/9ed381db-5931-4565-ab9e-af563027fff9)

3108{TIGASATUKOSONGLAPAN}
  
## 🧰 Tools Used
- Cipher Identifier
- Letter Number Code (A1Z26) Decoder
