# BLUE-writeup

<img width="949" alt="BLUE_description" src="https://github.com/J3Ss0u/BLUE-writeup/assets/90192954/63054837-ead5-41b8-bb20-8baef4f4a84e">

BLUE challenge one of DFIR challenges in Larbi CTF (Local CTF in 1337 school)

## Introduction
In this challenge, you are presented with a access.log file, a crucial component of web server security and performance monitoring. Your task is to analyze the log entries, identify anomalies, and extract a hidden flag.

## What is an access.log file?

access.log file is a record of every request made to a web server. It contains detailed information about each incoming request, including the client's IP address, request method, requested resource, response code, and other relevant data. The primary purpose of access logs is to track and monitor web server activity, helping administrators identify issues, optimize performance, and detect security threats.

## Importance of Log Files

**Security monitoring**: Logs help identify potential security threats, such as unauthorized access attempts, SQL injection, or cross-site scripting (XSS) attacks.
**Performance optimization**: Analyzing logs can reveal bottlenecks, slow responses, and other performance issues, enabling administrators to optimize server configurations and improve user experience.

## Challenge Solution
To solve this challenge, you need to carefully examine the access.log file and identify unusual patterns or anomalies. Upon closer inspection, you may notice that some log entries contain a browser version with a typo: "Mozlla" instead of "Mozilla". This is a red flag, indicating that these log entries might be suspicious.
<img width="1665" alt="Screen Shot 2024-07-07 at 10 17 53 AM" src="https://github.com/J3Ss0u/BLUE-writeup/assets/90192954/7396eed9-9a81-4e4b-8c81-f52aa5d83108">

Further analysis reveals that each "Mozlla" log entry contains a character in the path directory, such as "/category/T". Your task is to collect these characters and arrange them in the correct order. However, the challenge is that the characters are scattered across different log entries, and the timestamps are not in chronological order.

To overcome this, you need to sort the "Mozlla" log entries by their timestamps and extract the characters in the correct order. Once you have the complete sequence of characters, you'll find the flag: `AKASEC{Y0U_N33D_T0_B3_GOOD_4T_4N4LYS1S}`

## Additional Challenges

There are some challenges related to log analysis that you can try:
* [Web Investigation](https://cyberdefenders.org/blueteam-ctf-challenges/web-investigation/)
* [Hacked](https://cyberdefenders.org/blueteam-ctf-challenges/hacked/)
* [Hammered](https://cyberdefenders.org/blueteam-ctf-challenges/hammered/)

### Akasec family :heart:
