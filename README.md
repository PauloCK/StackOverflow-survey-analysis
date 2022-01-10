# **1. About the Project**

Hi! This project was created to try to better understand what are indicators of good salaries when it comes to tech
careers. Since I'm Brazilian, I wanted to explore further my country's scenario in relation to salaries in tech jobs. 

## **1.1. Business Problems**

I come from an engineering background and I saw many people fail in tests (including me), for example, because they 
had learned to solve some specific cases, not the root concepts of the topic, and because of that they weren't able to 
generalize and solve new problems.

I also wanted to know devs' salaries situations comparing professionals in Brazil and in the US and make the same
comparison between Brazilian professionals who earn in BRL and in USD.

Putting it all together, I wanted to answers the following business questions:

**1** Are the programming languages devs with great salaries want to learn the same ones students want? What other
questions can we create from the results of this analysis?

**2** Are American tech professionals who earn in USD better compensated than 
Brazilian professionals who earn in BRL? What about Brazilian tech professionals
who earn in BRL versus Brazilian tech professionals who earn in USD?

**3** Are tech salaries growing faster in the US or in Brazil?

## **1.2. Data Understanding**

The data used in this analysis was taken from the StackOverflow's surveys from 
2019, 2020, and 2021 and can be found [here](https://insights.stackoverflow.com/survey). 

All of the datasets contains answers from surveys, and in all of them each row
represents one respondent and in the columns are the answers to the survey's 
questions, such as their countries, whether they are devs (if so what type of dev) 
or not, their salaries, etc. If you want to further explore these datasets, please
refer to the link above.

## **1.3. Preparing Data**

In order to prepare the data, since the intention in this analysis was to correlate
*typical* salaries with other information, such as whether the respondent was a 
tech professional or a student and the country of the respondent, we dropped 
rows which contained no information in a field of interest (such as salary) and
trimmed the dataframes removing rows with top 15% of salaries. 

## **1.4. Data Modeling**

In this study no regression or Machine Learning model was used.

## **1.5. Evaluating the Results**

Looking at the results of the analysis, one could see that:

### **1.5.1.** 
In terms of desired programming languages to learn, students and
well compensated devs most of the time want different things, although there is
some overlapping.

### **1.5.2.** 
Brazilian tech professionals who earn in BRL are worst compensated 
when compared to Brazilian devs who earn in USD. The latter are worst compensated
than American tech professionals who earn in USD.

### **1.5.3.** 
The trend of salaries in the US and Brazil to become more even in the 
future was observed observed. But since the data observed was from only three 
years of surveys (the surveys from years before 2019 didn't have information 
about salaries), it could be an indicative that maybe in the next years salaries 
in Brazil will be more competitive compared to US salaries for tech professionals.

# **2. Installations**

All the packages necessary to be able to use the notebook can be found in the *requirements.txt* file

If you want to install them all, execute this command:

    pip install -r requirements.txt

# **3. File Descriptions**

**1.** README.md - This file. This is the guide for the rest of the project :D

**2.** SO_survey_analysis.ipynb - This is the notebook containing the code used to the questions mentioned above 
and the plots in [my post on Medium](https://medium.com/@paulockoff/helping-brazilian-tech-professionals-to-understand-what-to-expect-in-terms-of-salary-f25e9e9ce990)

**3.** survey_results_public_2019.csv - CSV file containing the answers from the 2019 StackOverflow survey

**4.** survey_results_public_2020.csv - CSV file containing the answers from the 2020 StackOverflow survey

**5.** survey_results_public_2021.csv - CSV file containing the answers from the 2021 StackOverflow survey

# **4. Usage**

Open the *SO_survey_analysis.ipynb* notebook and execute the cell with the *!pip install -r requirements.txt* command. 
After installing the necessary libraries, just execute the cells and check the result plots. Feel free to create new 
cells and further explore the data!

# **5. Licensing**

The MIT License (MIT)

Copyright (c) 2015 Chris Kibble

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
