---
title: My Journey to OSCP 2025
categories: [ "Review" ]
tags: [ "oscp" ]
description: Passed the OSCP on my first attempt with 80 points – sharing my full journey, lessons learned, and practical tips.
---

## Introduction

Hey everyone, I recently passed OSCP+ back in June 2025 with one attempt and got 80 points and I wanted to share my experience taking the exam + some tips and tricks that helped me to pass. For a bit of background, I am in IT for just over 2 years, starting in IT Helpdesk and now working as a System Security Engineer at the time of writing. Prior to getting OSCP+, I have other certs under my belt such as A+, Sec+, eJPT and PNPT. While all of the certs are not necessary for OSCP, I do recommend it for building a solid foundation in IT.

### Motivations

Back when I'm on the journey, I have read countless reviews and posts on Reddit to know that many people needed 2~3 attempt to pass. And to be honest, that really scared me but it also motivated me to push harder and to aim for a first-attempt pass, and I’m proud to say I achieved it.

## Getting Learn One

I purchased Learn One back in November 2024 as Offsec usually have 20% discount toward the end of every year. Learn One gives me 1 year of access to the course material and Proving Grounds lab access. It also gives 2 exam attempt. In terms of value/cost, Learn One is better as compared to Course + Cert Bundle as it only gives 90 days acces to course material and lab access, not to mention only 1 exam attempt.

## The Journey

I started studying for OSCP right after I got Learn One in late November 2024. I spent about 1.5 month with 2~3 hour per day going through the course material to about 40%. The progress slowed down around mid Jan 2025 as I got busy with work and life. I started to pick up again in April to go through the course material. To be honest, the course material did not hold up to the price tag as I have hoped for. Sure I have learned a few things here and there, but overall it is not up to par compared to others like PNPT. I have go through PNPT prior to this and I learned more for just the fraction of the cost.

### Building a study plan

It is now mid April and I looked at the timeline I have little more than 7 month to get the cert. With the current pace and what I learned in the course material, it is not going to be enough for me to pass the exam so I had to come up with a study plan and lock in for the remaining days as I have booked my exam on 28 June.

I changed up my study routine by shifting away from just going through the course material and the labs within. Instead, I focused more on doing OSCP-like boxes in HTB and PG, and only visit the course material when I hit a roadblock or needed to brush up on a specific concept. This approach works better for me and I am able to retain the knowledge better.

