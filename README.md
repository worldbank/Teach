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
The code in this directory contains python code useful for creating 15 minute video clips from the Teach video recordings of classrooms.  The 15 minute clips are then used by the Teach scorers to evaluate teacher pedagogical skills.

The basic loop does the following:
1.	Read the contents of a folder containing videos
2.	Get a list of all videos
3.	Loop through each video
4.	Check the length of each video
5.	Clip either 0,1,or 2 videos based on the length (if the video is at least 41 minutes long, it clips at 10-25 min through the video and 26-41 minutes.  If under 41 minutes, it clips between 10-25 minutes, and if under 25 minutes, it will skip the video
6.	Produce 15 minute clips.
7.	Save the video clips

### Prerequisites

The user will need a modern version of Python 3 installed on their machine.  In my opinion, the easiest way to install python is to download the Anaconda python distribution, which includes a number of pre-installed packages for data science.

The link to download can be found here:

https://www.anaconda.com/distribution/

Once python 3 is installed, you will need the following packages:

1. moviepy.editor # Import everything needed to edit video clips

2. pathlib #import tool for dealing with files and paths

3. IPython.display  #Allow showing video in python notebook

4. os.path #some tools for navigating files and paths

### Customization Required before Running

The repo contains two files: the teach_video_slicer.py and the teach_video_slicer.ipynb.  The files are nearly identical, but the .ipynb is converted to be used in Jupyter notebooks, whereas the .py file can be read in any instance of python 3.

I will provide instructions for the .py file, but the .ipynb file should proceed similarly.

1. You will need to modify the directories in line 26, 27 to match your needs

2. You will need to modify the test file path in line 38, based on your system
