---
layout: post
title:  "Systems, Security and Startups - Prof. Peter Druschel, Max Planck Institute for Software Systems, Germany"
author: stan
categories: [ Interview, Systems, Research, Security, Startups ]
image: assets/images/peter_druschel.jpg
featured: true
toc: true
---

_Prof. Peter Druschel is the founding director of the Max Planck Institute for Software Systems (MPI-SWS) and Associate Chair of the Chemistry, Physics, and Technology Section of the Max Planck Society in Germany. Previously, he was a Professor of Computer Science and Electrical and Computer Engineering at Rice University in Houston, Texas. His research interests include distributed systems, mobile systems, privacy, and compliance. He is the recipient of an NSF CAREER Award, an Alfred P. Sloan Fellowship, the ACM SIGOPS Mark Weiser Award, a Microsoft Research Outstanding Collaborator Award, and the EuroSys Lifetime Achievement Award. Peter is a member of Academia Europaea and the German Academy of Sciences, Leopoldina._

> **Foreword:**
Prof. Peter has had an unconventional journey to being an academician; it’s not usual to find a professor who used to be an entrepreneur at some point. On one hand, you see professors starting companies while on the other, you meet Peter who is convinced that he isn’t returning to the bootstrapping scene. It would be right to say that the skills required to start an entity from scratch can benefit the research process; an appetite for risk is a crucial skill, for example, that is common to both worlds. I strongly believe that start-ups and research have quite in common; an interesting YouTube talk, “The Lean Researcher” by Alistair Donaldson expounds further. In this interview, Prof. Peter discusses these topics and other interesting questions such as:
* Do you need industry experience before getting into Systems Research?
* What constitutes an optimal work-life balance during Ph.D.?
* Views on security, cryptography, ML, theory, and practice,
* What are the possible research opportunities at MPI-SWS? And more …
Stanly Samuel, Ph.D. student,  CSA, IISc

This interview between **S**tanly **S**amuel, **M**ahak **P**ancholi, CSA, and Prof. **P**eter **D**ruschel.

### SS: Can you tell us about your academic background and how you got interested in distributed systems? What/ Who were the major influences when you took this decision?

PD: I had a somewhat unconventional academic career. I first went to a University of Applied Sciences - Polytechnique as they call it - because, at that time, I was very interested in engineering that involved building systems. I was not very interested in the sciences. So, I got a degree there. While I was at university, we founded a start-up company that marketed electronic control systems that go into buses and public transportation. These devices were used to print tickets and control various signals. Since this was around 1982, the idea was very novel.

I worked with this company for two years. Initially, it was very exhilarating as you built a business that had many technical challenges. But after a few years, it became very monotonous. Customers would have new requirements for something that you had already done but slightly different. It wasn't really attractive anymore. However, I realized that interactions were becoming more and more software-based and, computer science was becoming crucial and important. I had an EE background at the time, so I decided I'll go back to university and pursue a graduate degree in computer science back in the US, and that's how I got into the academic career.

You also asked about distributed systems, but my first interest actually was more in operating systems. In the early 90s, there was a lot of work going on in getting operating systems ready for high-performance computing networks, graphics, and multiprocessors. These were all new at the time. Then over time, of course, systems work has gone more into distribution - distributed systems became pervasive, and I got into distributed systems as well. More recently, in the last 5-10 years, I've also developed an interest in Mobile Systems.

### SS: How did this transition from the start-up world to academia affect your research career? Also, do you recommend industry experience before academic research?

PD: I took this particular path, so it's a little bit hard for me to say with certainty. But, I've talked about this with many people, and this question comes up regularly with students too, and all I can say is that I don't think there is any harm in working a little bit in the industry although I am not convinced that it's an absolute must.

But if I think about it hard, then the two things that I learned there that benefitted me later are - first, I realized that getting a piece of software or a product into actual practical use is much more complicated than you think. It's one thing to get a part of a program to work and substantial additional effort to actually getting it to production use. So that was certainly interesting, but I am not sure you have to have that experience yourself to know it. The other thing is that it somehow eradicated my curiosity about what it would be like. Unlike many of my colleagues who always thought, "Ugh, I wanna do a startup at some point! I've never done this!", I was never tempted (laughter). I had seen that side before.

