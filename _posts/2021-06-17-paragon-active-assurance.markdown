---
layout: post
title:  "Juniper Paragon Active Assurance"
date:   2021-06-17 10:00 +0700
categories: blog
author: wesley
---

<div markdown="span" class="alert alert-info" role="alert"><i class="fa fa-info-circle"></i> <b>Note:</b> I didn't know of Juniper Paragon Active Assurance until I've applied for a job at Juniper Networks - "Technical Marketing Engineer little did I know that this was for Paragon Active Assurance, this post is about my experience with the former Netrounds folks and my interview process."</div>
<br>
So, I applied for the role and about a week after applying for it [Mats Nordlund](https://www.linkedin.com/in/matsnordlund/) reached out to me by LinkedIn because my MTA was not accepting inbound e-mails from juniper.net due to a bad senderscore it appeared later. We had setup a Teams meeting for that evening my time and we had a great conversion. The same was repeated two days later with [Jonas Krogell](https://www.linkedin.com/in/krogell/) where after this meeting I received homework, read a assignment. Also it was made clear that the role I've applied for was already filled by somebody else but there was interest in me perhaps furfilling a different role in the form of Solution Architect. So we decided to explore this possibility from there.
<br>
I liked the assignments given, get to known their product Paragon Active Assurance and workout a presentation on the topic. Amongst this I was asked to create a ansible workbook to show that I would automate my work.

I proceeded with creating the [ansible-playbook](https://github.com/ExpertLevel/automation-examples/blob/main/ansible/Juniper/Paragon/Active-Assurance/install-paacc-ansible.yml) first.

This is basically pretty much everything which is in the [installation documentation](https://www.juniper.net/documentation/us/en/software/active-assurance3.0.0/paa-install/index.html) for the Control Center. After this you need to proceed creating user's & account's and request a license.

Besides this I had a [inventory](https://github.com/ExpertLevel/automation-examples/blob/main/ansible/Juniper/Paragon/Active-Assurance/hosts) file:
```
[paacc]
paacc.demo.expertlevel.blog

[paacc:vars]
CC_VERSION=3.0.2
TA_APPLICATION_VERSION=3.0.0.15
TA_APPLIANCE_VERSION=3.0.1.35
DB_USER=netrounds
DB_PWD=netrounds
DB_NAME=netrounds
```
Again just a basics simple inventory and workbook, this I used to deploy my Control Center with, this went down without any big hassles. Be sure you read the requirements carefully in regards to the amount of RAM needed for the Control Center in the installation documentation listed above.
<br>
Evaluation time:
During my 48 hours I've played with the tool, I can hands-down state that if in earlier engagements I had this it would've made my life WAY easier.

All the sleepless nights I've had about explaining to Management why something wasn't performing in the most simplified way I could by producing manual reports of completicated networking stuff (IGMP/VoD problems, QoS misconfigured, Jitter, Underperformance of a Service). This can be as simple as pressing a button or doing a API call with Paragon Active Assurance.

<br>
Presentation time:
I've presented my demo environment to the Mats, Jonas but this time [Marcus Friman](https://www.linkedin.com/in/marcus-friman-32a0434/) so basically I had the whole former Netrounds team to present too. Something happened before the presentation that made me lost my Zen, this is obviously no execuse but this is reality, so in my own evaluation my presentation was far from my Best one given ever but not my worst either.
Was able to handle the questions fired at me, even through one cannot be completely comfortable about an product one hasn't touched before.
<br>
Now the big question my [wife](about/elena) asked me is "Would you like to be a Solution Architect" for Paragon Active Assurance, my answer was YES to this. I believe my knowledge in the Enterprise & Service Provider world can make difference to rolling out this solution. 

Let's wait upon their feedback about my performance and what the next steps would be. I think the former Netrounds team are awesome guys to work with if I get the chance too.

For now this is me sharing my two cents about Juniper's Paragon Active Assurance and my process of perhaps becoming a Juniper Employee.
