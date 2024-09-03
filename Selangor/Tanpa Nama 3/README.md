# Tanpa Nama 3 🧮

## 🧾 Challenge Description
> **Points:** 100    
>   
> **Category:** Cryptography 🧮

## 🔍 Analysis
- **Initial Thoughts:**  
 So the python script provided takes a binary string, splits it into individual 8-bit binary numbers, and then XORs each of these with a given XOR string (also in binary). 
```
def xor_with_binary(binary_str, xor_str):
    # Split the binary string into a list of binary numbers
    binaries = binary_str.split()
    
    # Convert the XOR string into an integer
    xor_num = int(xor_str, 2)
    
    # List to hold the XOR results
    xor_results = []
    
    # Loop through each binary number in the list
    for b in binaries:
        # Convert each binary number into an integer
        num = int(b, 2)
        
        # Perform the XOR operation between the number and xor_num
        result_num = num ^ xor_num
        
        # Convert the result back to an 8-bit binary string
        xor_results.append(format(result_num, '08b'))
    
    # Join the results into a single string with spaces between them
    return ' '.join(xor_results)

# Example binary string and XOR string
binary_str = "01010110 01010100 01010101 01011101 00011110 00110110 01010100 00101000 00110101 00101001 01010110 00111010 00100110 00110111 00110101 00111100 00110001 01010101 00111010 00100110 00101101 00100100 00101001 00101001 00100000 00101011 00100010 00100000 00011000"
xor_str = "01100101"

# Run the XOR function and print the result
result = xor_with_binary(binary_str, xor_str)
print(result)
```


## 🛠️ Solution
- To get the result in ASCII, I modify the code so that after performing the XOR operation, the binary result is converted to its corresponding ASCII character. 
 ![image](https://github.com/user-attachments/assets/2ed40732-597c-47e8-b331-f3d2f26eb356)
3108{S1MPL3_CRPYT0_CHALLENGE}

## 🧰 Tools Used
- ChatGPT for explanation
- Programiz Python Online Compiler


