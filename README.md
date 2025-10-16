# keshavbararia-langgraph-MAT496
https://academy.langchain.com/courses/intro-to-langgraph

## MODULE 1

### MODULE 1 - VIDEO 1

**Learnings:**

Learned that LangGraph addresses the limitation of language models due to lack of access to tools, external context like documentation.                 
The video explained how basic language models are limited in their capabilities and it introduced the concept of control flow.                          
Learned about chain and agent architecture.                                                                                                           

( No changes and code files since the video was entirely theoretical. )

### MODULE 1 - VIDEO 2

<img width="876" height="661" alt="image" src="https://github.com/user-attachments/assets/71a99a83-6513-47de-a81b-b71b9bb844c5" />
( Modified Graph with extra node. )

**Learnings:**

Learned to use the LangGraph library to build simple graphs.                                                                                         
Learned about the StateGraph, START, END to build and manage the graph.                                                                           
Learned how to connect nodes from START and EDGE.                                                                          
Learned how invoke function is used for execution from START.

**Changes:**

Added an extra node in the simple graph.                                                                                                           
Changed the probability to 1/3 because of the added node.                                                                                          
Gave the new node the state of "bored" which can be seen in the code file and its output.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module1/simple-graph.ipynb                                    

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/simple-graph.ipynb

### MODULE 1 - VIDEO 3
<img width="2721" height="1209" alt="image" src="https://github.com/user-attachments/assets/269b2584-8163-46d5-aff5-ecc82ca43297" />

(LangSmith Studio download.)

<img width="975" height="510" alt="image" src="https://github.com/user-attachments/assets/13604760-56b7-4657-ba09-d3565414764f" />

(New simple graph with extra node opened using LangSmith studio.)

<img width="975" height="517" alt="image" src="https://github.com/user-attachments/assets/1d0874ac-ea32-43c4-9419-8928e6d89396" />

(Agent code to perform arithmetic functions.)

**Learnings:**

Learned to download studio and use it to visualize and test graphs.                                                                           
Learned how LangSmith studio is used to track workflow steps. 

**Changes:**

Changed simple.py to add an extra node and changed its probability to 33% from 50% due to an extra node. The new node had the state of "bored". 
Asked agent graph to multiply 10 and 2 thus performing a multiplication.                                                                                                                            

Code files: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/tree/main/Module1/Studio

### MODULE 1 - VIDEO 4

**Learnings:**

I learned how to a simple chain in LangGraph works by taking chat messages as the state.                                                    
I also learned how to bind tools to a chat model so it can make function calls automatically.

**Changes:**

Changed the messages to know about the best place to see Indian architecture instead of orcas in USA.                                         
Changed the multiplication tool to perform addition instead.



