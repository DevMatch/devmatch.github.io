---
layout: post
title: "Hiring Process for Extropolis"
date:   2023-06-02 23:45:29 -0800
categories: docs
---

# Extropolis AI: Case Study
## How DevMatch Assisted Extropolis in Improving their Hiring Process Finding Machine Learning Operations Engineer for Extropolis 

<img align="right" src="/images/extropolis-case-study/extropolis-intro-image.png">

### Introduction
Extropolis is a local tech startup that specializes in the development of generative-AI mobile apps for image generation and voice assistants. With a keen understanding of the challenges involved in productionizing machine learning, Extropolis navigates the complex machine learning lifecycle, including data ingest, preparation, training, tuning, deployment, monitoring, and explainability. Collaboration and seamless hand-offs between teams are vital, from Data Engineering to Data Science to ML Engineering.   

Extropolis is currently seeking a talented and part-time MLOps Engineer to join the team. The ideal candidate will possess a strong background in machine learning, software development, and DevOps practices. Key responsibilities for this role include developing, deploying, and maintaining machine learning models to power the unique and innovative art generation features of Extropolis' mobile apps. 

The candidate should have practical experience scaling RESTful applications and Python, particularly in computing-intensive workloads like Machine Learning. They should thrive in a dynamic, fast-paced environment and be willing to continuously learn new frameworks, tools, and cloud vendors. Familiarity with Docker containers, RESTful frameworks such as FastAPI, and reverse proxies like Nginx or Traefik is highly desirable. Additionally, understanding and optimizing performance, including Service Level Agreements (SLAs), is crucial. 

Extropolis values trustworthiness in handling sensitive data and maintaining data integrity. By joining the Extropolis team, the candidate can contribute to cutting-edge generative AI technology while working alongside a dedicated and passionate team. 



### Setting up a hiring process
#### Challenge: Identifying the Right Skills and Matching Candidates 

Normally, DevMatch is a self-service platform, but we do find time to time customers that need help with more than the tech assessment, such was the case with Extropolis. First thing we did was to stablish a hiring process. We created a schedule of when things were going to happen.

* Definition of the profile. This includes calibration.
* Sourcing and launching application.
* Technical assessment. 1 hour technical assessment on DevMatch.
* 15 minute chat with the founder.
* 45 minute final interview.

There are things that cannot be tested in a technical assessment, the idea is that we test basic qualification so that later in the pipeline we can asses cultural fit. Having DEMONSTRATED qualifications, now the Extropolis team could have longer cultural fit meetings with the candidates.
https://www.loom.com/share/3f4877da640143f497768e0998eeaa94

<figure class="video_container">
  <iframe src="https://www.loom.com/embed/3f4877da640143f497768e0998eeaa94" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

### Sourcing
We attended career fairs, and supported Extropolis with an ATS in which candidates could apply. We also published the job description in other relevant job boards both relevant to MLOps and startups. Since this was for a junior engineer, we also did it on job boards popular amongst students.

![Group of students talking to a recruiter](/images/extropolis-case-study/career-fair1.png)

![Overview of crowd at the career fair](/images/extropolis-case-study/career-fair2.png)

The top 3 schools were University of California, Irvine, San Jose State University and University of Washington.  

### The DevMatch Assessment
Extropolis recognized the need for a Python/ML assessment on the DevMatch platform, specifically tailored to the real-life scenarios the team is currently facing. The goal was to create a realistic and approachable assessment within one hour while ensuring candidates couldn't trivially solve the question with the assistance of AI.
 
To design the assessment, the DevMatch team referred to the job description and identified the required key skills. These included knowledge of Python, distributed computing, parallel processing, root cause analysis, experience with FastAPI, uvicorn, Docker, Kubernetes, monitoring tools like New Relic, familiarity with load balancing technologies such as Nginx and Traefik, proficiency in popular machine learning frameworks like Hugging Face Transformers, Diffusers, and PyTorch, as well as a solid understanding of DevOps practices, Git, and experience with platforms like GitHub, GitLab, or Bitbucket.
 
From these essential skills, we extracted the core areas of focus for the final interview: git, uvicorn (rest APIs, services), Python, hugging face, and pytorch. By aligning the assessment with the candidate's expected responsibilities, the interview can delve into performance improvements and design decisions, establishing a shared context between the interviewer and the candidate. Understanding performance, especially regarding Service Level Agreements (SLAs), is deemed essential.
 
The assessment task involved working with a Python web application that utilized a pre-trained image-text model called CLIP to generate textual descriptions of uploaded images. The Hugging Face library transformers were utilized to load the CLIP model. The process of image description generation revolved around comparing the uploaded image features to a set of text features corresponding to different image classes in the CIFAR100 dataset. The starting code for this task was made available in a Git repository, providing a foundation for the candidate to work with.

![DevMatch MLops Assessment](/images/extropolis-case-study/assessment.png)
![Candidates pipeline](/images/extropolis-case-study/pipeline.png)

Candidates started solving the assessment and we had a 64% open rate. This is because some people don’t bother to open the project, or they didn’t see the invitation email or better yet, they open the project/problem and they see that this is not the sort of job they want to take part in.

In the end, only 45 candidates (35.7%) submitted something, anything, and out of those, only 19 scored 100 points in the assessment.
The ranking shows each candidate individually so that we know when they started and their submissions.

![Ranking of candidates](/images/extropolis-case-study/ranking.png)
![A submission made by a candidate](/images/extropolis-case-study/candidate-submission.png)

### Feedback from Candidates
![Positive feedbacks](/images/extropolis-case-study/positive-feedback.png)
![Pain points](/images/extropolis-case-study/pain-point.png)
![Graph of average rating](/images/extropolis-case-study/average-rating.png)
![Quotes from candidates](/images/extropolis-case-study/testimonials.png)

### Improved Candidate Experience
Candidates expressed their satisfaction with the DevMatch platform, citing the engaging and authentic coding experience it provided. The automated skill assessments offered a realistic and challenging simulation, allowing candidates to showcase their skills effectively. Instantaneous feedback and transparent evaluation enhanced the overall candidate experience.

### Solution: DevMatch's Approach
Automated Skill Assessments: To address Extropolis' specific requirements for the MLOps role, DevMatch provided a suite of automated skill assessments. These assessments allowed Extropolis to evaluate candidates objectively and efficiently, eliminating the need for manual assessments and reducing bias.

Enhanced Candidate Engagement: DevMatch's integrated development environment (IDE) empowered candidates to showcase their skills effectively. This immersive experience increased candidate engagement and improved the accuracy of skill assessments.

### Results: Efficiency and Quality Improvement
The collaboration between DevMatch and Extropolis yielded significant improvements in the hiring process, leading to the following outcomes.

[comment]: <> (There should be a list of outcomes but there is currently only one right now.)

1. Increased Conversion Rate:  The integration of DevMatch with Extropolis' hiring process significantly increased the conversion rate from application to on-site interviews. Candidates felt empowered to demonstrate their skills, resulting in a higher number of completed applications and a stronger pool of qualified candidates.

### Conclusion
By collaborating with DevMatch and leveraging their innovative hiring platform, Extropolis successfully improved their hiring process and overcame the challenges of skill assessment and candidate matching. DevMatch's integrated approach, which included a simplified application process, automated skill assessments, an immersive coding experience, and data-driven decision-making tools, enabled Extropolis to attract, assess, and select top talent efficiently. The partnership between DevMatch and Extropolis exemplifies the power of utilizing advanced technology to optimize hiring practices and achieve remarkable outcomes.
