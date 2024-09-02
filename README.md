<h1>Decrypting an encrypted message </h1>



<h2>Description</h2>
In this lab, I completed a series of tasks to obtain instructions for decrypting an encrypted file. Encryption of data in use, at rest, and in transit is critical to security functions. I used the Linux skills I have learned to uncover the clues needed to decode a classical cipher, restore a file, and reveal a hidden message.
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>Listing hidden files</b> 
- <b>Decrypting a Caesar cipher</b>
- <b>Decrypting an encrypted file</b> 


<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Read the contents of a file </h2>
In this task, I need to explore the contents of my home directory and read the contents of a file to get further instructions.
 <br/> <br />
(1) I used the command "ls /home/analyst" to list the files in the current working directory. <br/> 
(2) I used the command "cat README.txt" to list the contents of the README.txt file.
<br/> <br/> <p align="center">
<img src="https://imgur.com/AoECcra.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 2: Find a hidden file </h2>
In this task, I need to find a hidden file in my home directory and decrypt the Caesar cipher it contains. This task will enable me to complete the next task.
<br/> <br />
(3) I used the command "cd caesar" to change to the caesar subdiretory of my home directory. <br/>
(4) I used the command "ls -a" to list all files, including hidden files, in my home directory. <br/>
(5) I used the command "cat .leftShift3" to list the contents of the .leftShift3 file. <br/>
(6) I used the command "cat .leftShift3 | tr "d-za-cD-ZA-C" "a-zA-Z" to decrypt the Caesar cipher in the .leftshift3 file. <br/>
(7) I used the command "openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute" to recover my files.
<br /> <br /> <p align="center">
<img src="https://imgur.com/AQdFrWi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Description </h2>
In this task, I need to use the command revealed in .leftshift3 to decrypt a file and recover my data so I can read the message it contains.
 <br/> <br/>
(9) I used the command "openssl aes-256-cbc -pbkdf2 -a -d -in Q1.encrypted -out Q1.recovered -k ettubrute" to <br/>
(10) I used the command "ls" to list the contents of my current working directory again. <br/>
(11) I used the command "cat Q1.recovered" to list the contentsof the Q1.recovered file.  
<br/> <br/> <p align="center">
<img src="https://imgur.com/Epd4dMO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
