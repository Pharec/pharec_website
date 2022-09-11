---
Title: Phishing Overview

---

Social Engineering and Phishing attacks are two types of deception and information disclosure attacks. In this post we define phishing with examples, anatomy of attack and tips to avoid and mitigate these attacks. Historically there have been many examples (incidents) that involved social engineering as a whole attack or part of a series of malicious operations to achieve adversarial goals. Social engineering is a major threat that “was responsible for over 69% of breaches” on public administration organizations around the world, almost all of the breaches involved phishing attacks, as reported in Verizon’s 2021 DBIR (Data Breach Investigation Report). Furthermore, according to APWG (Anti-Phishing Working Group), the number of phishing attacks has doubled after 2020 and remained at the same high level, more specifically, in June 2021 they observed 222,127 attacks. In this article we answer and discuss the following questions: what is phishing? How are attackers able to mount phishing campaigns and targeted attacks? What can we do to avoid and mitigate phishing?

# What is phishing?
Phishing is the use of modern technologies (e.g. email, web) to deceive humans into disclosing personal (sensitive) information or performing harmful actions to themselves or their organizations. 
# Examples of phishing attacks
“Bad Tidings” is a famous example of a phishing campaign that targeted Saudi Arabia. According to Anomali labs, the campaign targeted people in Saudi Arabia by publishing fraudulent sites of many services including governmental (e.g., Absher portal) and private (e.g. local bank sites). They observed 95 unique phishing hostnames that use various textual deception techniques. An example of what an Absher fraudulent site looks like is below. It can also be accessed through the link: [https://abshar-project.web.app/home.html](https://abshar-project.web.app/home.html) (access the link from outside the kingdom if it does not work).

![ex1_1](/assets/posts/phishing_overview/ex1_1.png)
![ex1_2](/assets/posts/phishing_overview/ex1_2.png)

Postal service and delivery companies were also a target of phishers recently in the region. One such example is an Aramex phishing website that was discovered trying to deceive people into paying a fraudulent bill as shown in the figure below. This sort of scam URL could have been received in shortened form, to mask the domain name difference, through a mostly trusted communication channel (e.g. SMS).

![ex2_1](/assets/posts/phishing_overview/ex2_1.png)
![ex2_2](/assets/posts/phishing_overview/ex2_2.png)

There are also other types of phishing attacks frequently observed in the wild like BEC (Business Email Compromise) and spear phishing scams. BEC are email attacks that usually involve impersonation of people with important business roles or authority in an organization with the goal of deceiving others in the organization into disclosing information or performing harmful actions. For example, an attacker might target the financial officer of a certain company that, has known business and vendors, with a spear phishing attack asking to pay outstanding bills to a new bank account after impersonating the vendor. According to APWG this type of scam accounted for around $106,000 in losses last year.

# How do adversaries mount phishing attacks?
An attacker mounting a phishing attack typically starts by selecting a target website or scam scheme. The target website is usually a popular website that provides a service aimed at the average individual or organizations. The phisher then tries to construct a page or a story with the goal of making the attack believable by victims. After that, the attacker chooses the distribution channel and starts mounting (distributing) the phishing attack. Finally, they wait for victims to fall prey to the attack and collect disclosed information or the targeted resource as illustrated in the following figure.
 
![Phishing process](/assets/posts/phishing_overview/phish_process.png)

# How can you protect yourself from phishing attacks?
Typically, in phishing the attacker will ask the victim to perform a certain action or enter their data, so, we ought to be careful when asked to enter any personal data or login credentials. The following tips are helpful in these scenarios where phishing attacks are common:

*	Check URLs carefully (does the URL perfectly match the expected site)

A phisher will typically try to deceive users by presenting them with a URL similar to what they expect (e.g. [http://abshr.com](http://abshr.com)). Users need to check whether the domain name and top level domain match those of the expected website/service. For instance, the example domain name “abshr.com” is clearly not correct for the Absher site for two reasons: the top level domain for a Saudi government service should be ‘.sa’ and the “Absher” service is spelled without the “e”. There are more advanced attacks to mask URLs like the homograph attacks, but we leave details of these attacks to future articles.

*	Double check suspicious emails claiming to be from people of authority

For example, if you receive an email, from an important individual, urgently asking you to take action. Rather than performing the action directly, one should contact that individual (sender) through a different channel and confirm the action with them. 

*	Use phishing solutions/ anti-phishing products

One such tool is the [Zelda Anti-Phishing](https://github.com/Segasec/zelda-anti-phishing) browser extension; it is an open-source tool that relies on open-source feed (list) of phishing URLs to block phishing sites. Another service that allows you to query the status of a website is [Google safe browsing](https://transparencyreport.google.com/safe-browsing/search).There are other techniques that help detect and mitigate phishing, like black listing low reputation sites and URL pattern recognition. 

# References							 		
- Verizon. “Verizon 2021 Data Breach Investigations Report”
- Laudon, K. C., & Traver, C. G. (2020). E-commerce: Business, technology, society.
- Anomali lab. [“Bad Tidings” Phishing Campaign Impersonates Saudi Government Agencies and a Saudi Financial Institution](https://www.anomali.com/blog/bad-tidings-phishing-campaign-impersonates-saudi-government-agencies-and-a-saudi-financial-institution) (accessed Nov 2021).
- APWG (Anti-Phishing Working Group). [Phishing Activity Trends Reportls](https://apwg.org/trendsreports/) (accessed Nov 2021).