### SS: Which area in Computer Science should we be looking at for the next decade?

PD: All of us are biased by what we are personally interested in. I could, of course, tell you all the things that I work on, but that wouldn't be fair as that's my personal take. But generally speaking, I think security and privacy are hugely important themes, and so is ethics in computing. Not to say that other things are not interesting - I mean, there are tremendous advances in AI and vision and NLP, but the issues that fire me up more and where I see potentially game-changing decisions being made, are in security and privacy. The reason is that the way society uses computing technology will depend on how we position ourselves related to these subjects in the next ten years. This may not be as critical as it may seem and it may not be the same in all parts of the world. Nevertheless, I have a feeling that, in society, as computing becomes more pervasive, it entrenches positions that affect everybody. For example, credit applications, job applications, what news you see, whom you get introduced to on social networks, etc will be soon be managed by computing technology, algorithms, and machine learning. These are such deep influencers on people’s lives that people will sooner or later start asking questions about fairness, about issues like discrimination, about issues of what happens with my private data, and what's the balance of power between someone who is just a consumer, someone who releases their data, the corporations - perhaps the governments - that are using this massive data and how much knowledge can be extracted. I think this is really critical, and security is tied to that as well.

So, I guess anything that combines a computer science area (say X) with aspects of privacy, security and fairness, ethics - questions about how this affects society are, I think, super important, but this is just my opinion. I think people are beginning to realize just how pervasive computer technology impacts people.

Of course, there is all the hype about machine learning - I don't mean it is negative, it's a very powerful technology - but of course, it now has become massive in the public's eye, probably also due to its unfortunate name, which makes people expect too much, probably even scares some but nevertheless, I think it's present on everyone's minds.

### MP: I am a master's student, and I am working in cryptography. The way I see it - there's security, and then there’s cryptography. Cryptography approaches privacy in a more theoretical sense while security is more practical and well, doesn’t give proofs and theoretical guarantees. Do you think we need to bridge this gap from theory to practice? I don't see crypto being applied a lot in the real world. What are your thoughts on this?

PD: So I think there is a certain bias. Much of the work being done in cryptography is very interesting intellectually, but it's not so clear how to use it in practice; this is maybe one thing. On the other hand, I am also surprised how little concepts like - time signatures, encryption, and similar ideas are used in practice. There might be a long road there because people are a little worried, particularly in production environments, about using and depending on tech they don't fully understand. So I think it is partly a matter of education as well. I feel the other issue is that we often have this idealized goal to have provable guarantees of everything. But we know proving security is impossible, and with privacy, it's even direr right? Differential privacy shows you that there is no easy way out. If you want strong privacy, you need to give up utility, and in some cases, it's a terrible trade-off.

So, I think we need to also get on both sides. I think the general population needs to be more comfortable and more knowledgeable about cryptography. At the same time, security researchers - may be also cryptographers - need to get more comfortable with the idea that sometimes we cannot have hard guarantees. We need to settle for raising the fence to a certain level and hopefully have a good understanding of how high the fence is - what that means is focusing on where the remaining threats are. I hope this makes sense.

### SS: You've worked with many esteemed researchers and scientists. Would you like to share any interesting stories or something you think a general audience would benefit from?

PD: I'm very privileged to have met very smart people with exceptional skills but interestingly, having been really gifted intellectually is not a guarantee of success when you do research. I have seen some people much, much smarter than I am and they never made it through graduate school because somehow they couldn't get the balance right between time management, focus, risk-taking, and all these things that play into it.

>Interestingly, having been really gifted intellectually is not a guarantee of success when you do research.

But this is not a negative, right? I don't view these people as failures, and I don't consider it as a failure to have not succeeded in this. It just means that it wasn't a good match. I think we're all very differently talented, and I think it's a problem of finding your niche, finding the right niche. At the same time, we are incredibly fortunate to be able to work in a world where ideas matter, not only money and power; although the latter plays into it as well, it is not the primary thing. I feel highly privileged for that.

