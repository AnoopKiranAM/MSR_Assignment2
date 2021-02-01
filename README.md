# MSR_Assignment2

## Metadata   
##### A reproduction as part of the MSR course at MSR course 2020/21 at UniKo, CS department, SoftLang Team   
##### Title: An Empirical Study on Regular Expression Bugs   
##### DBLP link: https://dl.acm.org/doi/10.1145/3379597.3387464  

<br/>
<br/>

## Requirements   
##### Hardware: Windows, Mac or Linux operating system. Good and fast processor.
##### Software: Anaconda, Python(pip install the required libraires mentioned below), Microsoft Excel

<br/>
<br/>

## Process   
### Steps:   
#### **Step:1 Install below third party libraries using below commands**

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**a) Install python 3.7.4 (in Mac)**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sudo apt-get install python3=3.7.4* OR Follow the steps given here for windows - https://phoenixnap.com/kb/how-to-install-python-3-windows 

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**b) Install numpy 1.17.2**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pip install numpy==1.17.2   

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**c) Install pandas 0.25.1**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pip install pandas==0.25.1   

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**d) Install matplotlib 3.1.1**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pip install matplotlib==3.1.1    

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**e) Install GitPython 3.1.0**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pip install GitPython==3.1.0   
  
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**e) Install Beautiful Soup**   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; pip install beautifulsoup4
  

#### **Step:2 Download this github repository**   
**git clone https://github.com/AnoopKiranAM/MSR_Assignment2.git**     

#### **Step:3 Run Anaconda and Open the jupyter Notebook in browser**    

#### **Step:4 Make sure the data.csv file is in the data folder and run the python file "MSR_assignment-2"**     

### Validation:

The output of the execution will be stored in the data folder with the name "result.csv". For the quicker execution we have only taken the pull request of apache repo. With all the 356 Pull request the execution takes more time as it has to scrape all the git repo of the 356 PR's.   
We have scraped the comment and the title of all the PR's and answered the research question 1
#### RQ1- What are the characteristics of the problems being addressed in regex-related PRs?   
We have automated the process which was manually done in the researh paper. We have looped each and every PR. Took the comments, conversations and title and analyzed each of them with the Key word to form a **Root Cause** and **Manifestaiton** which was done in research paper.   
Identified the 3 root cause and manifestation within each type of root cause 







