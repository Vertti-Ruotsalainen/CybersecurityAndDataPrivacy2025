| Account  | Token | Method |  Outcome(s) | 
| :---         |     :---:      |     :---:      |     :---:      |
| whatsupdoc@looneytunes.tv | a0e8402fe185455606a2ae870dcbc4cd | dictionary attack  | <img width="973" height="88" alt="kuva" src="https://github.com/user-attachments/assets/6a3ddae0-3894-4c7f-99b0-ef5a2f2ed023" />, <img width="938" height="498" alt="kuva" src="https://github.com/user-attachments/assets/878e2b58-7ddb-4f43-a14c-ecbc2f708123" /> |
| doh@springfieldpower.net | d730fc82effd704296b5bbcff45f323e | dictionary attack  | <img width="965" height="51" alt="kuva" src="https://github.com/user-attachments/assets/d7d42ea4-e346-4f34-852b-ceff63409c26" />, <img width="559" height="40" alt="kuva" src="https://github.com/user-attachments/assets/62cde03d-70e1-49ff-8d3c-7f35b897a5af" />  |
| darkknight@gothamwatch.org | 735f7f5e652d7697723893e1a5c04d90 | 12 lowercase letters -> first 6 are iamven  | <img width="572" height="30" alt="kuva" src="https://github.com/user-attachments/assets/97cf4d44-7023-4267-9aeb-b715a2b90459" />, <img width="954" height="51" alt="kuva" src="https://github.com/user-attachments/assets/77bf8f3c-3081-4f73-a44e-fbef63dff8ce" />|
| chimichanga@fourthwall.com | 7cb56c2b86150b797cff32eaef97f338 | 1 digit, 14 lowercase letters -> first 8 are breaking, last 2 are ll  | <img width="975" height="56" alt="kuva" src="https://github.com/user-attachments/assets/105d506f-7f7e-47ea-bd8b-98881634116d" />, <img width="597" height="40" alt="kuva" src="https://github.com/user-attachments/assets/815961c7-9771-4c2c-9328-ff01b98b3b2b" />|
| iamyourfather@deathstar.gov | 706ab9fc256efabf4cb4cf9d31ddc8eb | dictionary attack  | <img width="965" height="56" alt="kuva" src="https://github.com/user-attachments/assets/84579240-b742-41d8-b6d7-6236e6897be2" />, <img width="544" height="35" alt="kuva" src="https://github.com/user-attachments/assets/a9217eb3-cdfa-4cb5-98f2-bfb576950083" />|
| elementary@221bbaker.uk | 12c9cef0bfb6b91c42b363b4cf02d8bb | 3 digit, 10 letters -> first part of the password is deduction  | <img width="943" height="55" alt="kuva" src="https://github.com/user-attachments/assets/c3fd0e23-11ea-438b-b4fc-102d5dcbd329" />, <img width="580" height="36" alt="kuva" src="https://github.com/user-attachments/assets/c96a3166-a583-4412-b185-c80709df4287" />|
| genius@starkindustries.com | d50ba4dd3fe42e17e9faa9ec29f89708 | dictionary attack  | <img width="967" height="48" alt="kuva" src="https://github.com/user-attachments/assets/72716362-ca3d-4ba4-8715-4982a5553b40" />, <img width="534" height="32" alt="kuva" src="https://github.com/user-attachments/assets/c83ef8fa-27f4-4501-afd0-e2832638bd25" />|
| whysoserious@gothamchaos.net | f158d479ee181aac68b000a60e7a3d7a | 9 mixed characters -> first part is chaos, last character is !  | <img width="889" height="50" alt="kuva" src="https://github.com/user-attachments/assets/11c4d063-6670-447f-a48c-2a9c7b66b18b" />, <img width="512" height="40" alt="kuva" src="https://github.com/user-attachments/assets/8cc9c933-7f51-4832-9ec5-bd8e40eb9411" />|
| quackattack@duckburg.org | ea261222d4867b3ebdfadbe2b35e19d5 | 15 lowercase letters -> last part is isjealous  | <img width="984" height="48" alt="kuva" src="https://github.com/user-attachments/assets/b1e556f5-66a0-4283-9461-accb7d8d1144" />, <img width="598" height="40" alt="kuva" src="https://github.com/user-attachments/assets/5cbe229a-655d-4956-9a4a-4eb7ac346253" />|
| ruhroh@mysterymachine.com | ad17fbd845000b11678ccbf94e135b56 | 1 digit + 12 lowercase -> last part is scooby, digit is the middle character  | <img width="978" height="58" alt="kuva" src="https://github.com/user-attachments/assets/89864510-f740-419b-8173-c4aff7b71d32" />, <img width="574" height="44" alt="kuva" src="https://github.com/user-attachments/assets/9ee422ff-f1bb-42ff-bffe-19d59d3a522d" />|


In  this exercise i used kali linux and there we downloaded hashcat, hydra, rockyou.txt.

Used hashcat commands:
1. hashcat -O -m 0 -a 0 "a0e8402fe185455606a2ae870dcbc4cd" rockyou.txt --force
2. hashcat -O -m 0 -a 0 "d730fc82effd704296b5bbcff45f323e" rockyou.txt --force
3. hashcat -O -m 0 -a 3 "735f7f5e652d7697723893e1a5c04d90" iamven?l?l?l?l?l?l
4. hashcat -O -m 0 -a 3 "7cb56c2b86150b797cff32eaef97f338" breaking?d?l?l?l?lll
5. hashcat -O -m 0 -a 0 "706ab9fc256efabf4cb4cf9d31ddc8eb" rockyou.txt --force
6. hashcat -O -m 0 -a 3 "12c9cef0bfb6b91c42b363b4cf02d8bb" deduction?d?d?d?u
7. hashcat -O -m 0 -a 0 "d50ba4dd3fe42e17e9faa9ec29f89708" rockyou.txt --force
8. hashcat -O -m 0 -a 3 "f158d479ee181aac68b000a60e7a3d7a" chaos?d?d?d?s
9. hashcat -O -m 0 -a 3 "ea261222d4867b3ebdfadbe2b35e19d5" ?l?l?l?l?l?lisjealous
10. hashcat -O -m 0 -a 3 "ad17fbd845000b11678ccbf94e135b56" ?l?l?l?l?l?l?dscooby

Tested cracked passwords in exercise site and those worked. Think i passed this task.