For OSCP-like boxes I followed a curated list to stay focused on machines that matched the exam style. In my case i used [lainkusanagi list](https://docs.google.com/spreadsheets/d/18weuz_Eeynr6sXFQ87Cd5F0slOj9Z6rt/htmlview#) which is a popular one in the community.

### Pwning boxes

At the start of May, I have only completed 10+ boxes from the list and I felt that I needed to be more efficient as I have only have about 2 months until my exam. So I made a small tweak to my study routine to look up at writeup for a nudge when I’m stuck for an hour to move forward.

Before this, I used to get stuck for 3–4 hours on a single step whether it was the initial foothold or privilege escalation, and I’d feel guilty or even defeated whenever I gave in and looked at a solution. It felt like I was cheating.

It is until I stumble upon this article [It is Okay to Use Writeups](https://www.hackthebox.com/blog/It-is-Okay-to-Use-Writeups) by Ippsec and 0xdf it immediately changed my mindset on how I use writeup. It is all about learning, and in initial stage when I look at writeup, often than not it is a new concept that I don’t even know. So I started embracing that. I took detailed notes, absorbed the concept, and moved on. It made my study process way more productive and less frustrating.

### Note-taking

Taking good notes is one of the most important step in my OSCP prep. It wasn’t just about recording commands or steps but about building a personal knowledge base I could refer back to, especially when I encountered similar techniques later on when doing different box. Note down every commands executed on the target box along with screenshots so able to refer back in the future.

#### Build a high level notes by technique

One of the most effective ways I organized my notes was by **creating a dedicated note for each attack technique**. Instead of dumping everything into one massive note, I structured my notes around individual techniques like Asreproasting, Credentials Dumping and Pivot.

This practice alone helped me tremendously in the exam as I was able to just search for the specific technique in my note taking app to copy and paste the commands and just change the IP address to run it.

### Note taking app

With all the tips I’ve mentioned so far, you’re probably wondering what note taking app I use, and the answer is **Obsidian**.

One of the Obsidian core feature is Wikilink. I am able to link to another note. This is wonderful for my workflow as I can just search for a specific technique, and Onsidian will show me all of the related notes that are linked to it. Let’s take an example, I have a note on Pivot, and in the note I have different note on tools to perform pivot like using Chisel and Ligolo-ng. And each of the tool gets its own note as well.

Apart from Obsidian, there are other good alternative like OneNote, Notion and CherryTree to name a few. Each has its own pros and features so pick your poison.

### Trying Harder

Fast forward to start of June, up until this point I have pwned about 60+ boxes from PG and HTB, averaging about 2~3 box per day. Fortunately for me during the time period, I have some downtime during work so I utilise the time to do more boxes.

#### OSCP ABC

With the challenge labs like OSCP A,B and C it is the past exam set so it makes sense for me to simulate the real exam so I decided to do one every weekend leading to the week before my exam week. No hints for the first 24 hour to simulate the real exam. I got 40, 70 and 30 respectively on ABC. It is worrying at that time because I felt like I am still not ready to take the exam.

With that said, I took on extra challenge and finish Secura and Medtech as well. And to be honest, it is easier for me than OSCP ABC.

## Calm before the storm

Fast forward to 48 hour before the exam date, at this point I have pwned about 90+ boxes including the challenge lab OSCP ABC, Secura and Medtech. Even then, I didn't feel 100% ready. Around 50% of the time I still peek at writeup when I am stuck.

But honestly, I think that’s normal. You’re never going to feel completely ready for something like OSCP. At some point, you just have to trust your prep and go for it. I told myself, "_This is as ready as I’ll ever be_."

### Exam Preparation

At that point, I completely stopped doing boxes and shifted my focus to **reviewing all my notes**. I went through my methodology, double-checked commands cheatsheet, and made sure all the tools were working properly in my VM.

One important tip: **take a snapshot of your VM before the exam**. In case anything breaks or something unexpected happens, you’ll have a clean state to roll back to. It’s a simple step that can save you a lot of stress.

## Exam Day

I booked my exam on 10AM in the morning that day. I woke up at around 8AM, took a cold shower, had a great breakfast. My plan for the exam is as follow:

1. Focus on AD set before lunch as it gives 40 points on entire AD compromise
2. Move to the standalones once AD is compromised
3. Take quick 3~5 min break every hour to clear the mind
4. Stay hydrated throughout the exam session
5. Have fun

**9:36AM**: Eagerly enter the proctoring session and the proctor is already inside so I decided to start the pre-exam verification. The proctor told me to scan around my room with the webcam and I have a unused monitor beside me so I had to unscrew everything and unmount to put in the living room. The entire process took about 20min-ish including setting up my webcam and screenshare. I was able to start my exam around 10:03AM.

**10:03AM**: Everything is set and so I started my exam. Ran autorecon on all the machines including standalones and I focus on the AD set.

**10:30AM**: Scored 10 point on the AD set

**12PM**: Spend the last 1.5 hour to move forward but unable to. Stuck at 10 point so I decided to take a 45 min lunch and to clear my mind.

**12:45PM**: Back to the exam. During lunch I have had few ideas pop up in my mind to try so I tried it all

**2:10PM**: By around this time I had compromise the entire AD network and got Domain Admins. I was so happy at this point and I only needed another 30 points to cross the passing mark.

**2:20PM**: Dive into the first standalone machine

**3:30AM**: Got initial foothold on the first standalone machine, bringing me to 50 points. Could not get root as this point so decided to take a quick break and dive into standalone 2 machine.

**3:40PM**: Start doing Standalone 2 machine.

**6:00PM**: No progress for standalone 2 machine and this is one of the hardest machine I encountered, lots of rabbit hole. I decided to take a longer break this time to get dinner and shower to clear my mind.

**7:30PM**: Back to the exam after 1.5 hour break and I re-visited standalone 1 to get root

**8:00PM**: Finally got root in standalone 1 and this brings my point to 60. I only needed 10 point to cross the passing mark! At this point I start doing standalone 3 to get the remaining 10 point.

**9:05PM**: To my surprise, I successfully compromise the entire machine, bringing my points to 80! I have crossed the passing mark! I was so happy at this time and felt the pressure relieved. Since I have already cross the passing mark, I shifted my focus to getting points to re-compromise the machines and report writing to ensure I have all the necessary screenshots.

**12AM(Second day)**: By this time I have finish most of the report writing. The reason I was able to complete that fast is during the exam, I note every commands and took the necessary screenshots in my note taking app. I just had to copy paste the commands and screenshots into the report and little bit of touchup. Since the report is done, I decided to take another stab at standalone 2 as extra challenge to see if I am able to get 100 points.

**3AM**: Took me another 3 hour but to no avail. I tested everything that I know of, get into every rabbit holes to test out my hyphothesis but no progress. At this point my brain is beyond fried so I decided to sleep and try again in the morning.

**7AM**: Woke up and back to the exam. I ran out of ideas to compromise standalone 2 so I gave up on that. Instead I spent the remaining hour to re-compromise all the machine again from just the commands from my report to make sure it is reproducible.

**9:20AM**: I have triple-checked everything and decided to end my access to the exam and go into report writing phase. I then started to reveiw the note and doing some toucnup on the formatting, fixing typos, include all the links in my report for the exploits that I used.

**12PM**: By this time I have finish everything so I decided to submit my report and concluded my OSCP exam.

## Result

I got my result in the evening on Monday. Althhough the actual wait is just one and half day but felt like forever. I kept checking my phone, refreshing both my email and the Achievements section in the OffSec portal every so often. When I receive the update, it was one of the best feeling ever as all of the hardwork in the past few month has finally paid off. For those that taking the exam, do not give up. I hope this (long!) post gave you some insight or motivation. And if you have any questions, please feel free to reach out to me on Discord.

Below are some of the takeaways from my experience:

### Takeaways

#### Have a solid methodology

Having a good methodology is important to the exam everything about the exam is methodology. Always enumerate fully, try every angle, and leave no stone unturned.

To develop your own methodology, you have to solve different boxes. See my next point.

#### Get exposed to a variety of machines

Volume matters. The more boxes you do, the more patterns you recognize and through that you'll also develop a methodology of your own. Exposure to different setups, misconfigurations, and privilege escalation paths helps build intuition. But it's not just about rooting a box and moving on.

Poke around the machine to see how things are being set up, look for any alternative paths to compromise the machine. I often study different writeup to see how other solve the box, analyzing their methodology, often time I learned about there is alternative ways to get root and that techniques I learned goes straight into my note.

#### Maintain a structured knowledge system/cheatsheet

This is key. During the exam most of the time you'll be referring to own notes. So having an organized note make it easier to find the exact command, tool, or technique you need. The goal here is to make it "copy-paste ready", meaning once you search up the command you can just copy paste to execute it with minimal change.

#### Be Consistent

Be consistent in solving boxes regularly, this is what helps to build the skills and muscle memory. It's better to make steady daily progress than to cram everything at the end. Progress might feel slow at times, but trust the process.

#### Re-compromise boxes using your report commands

During the exam, once you've rooted a machine, go back and re-compromise it using only the commands you've documented for your report. This helps to identify any missing steps in the report
