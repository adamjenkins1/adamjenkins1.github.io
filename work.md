---
layout: default
title: work
group: "navigation"
---

<h2>Work History</h2>     
<ul>

<h3 style="display:inline;"><a href="https://www.veeva.com/" target="_blank">Veeva Systems</a> - Security Engineer Intern</h3> 
<h4 style="display:inline; float:right;">May - August 2018</h4>
<p>While at Veeva, I worked in collaboration with additional security engineers
to design and implement an incident response Slackbot.  The purpose of this 
Slackbot was to notify us when we received an alert from our several security 
alert applications. When an alert was received, the bot posted to the Slack 
channel and provided the ability for users to open a 
<a href="https://www.atlassian.com/software/jira" target="_blank">JIRA</a>
ticket for the triggered security alert, or dismiss it. We decided to implement 
this Slackbot in <a href="https://kubernetes.io/" target="_blank">Kubernetes</a>
and designed the project with the decoupled micro-service architecture in mind.  
To elaborate on that, each micro-service of this bot (posting to the channel, 
listening for the alerts, creating the ticket, etc.) was implemented as its own 
<a href="https://www.docker.com/resources/what-container" target="_blank">container</a> 
in our Kubernetes cluster. Our Slackbot was hosted on AWS 
<a href="https://aws.amazon.com/eks/" target="_blank">EKS</a> which is Amazon's managed Kubernetes service.
Over the course of the internship, I completed 
the <a href="https://minio.io/" target="_blank">Minio</a> and JIRA containers 
(this included the <a href="http://flask.pocoo.org/" target="_blank">Flask</a> 
<a href="https://www.codecademy.com/articles/what-is-rest" target="_blank">REST</a> 
<a href="https://medium.freecodecamp.org/what-is-an-api-in-english-please-b880a3214a82" target="_blank">API</a> 
to create the JIRA ticket), and worked on the incident response container which was responsible
for parsing alerts.  I also created a <a href="https://helm.sh/" target="_blank">Helm</a> 
chart to organize and generalize 
our Kubernetes deployments.  Later, I implemented 
<a href="https://rollout.io/blog/blue-green-deployment/" target="_blank">blue/green deployments</a> 
for our Slackbot and built the automation pipeline using 
<a href="https://about.gitlab.com/features/gitlab-ci-cd/" target="_blank">GitLab CI/CD</a>
to automate the test, build, deploy, and release stages of our software. 
By the end of the internship, I had learned <a href="https://kubernetes.io/" target="_blank">Kubernetes</a>, 
<a href="https://www.docker.com/" target="_blank">Docker</a>, 
<a href="https://helm.sh/" target="_blank">Helm</a>, 
<a href="https://about.gitlab.com/features/gitlab-ci-cd/" target="_blank">GitLab CI/CD</a>, 
<a href="http://flask.pocoo.org/" target="_blank">Flask</a>, 
and numerous <a href="https://aws.amazon.com/" target="_blank">AWS</a> services.
</p>

<h3 style="display:inline;"><a href="http://www.llnl.gov/" target="_blank">Lawrence Livermore National Lab</a> - Computation Intern</h3> 
<h4 style="display:inline; float:right;">January - August 2017</h4>
<p>After completing the Fall semester in 2016, I was hired for a co-op internship at Lawrence Livermore National Laboratory. 
While at the lab, I primarily worked on two web applications: the Student Poster Grading Application (SPGA) and the Java Cafe Replacement Application.
Every year at the Annual Student Poster Symposium, faculty used to grade student posters by hand and requested a website to make the process a bit easier. 
My job for this project was to redesigned the existing JavaEE application to use the Java Play Framework and AngularJS 
and also make design changes to improve user experience. I worked closely with my mentor and the other clients to ensure that the 
application met the users' needs and also implement any changes they proposed to improve functionality. This was my first major
web application, so it was a great opportunity to learn how to implement a website backend that worked together 
with the adaptive frontend built with AngularJS.  During the Annual Student Poster Symposium, SPGA was used by faculty members to grade
several hundred posters and deliver concise and human readable results in the form of an Excel spreadsheet. The Java Cafe Replacement Application was meant 
to do what it's name suggests: replace Java Cafe.  Java Cafe is an old Java web framework and I was tasked with replacing it with a 
Java Play/Angular 2 application. By the end of my internship, I had completed the first screen which allowed users to 
alter which employees worked on which tasks. This project has since been passed on to other employees to complete.
</p>

<h3 style="display:inline;"><a href="http://www.csuchico.edu" target="_blank">CSU, Chico</a> - Lab Assistant</h3> 
<h4 style="display:inline; float:right;">August 2016 - Present</h4>
<p>I am currently working as a lab assistant in the Butte Hall computer labs on campus. 
My primary task is to open the labs for students and faculty to use and resolve any technical issues 
that may arise. Ocassionaly this means helping professors learn how to better use the technology we have, 
but more often, I spend the majority of my time maintaining and repairing all of the computers in the labs. 
However, there are multiple side jobs that my supervisor brings to me when faculty have more complex problems. 
For example, this included replacing a faculty member's iPad screen. I also designed a new form for the 
tutoring labs that allows professors to track how long students spend in the tutoring labs, the purpose for their visit, 
and multiple other fields. This form replaced the previous Microsoft Access form that both students and faculty had trouble using. 
Professors can also download all of the data as a .csv and conduct their own analysis if they wish.</p>

<h3 style="display:inline;"><a href="http://www.jewishlearningworks.org" target="_blank"> Jewish LearningWorks</a> - Marketing and Development Intern</h3> 
<h4 style="display:inline; float:right;">Summer 2015</h4>
<p>During the summer of 2015, I was an intern at Jewish LearningWorks 
(previously known as the Bureau of Jewish Education), 
<a href="https://www.google.com/maps/place/Jewish+LearningWorks/@37.7760083,-122.4731152,15z/data=!4m5!3m4!1s0x0:0x3d00aeefab06495b!8m2!3d37.7760083!4d-122.4731152" target="_blank">located</a> 
in the Richmond district in San Francisco. My primary goal was to assist in migrating content from 
their old website hosted by soapbox, to their new website hosted by Squarespace. I also worked with the 
graphic designer to properly display content using IFrames as well as adding visual content to the new website. 
On my free time, I taught myself the basics of Javascript using <a href="https://www.codecademy.com/" target="_blank">codecademy</a>.</p>
<br>
<p>My most current resume can be found <a href="Data/media/pdf/resume.pdf" target="_blank">here</a>.</p>
</ul>
