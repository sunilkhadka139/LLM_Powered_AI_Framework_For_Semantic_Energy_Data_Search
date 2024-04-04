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

**2. April 3, 2024**
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
