# Assignment: Identify flaws in a study design

Imagine that you work in a large tech company, Conglomo, that is about to release a new computer security product. The specific product is a new graphical authentication scheme, “GraphicPass,” which allows users to draw a picture instead of having to remember a lengthy text-based password. The business plan involves selling this product to website operators, so that GraphicPass can be used to log into any website.

You lead a team that has been tasked with performing a usability study to compare the performance of this new graphical authentication scheme with that of traditional passwords. Your team designed and performed the study and wrote up the following memo for your review, which describes what they did and what they concluded from it.

Based on the information below, identify *at least* 5 flaws that jeopardize the validity of the conclusions. For each flaw identified, (1) concretely and succinctly explain why it is a problem, and (2) describe how the flaw could be prevented through different methodological decisions.



## Methodology

**Overview:**

We performed a study to compare GraphicPass to traditional passwords. Participants were observed using GraphicPass. Afterwards, we gave them a survey to evaluate each system.

**Experimental Environment:**

All participants were observed logging into the Conglomo employee portal. Currently, the employee portal uses standard textual passwords, so all Conglomo employees are familiar with using passwords on this system, and therefore we did not need to re-test them on traditional passwords. Thus, for the study, we provided them with an experimental version of the employee portal that allowed them to use GraphicPass. Participants were invited to show up in our laboratory, which was a room containing a single computer and two chairs. Each session was performed individually with the participant using the computer, while an experimenter sat next to them and observed.

**Participants:**

Because GraphicPass has not yet been released to customers outside of the company, and to save money on participant recruitment costs, we recruited participants from within our company. We ensured that no participants worked on the team that developed GraphicPass. To recruit participants, we sent an email to other development teams asking for volunteers. In total, ten employees participated. The demographics of our sample were evenly split between males and females, the average age was 31 (range of 22-38), and all participants had either a bachelor’s or master’s degree.

**Protocol:**

Participants arrived at the laboratory and were welcomed by the experimenter. They were told to take a seat at the computer, and the experimenter sat down beside them to go over the instructions. First, the experimenter asked each participant to sign a consent form. Next, they were given an overview of the study:

> *In this experiment, we will be observing you use the GraphicPass system to authenticate to the Conglomo employee portal. GraphicPass is a new product that is being developed by our team to revolutionize how website authentication occurs: it is designed to be faster, less error-prone, and more secure than traditional passwords. During the experiment, we will assist you in enrolling in GraphicPass, and then you will use it to login to the employee portal. At the end of the experiment, we will give you a questionnaire to gauge your feedback and performance.*

After reading the overview of the study to the participant, the experimenter then opened up the GraphicPass demo page, and demonstrated how the system works. Once the participant said that he/she understood the basics of the system, we began the enrollment phase of the study: the participant used GraphicPass to create a new graphical password. Finally, the participant was instructed to visit the employee portal to immediately use GraphicPass to login to the website. For security purposes, no data about the participants’ passwords was collected, and instead the experimenter looked over their shoulders to verify whether or not they were successful. Finally, the experimenter administered a questionnaire that contained 4 questions:

> Please rate the statements below using the following scale: *1: Strongly disagree, 2: Disagree, 3: Neutral, 4: Agree, 5: Strongly Agree*

1.  > *GraphicPass is much easier to use than traditional passwords: \_\_\_*

2.  > *GraphicPass is much faster than using traditional passwords: \_\_\_*

3.  > *GraphicPass is much less error-prone than traditional passwords: \_\_\_*

4.  > *I enjoyed using GraphicPass: \_\_\_*



## Results

After performing our experiment, we analyzed the data by first verifying that all participants had correctly used GraphicPass, and then we examined the questionnaire responses.

Overall, we confirmed that 80% of participants were able to correctly log into the website on the first attempt, whereas the remaining participants were able to correctly do so within three attempts. Thus, we conclude that 100% of our participants were able to authenticate using GraphicPass.

Regarding the questionnaire data, we observed that on average, participants found GraphicPass easier to use than traditional passwords (mean=4.5). They also thought that it was both faster (mean=4.1) and less error-prone (mean=4.2). Finally, participants reported that they also enjoyed using it (mean=4.8). Based on this data, we conclude that GraphicPass is superior to text-based passwords in terms of both security and usability.
