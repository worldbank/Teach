# Teach

Teach is a free classroom observation tool that provides a window into one of the less explored and more important aspects of a student’s education: what goes on in the classroom. The tool is intended to be used in primary classrooms (grades 1-6) and was designed to help low- and middle-income countries track and improve teaching quality.

## About Teach
Teach captures practices that nurture children’s cognitive and — for the first time — socioemotional skills.Teach is the first tool to holistically measure what happens in the classroom. It does so by considering not just time spent on learning but, more importantly, the quality of teaching practices.

Teach was developed with low- and middle-income countries in mind and can be contextualized for different settings. For instance, additional elements can be added at the request of the government and local video footage is used to train observers on the tool.
Teach includes a complementary toolkit that helps teams conduct the training with a detailed script and training guide, collect data using a data collection app available in several languages, and clean and analyze data with automatized programs — including assessing the validity of Teach scores. A template report to help communicate the results is also available.
Teach and all its complementary toolkit is free.
In addition to its tailored design, Teach underwent a rigorous development and validation process over a 2-year timeframe. The tool was piloted in over 1,000 classrooms across Mozambique, Pakistan, the Philippines, and Uruguay, and tested with global video footage from 12 low- and middle-income countries. Analyses of the training data indicate that after only 4 days, almost 90% of participants passed the Teach Reliability Exam, which involves coding 3 videos reliably. Please contact us if you’d like more information on the tool’s interrater reliability and other metrics of validation.
For more information on the Teach project please see:

https://www.worldbank.org/en/topic/education/brief/teach-helping-countries-track-and-improve-teaching-quality

## Code Contained in this Directory
Contain code related to the Teach project.  Specifically, some python code useful for creating video-clips

The basic loop does the following:
1.	Read the contents of a folder containing videos
2.	Get a list of all videos
3.	Loop through each video
4.	Check the length of each video
5.	Clip either 0,1,or 2 videos based on the length (if the video is at least 41 minutes long, it clips at 10-25 min through the video and 26-41 minutes.  If under 41 minutes, it clips between 10-25 minutes, and if under 25 minutes, it will skip the video
6.	Produce 15 minute clips.
7.	Save the video clips