### SS: I'll ask you the last question then, based on what you just said. How do you actually choose a good idea? I understand that identifying a good idea comes from experience but is there any way to [in some sense] deterministically say - "yes, this is a good idea"?

PD: I have to say - I really don't know. But what I can recommend to you and what I keep following myself is this: when you have an idea, talk to lots of people. I feel this is very practical. Don’t just talk to people who are inclined to believe you because they are looking up to you; for example, your juniors or people less experienced in the area. Talk to various people from different sub-disciplines, including people who are very strong in your area. See what they say. You're not always getting unanimity in their opinions; that’s not required. But you get a much better idea of how the idea resonates with people, what their concerns are, and even if you go for it, you'll have a much better sense of what it will take to demonstrate the idea - how to convince people, as you know the counter-arguments.

But honestly, I can't explain how to pick an idea and I am not sure I have the magic bullet. Sometimes I have ideas that I am really excited about, but after reflecting on them and talking to people, I say, "Nah”!

### Prof. Narahari, CSA: Can I ask a question? What will be the opportunities for graduate students and Ph.D. graduates from CSA, IISc at MPI-SWS?

PD: There are plenty of opportunities, typically across the system. We have now four institutes in computer science [MPI-INF, MPI-SWS, MPI-IS, MPI-SP], so by all means, if you're interested in an academic career, apply to us. Also, if you're interested in internships, do apply. Internships are generally open to undergraduate students but are also open to graduate students if it's a good match.

For graduate students, the match matters because these students are generally involved in some primary area of research. I think it might make sense to do an industrial internship to get that industrial experience where you may be expected to do something unrelated to your primary research; this may be okay early in the research career. But, when you go into an academic institute, there should be some match of interest. So, there needs to be a match, but by all means, we're very happy to have you.

### SS: The trend I have seen is that students apply through the internship portal. However, it helps more if you know the professor or researcher you want to be working with, beforehand. How do you think a student should go about making that initial contact?

PD: It's a bit hard- the problem is that it’s difficult to stand out because we get lots and lots of emails. So, the ideal situation is when you have met the person, say, at a conference or when he/she visits the organization. But nevertheless, I think, to me, it's always impressive when I get an email and see that they've done their homework i.e. they've read my papers, they've something intelligent to say or to ask; this is the sort of thing that stands out. I am not looking for is a complete research proposal.

Sometimes I get an email that says, "I want to do the following" and they have some idea which may be good or not so good, but it's not within my current scope of things to invest time in and it's not a good match [then it won’t work out]. Thus, in general, if you see that someone has made the investment to read up on the work that is going in the institute or in the group, that's likely to catch people's attention.

### SS: Thank you Peter for the chat. It was a good discussion. That’s all we have from our side.

PD: Thank you very much. This was fun, you're very professional when you're interviewing. It was very well done.

### Other questions answered in the [longer version:](https://qr.ae/pGInn5)
* SS: To come back to the previous topic - now that we have broached the subject of machine learning - what are your exact views of this particular area, and where it is headed? (since you seem to have certain strong views on that.)
* SS: What do you do apart from work? For example, I see that you are interested in heavy metal concerts, I don’t know if you’re a musician, but is there any side of you that you'd like to share with the general audience, and how does that help you complement your research?
* SS: Any particular specific advice apart from what you just said which can help a graduate student?

>I think you need balance in life; a lot of technically inclined people underestimate this fact. The following statement might be controversial but the world doesn't operate on math. It operates on human relationships. So you cannot neglect these aspects even if it might be very exciting to get deep into technical stuff. This is important to keep in mind.

**Credits:**

* **Interviewed by:** Stanly Samuel, Ph.D. student, and Mahak Pancholi, MTech 2018–2020, CSA[with Prof. Narahari towards the end]

* **Transcribed and Compiled by:** Gokulnath Pillai, MTech 2020–2022, CSA

* **Final Editing by:** Stanly Samuel

**CSA Writing Team (CWT)**