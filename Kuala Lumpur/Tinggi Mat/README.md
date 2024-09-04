# Tinggi Mat 🕵🏻‍♀️

## 🧾 Challenge Description
> **Points:** 100   
>  
> Kalau kat KL je mesti ingat KLCC. Alang-alang kita cerita pasal bangunan tinggi ni. Kenal tak Warisan Merdeka Tower?
>
> **Challenge Material:** WMT.rar
> 
> **Category:** Forensic 🕵🏻‍♀️  

## 🔍 Analysis
- **Initial Thoughts:**  
So, the first thing came into my mind is to unrar the file. Two files were obtained, flag2.rar and WarisanMerdekaTower.png.  
![image](https://github.com/user-attachments/assets/09f8c32d-f15f-44c1-82be-f753a384f27d)


## 🛠️ Solution
- Running the command *zsteg -a WarisanMerdekaTower.png* reveals the first part of the flag and provides the password for flag2.rar, which is **MERDEKA118**.

![image](https://github.com/user-attachments/assets/543df232-aa65-44b5-b3b3-85fc63a9aa8e)

- Use the password to unrar the file. Using the command *cat flag2.txt* does not give much information about the file, thus I use the command *hexdump -C flag2.txt*: This command shows the file's contents in hexadecimal format, which can be useful for seeing hidden data or non-printable characters.
  
![image](https://github.com/user-attachments/assets/792d6115-4fad-476b-a052-c3bac3bf413f)

- The hexdump seems suspicious, so I copypaste it at ChatGPT for more information. Turns out to be related to **Unicode zero-width spaces**.

![image](https://github.com/user-attachments/assets/a2e0fa07-d246-47ef-b136-b332c5312186)

- Open the flag2.txt file, then Ctrl+A, and copy the whole content of the text file. Paste it at [Unicode Steganography with Zero-Width Characters Decoder](https://330k.github.io/misc_tools/unicode_steganography.html) and decode the text to reveal the last part of the flag. Finally, combine it and FLAGG!!!

![image](https://github.com/user-attachments/assets/e71a2e4a-41a1-4b77-98d1-fc69d5bb9fe2)

3108{th3_t4ll3st_0n3_1n_M4l4ys14!}

## 🧰 Tools Used
- Linux CLI
- ChatGPT
- Unicode Steganography with Zero-Width Characters Decoder
