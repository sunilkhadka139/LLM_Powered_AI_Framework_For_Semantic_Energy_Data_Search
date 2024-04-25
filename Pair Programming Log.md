**Pair Coding Notes**

**General Arrangement**
- Deliver Retrieval-Augmented Generation (RAG) workflow via GitHub by 4/21/2024
- General Steps: 1) Find the right tool/structure/codebase for RAG, 2) enable accurate location of dataset based on user's question, 3) enable accurate data processing based on user's need
- Suggested arrangement of pair coding
-- First 10 minutes: 1) outline tasks, 2) communicate division of labor
-- Last 10 minutes: 1) communicate next steps, 2) communicate take-home tasks, 3) Update the "Pair Programming Log.md"

**Resources**
- RAG tutorial: https://www.deeplearning.ai/short-courses/large-language-models-semantic-search/
- RAG tool: https://github.com/netease-youdao/QAnything
- Google Gemini API setup and usage: https://colab.research.google.com/github/google/generative-ai-docs/blob/main/site/en/tutorials/python_quickstart.ipynb
- AutoGen with Gemini: Runnable with a simple example. Author: Liang Zhang and Sunil Khadka: https://colab.research.google.com/drive/1P9FXjOThefx_gVTsnxzra3cz5rDJ89n6?usp=sharing
- AutoGen with Gemini: Other resources: https://github.com/microsoft/autogen/blob/7265ef1a3fb194e1d3d7345e47e4dc9a30ecd6fd/notebook/agentchat_gemini.ipynb

**Liang's Notes on Test 2**

Type 1 is already finished

Type 2:

Placeholder 1: ["Weather Information","Building Stock GIS Information","Occupant Behavior","Building Characteristics",""Macroscopic energy data,"Microscopic energy data","Comprehensive Data Lake"]

Placeholder 2: ["Residential building", "commercial building", "industrial building"]

Placeholder 3: ["in the year 2020", "in the year 2012", "in Arizona", "in the U.S."]

Prompt: I want to know about [Placeholder 1] in the type of building of [placeholder 2] in [Placeholder 3], generate a list of the relevant open data name

This prompt should be fed into RAG not just LLM.

Type 3: 

Generate about 10 questions. Use your customized question as prompt to ask for relavant open data name. Select 10 good questions, with 8/10 answer available, rewrite it in 10 different questions and the result must be Database
.
Example: "Please give me weather information in Arizona in 2015. What open data should I look at"

Our goal is not to make sure 100% accuracy, but we want to use the right question to test whether RAG and LLM does a good job.

If the accuracy is not good, redo the above 3 types using Gemini.

Type 1, Type 2 and Type 3 reeults for Task 1 on Building Energy Data shared

Test 3. Mannually feed data request to ChatGPT

Procedures: 1 Design 2-3 questions for every dataset 2. for each dataset, update the data to ChatGPT and get answer, 3. copy paste results to the cvs file, 4. judge the restuls, 5. repeat the procedure for 21 times (number of datasets)

Test 4. AutoGen

1. To make sure AutoGen can read google drive data, 2. Use the question designed in Test 3, 3. Designing a prompt to include your question, as well as the data you read., 4. If works well, do the same thing like test 3 to record answers, 5. if not work well, we can discuss in the Friday's pari coding

**4. Transportation Data Set**
1. Design the dataset in more structured way. Then arrange it in tabular fromat and Use RAG to access datas.

4. April 24, 2024**


Outlined Tasks
- Sunil Test 3
- Research on Test 1 and Test 2
  

Take-home tasks and Next Steps
- Idea to solve individual problem
- Maybe Train the Meta Data.

*4. April 17, 2024**


Outlined Tasks
- Sunil Re-do the coding Task
- Pei-Yu does research on Trasnportation Data
  


Take-home tasks and Next Steps
- Complete all task
- Pei-Yu makes transportation data API access


**4. April 10, 2024**
![unnamed](https://github.com/sunilkhadka139/LLM_Powered_AI_Framework_For_Semantic_Energy_Data_Search/assets/33605314/c2b84ba2-0326-4cdb-9bfb-9405ccb5f8b6)
*Revision: "Copy-paste the code" should be "Copy-Paste the Prompt"

Outlined Tasks
- Create function for Task 1.1 and Task 1.2
- Complete Task 1
  

Progress

- Program running for test 1
- Re-arrange the codes to make it look better
 


Take-home tasks and Next Steps
- Sunil tries GEMINI
- Pei-Yu makes transportation data API access
- Task 2: Set of specific question as columns to see result success


**3. April 3, 2024**
Outlined Tasks
- Dictionary in dataset
- Automate the code, edit all the hard coding
- Test Results
- Planning for for-loop and dataframe preparation

Progress

-Dictionary made
-Result Query few tested


Take-home tasks and Next Steps
- Try more prompts
- Task 1: Check all the columns using for loops to check pass/fail
- Task 2: Set of specific question as columns to see result success

  


**2. March 27, 2024**
Outlined Tasks
- Check the code by Pei-Yu
- Discussion with Saquib regarding updates
- Try for Building Energy Data
- Discuss for the improvement and future next steps

Progress

-Data in the Building csv file, Ensure it works.
-Add more columns to make the data more descriptive.
-Test some transportation questions and we cannot provide the most related specific datasets.
-Box got access to token.




Take-home tasks and Next Steps
- Data Structure: Divide the datasets to be more specific to give more accurate results.
- Improve the CSV file so that LLM can easily give better performance
- How related data set is accessible? and Try to make some research regarding this problem.
- How to get data from box drive token?
  



**1. March 20, 2024**

Outlined Tasks
- Liang introduces and shares his RAG work
- Setup the environment
- Start watching video

Progress

-Re-build the code on local environment (anaconda)
-Re-build the code on collab so that we can make it accessible for other team members
> Collab link:  https://drive.google.com/drive/folders/1Yj4SyjR1eUxsHiZfomb1y1z4jT16DBFk

  

Take-home tasks and Next Steps
- Watch the video, understand the logic behind the code
- Do research and try to think of the way to make boxdrive link accesible with the code.  
- Do research on how people deal with different sturcture of the data source to their knowledge base.
- Try to find relevant algorithm for llm to chose between building data and transportation data at the beginning so that llm can know whether user is asking questions related to building or transportation.

[Pei-Yu]

Box: https://colab.research.google.com/drive/1mZVPGVGh6OhoD5SoZV-BMvjzsthPccR-?ouid=109669092208352724855&usp=drive_link
Transportation Search: https://colab.research.google.com/drive/1OanPWbgFUuAyhNS4WEjzCujc0icbpE8M?usp=drive_link
