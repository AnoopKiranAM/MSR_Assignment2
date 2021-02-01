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

#### **Step:4 Make sure the data.csv file is in the data folder and run the python file "[MSR_assignment-2](https://github.com/AnoopKiranAM/MSR_Assignment2/blob/main/process/MSR_assignment-2.ipynb)"**     

### Validation:

The output of the execution will be stored in the data folder with the name "result.csv". For the quicker execution we have only taken the pull request of apache repo. With all the 356 Pull request the execution takes more time as it has to scrape all the git repo of the 356 PR's.   

We have scraped the comment and the title of all the PR's and answered the research question 1

#### RQ1- What are the characteristics of the problems being addressed in regex-related PRs?   
We have automated the process which was manually done in the researh paper. We have looped each and every PR. Took the comments, conversations and title and analyzed each of them with the Key word to form a **Root Cause** and **Manifestaiton** which was done in research paper. Identified the 3 root cause and manifestation within each type of root cause.   
Similarly each of the root cause is again carefully sorted into different category just like the authors have done in Research Paper.   
   
As part of observation of the Research Paper in order to answer the Rsearch Question 1 :Through classifying the root causes and manifestations of those bugs in PR, we show that incorrect regular expression behavior is the dominant root cause of regular expression bugs.   

#### RQ2- What are the characteristics of the fixes applied to regexrelated PRs?   

As part of the answering the research question 2 from the paper we have successfullt automated the things which was manually done in paper. In analyzing the fixes in RegEx related PR's we had to measure the fix complexity with 4 PR featurers proposed in the paper.   
1) minutes between PR opening and merging;    
2) the number of commits in the PR;    
3) the number of lines changed in the fixes;    
4) the number of files touched in the fixes.    
To measure this we have to find the things mentioned above from each of the PR. Which we have succefully done. We have also executed the **Mann-Whitney-Wilcoxon Test** the result of which will be in the python file which is executed which shows the data obtained by the author and the data we have obtained using our methodology are almost same with similar distribution.   


## Data   
### Input Data: 
The input file for the execution is the data.csv file present in data folder. The data.csv file was obtained from the Research Paper.  We have used the column by name "Pull Request" present in [data.csv](https://github.com/AnoopKiranAM/MSR_Assignment2/blob/main/data/data.csv) for our process. We have utilized all the PR link and using the automated process to obtaine the title, comment, conversation etc.., 

### Output Data: 
The result of the execution is stored in the [result.csv](https://github.com/AnoopKiranAM/MSR_Assignment2/blob/main/data/result.csv) file which help us in answering the Research Question 1 of the paper.    

## Delta   
### Process Delta:   
Our process includes the Automation and involves more technical things of what the authors have done manually in the paper. We have tried to answer the RQ1 of the paper quite effectively in finding the root cause, manifestation and category of the PR's.   

But we were not able to continue the anaysis of the of RQ2 to the end as we require the credentials of the other PR's of other repo used by the authors. Plus it was a combursome task to fetch all the code and analyze if there was RegEx addition(RegEx Add) or RegEx Updation(RegEx Edit) or RegEx Deletion (RegEx Delete) or RegEx API changes in the PR. This is where we faltered and couldnot complete the reproduction of the RQ2. Since we coudnt automate the process of fetching the code of every PR using the PR link, we couldnt not suggest the 10 common fix patters to fix either a RegEx Bug or RegEx API Bug.   







