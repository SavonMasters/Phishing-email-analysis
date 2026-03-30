# Phishing-email-analysis


Title: Phishing email analysis

Analyst: Savon Masters  

Date: March 19th, 2026


                                                        Summary 

It is a necessary skill to have the ability to analyze a phishing email likely to be encountered on a personal devices system. Each email you could highlight inaccuracies on how an attacker shapes a person mind to connect and pass information through a self owned link.  A more inspection into this email I found out how a phishing attempt was taken. 


                                                      Investigation 


![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/c5a49591476d1f6f02d87c55114c6c28e36de1e6/Screenshot%20from%202026-03-19%2017-05-37.png)
I take the first step by looking to see any visible instances to tell if the email is a legitimate one or a phishing attempt. It is phishing warnings in the email in the way of impersonation: claiming to be “Voyager team”, urgency: “We strongly recommend initiating your in-kind recovery by clicking the button below as soon as possible”, and offering money for clicking on an unusual link. 


![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/1747538188dcc18fc190e088b63d68118b9837b9/Phishing%20email%201.png)
![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/050c6dee232e691fdf029c87fc7a1a96ea710a5a/Phishing%20email%202.png)
I went into the backend of the email to see anything to tie the phishing attack with a person. Then when I looked at the header area of the email I can see the email is trying to say they are from the “Voyager Team notice[@]office.vn”, trying to reach “phishing[@]pot”, on the date “Thursday, 14th September 2023 23:08:42”. Contradicting this is the return path email addresses “ 0102018a95f42f16-b164a8a8-4d38-474c-86ae-a78a822aa447-000000[@]eu-west-1.amazonses[.]com” a search sent back that “Amazonses[.]com” is potential phishing. 


![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/945039f755d6ef4d6bf340796d077946c9045f7a/Phishing%20email%203.png)
I used tools to find details on the email address and their IP address, I didn't find any issues with them although the email is telling you that the email is from the “Voyager Team” and the “Voyager Team” were not connected to the email address sent out. 


![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/08fe64fc6293ca5acf2eee01546eb30c8ceb7ccc/Phishing%20email%204.png)
The SPF (Sender policy framework) came back as a pass for the explanation of “Amazonses”  (Amazon simple email service) is a confirmed email provider and would not be bothered by the SPF, DKIM, and DMARC check. 


![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/13b58e50280e9d4f1f5f57f88d85a010c2280b1f/Phishing%20email%205.png)
![image alt](https://github.com/SavonMasters/Phishing-email-analysis/blob/693011e165f371ba87dfffd30eae2701b14cb628/Phishing%20email%206.png)
I additionally identified a clickable link “hxxps[://]newjerseysigninstallation.c=
om/withdraw?” in the “Intitante withdrawal” button. The link does not have any problems; it has no resemblance to the “Voyager Team”.


                                                        Conclusion 

When a message was delivered on “14th, September 2023 23:08:42” to “Phishing[@]pot” from “Voyager Team notice[@]office[.]vn” A switched return path email address “0102018a95f42f16-b164a8a8-4d38-474c-86ae-a78a822aa447-000000[@]eu-west-1.amazonses[.]com, 54.240.6.245” sent from “Amazonses Amazon Simple Email Service” was honestly used. The body was relaying to transfer funds into your wallet. The email coaxed the receiver to click on "Initiate withdrawal” button, in the inner button kept the link “hxxps[://]newjerseysigninstallation.c=
om/withdraw?”. An actual phishing email attack was communicated to our system. 


                                                        IOCs

* A copy email address “notice[@]office[.]vn”.

* The attackers email and IP address “0102018a95f42f16-b164a8a8-4d38-474c-86ae-a78a822aa447-000000[@]eu-west-1.amazonses[.]com, 54.240.6.245”. 

* The “Voyager Team” not being associated with the “Amazonses” account.

* A chance of an impersonation attack editing their presence to look as “Voyager team”.

* A chance of urgency to transfer funds to your wallet within a decreasing amount of time. 

* A chance of offering money to click on a normal button.

* A link put inside of the button “hxxps[://]newjerseysigninstallation.c=
om/withdraw?”.

* MITRE techniques “Phishing T1660”, “Email spoofing T1672”, "Impersonation T1656”, and “Steganography T1027.003”.


                                                        Recommendations

* Block the attackers email and IP address “ 0102018a95f42f16-b164a8a8-4d38-474c-86ae-a78a822aa447-000000[@]eu-west-1.amazonses[.]com, 54.240.6.245”.

* Let a Web application firewall block malicious links in emails.

* Use the email service provider built in phishing email blocks to sort emails with mystery origins.  

* An out of place email is seen with problem links, look at the link before you click.

* Block the link and stop trying to view its site “hxxps[://]newjerseysigninstallation.c=
om/withdraw?”.


                                                        Things I learned 

* The backend makeup of an email of how it arranges itself to be sent to a network. 

* How an email mistakes an non educated user to put out their information utilizing appearance, expressive words, and access to a group of rewards.

* The first factors inside of a imagine to see if its set up to phish. 

* Important mitigations to eliminate the opportunity to get phishing emails. 
