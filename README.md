### **Cross-Site Scripting (XSS) CTF Challenge**  

#### **Description:**  
This is a simple **Cross-Site Scripting (XSS) challenge** designed for CTF competitions and cybersecurity practice. The challenge involves a web page where users can input their name, which is then reflected back on the page **without proper sanitization**, making it vulnerable to XSS attacks.  

#### **Objective:**  
Your goal is to exploit the vulnerability by injecting JavaScript code into the input field to execute an alert box or steal cookies.  

#### **How It Works:**  
1. The webpage contains an input form where users enter their name.  
2. The entered name is displayed directly on the page using `innerHTML` **without escaping special characters**.  
3. This creates an XSS vulnerability where attackers can inject malicious scripts.  

#### **Challenge Task:**  
Find a way to inject JavaScript code (e.g., an alert box) through the input field and execute it. Example payloads include:  
```html
<script>alert('XSS!')</script>
```
or  
```html
<img src=x onerror=alert('XSS')>
```

#### **Difficulty Level:**  
🟢 Beginner  


