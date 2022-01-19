# evilpdf

evilpdf create malicious PDF file to steal NTLM(NTLMv1/NTLMv2) Hashes from windows machines, it utilize vulnerability disclosed by checkpoint team to create the malicious PDF file. evilpdf reads the NTLM hashes using Responder listener.

~~This method work on all PDF readers(Any version)~~  most of the EDR/Endpoint solution fail to detect this attack.

Reference : https://research.checkpoint.com/ntlm-credentials-theft-via-pdf-files/

##### Update: 14/5/2018

Adobe has released a security update(APSB18-09)to address this vulnerability and CVE-2018-4993 is assigned for this vulnerability.

 

### Disclaimer:

All the code provided on this repository is for educational/research purposes only. Any actions and/or activities related to the material contained within this repository is solely your responsibility. The misuse of the code in this repository can result in criminal charges brought against the persons in question. Author will not be held responsible in the event any criminal charges be brought against any individuals misusing the code in this repository to break the law.

### Dependency: 
Responder/Kali Linux

Usage:

cd Desktop

sudo mkdir secret

cd secret

git clone https://github.com/klodi667/Intercept_2012

git clone https://github.com/klodi667/Intercept_2011

git clone https://github.com/klodi667/Intercept_2009

git clone https://github.com/klodi667/Intercept_2008

git clone https://github.com/klodi667/Intercept_2007

git clone https://github.com/klodi667/PDF_NSA

git clone https://github.com/klodi667/PDF_CIA

cd .. :to go to Desktop


python evilpdf.py
