# keshavbararia-langgraph-MAT496
course: https://academy.langchain.com/courses/intro-to-langgraph

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

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module1/chain.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/chain.ipynb

### MODULE 1 - VIDEO 5

<img width="1676" height="1531" alt="image" src="https://github.com/user-attachments/assets/9b2587fc-572b-4cc7-8fac-4356c1e1cd80" />

(Routing workflow visualised on LangSmith.)

**Learnings:**

Learned about routing how it chooses between tool call or direct response based on input.                                                          
Used ToolNode to simply pass a list of our tools to initialize it and tools_condition to build a conditional edge and ToolMessage to respond.        

**Changes:**

Changed the multiplication tool to addition as can be seen in the edited file.                                                                   
Instead of perform 2*2 multiplication, I performed an addition of 2+3 which correctly gave us 5 as output. 

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module1/router.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/router.ipynb

### MODULE 1 - VIDEO 6

**Learnings:**

Learned how to build an agent using LangGraph and LangChain that can perform reasoning and use tools.                                            
Used the agent to call arithmetic tools like add, multiply, divide, or subtract.

**Changes:**
Added subtraction tool as well for more arithmetic operations.                                                                          
Changed numerical values to test different inputs.                                                                                               
Performed: (((5+10)*2)/5) - 1, which gave the correct output of 5.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module1/agent.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/agent.ipynb

### MODULE 1 - VIDEO 7

<img width="2877" height="1506" alt="image" src="https://github.com/user-attachments/assets/9fc5f5d8-7155-45f2-a4c3-a6de1b0b4c94" />

(arithmetic operations using agents in LangSmith studio.)

**Learnings:**

Used MemorySaver to store states for agent to remember.                                                                                             
Learned that graph states are stored in memory using a thread_id.

**Changes:**

Added a subtraction tool to perform more arithmetic operations.                                                                                    
Subtracted 2 in the end to showcase that the new tool was working as well as that previous outputs could be accessed thus showing the effectiveness of MemorySaver.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module1/agent-memory.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/agent-memory.ipynb


## MODULE 2

### MODULE 2 - VIDEO 1

**Learnings:**

I learned how to define and manage a state schema in LangGraph.                                                                                                                                      
Learned how to define a state schema in LangGraph using TypedDict, dataclass, or Pydantic.                                                                                                           
Learned how Pydantic checks data at runtime because of which only correct values are allowed.

**Changes:**

Changed the graph by adding an extra node with "angry" state.                                                                                                                                    
Changed the probability to 1/3 for each node from the original 1/2.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/state-schema.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/state-schema.ipynb

### MODULE 2 - VIDEO 2

**Learnings:**

Learned that reducers helps in resolving overwriting of the state.                                                                                 
Learned how operater.add reducer helps in concatenation of lists.                                                                           
Learned how custom reducers are used to handle none input.                                                                                 
Learned about add_messages reducer and how it helps with rewriting and removal.

**Changes:**

Instead of returning state['foo'] + 1 returned state['foo'] - 1, therefore got {'foo': 0} as output for {'foo': 1} input.                         
Changed the human message to ask about "dolphins" instead of "whales" and changed name from "Lance" to "Keshav".

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/state-reducers.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/state-reducers.ipynb

### MODULE 2 - VIDEO 3

**Learnings:**

Learned how private states are useful for intermediate working logic of the graph.                                                            
Learned how input and output schemas constrain input and output by performing filtering on what keys are permitted on the input and output of the graph.                                                                                                                      

**Changes:**

Changed state['baz'] + 1 to state['baz'] + 2 and got the output {'foo': 4} instead of {'foo': 3}.                                                  
Change name to "Keshav" from "Lance" and got {'answer': 'bye Keshav'} as output.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/multiple-schemas.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/multiple-schemas.ipynb

### MODULE 2 - VIDEO 4

<img width="975" height="555" alt="image" src="https://github.com/user-attachments/assets/fe6138e2-efe8-4627-9072-41891ed744d5" />

( LangGraph trace in LangSmith. )

**Learnings:**

Learned how to manage long chatbot messages in LangGraph using filtering and trimming.                                                            
Learned how to remove old messages using filter.                                                                                                    
Learned how using trimming we can limit number of tokens.                                                                                          
Used LangSmith tracing to see model invocation.

**Changes:**

Changed the human message to know about land mammals other than elephants instead of ocean mammals.                                          
Changed human name to "Keshav" instead of "Lance".                                                                                    
Wrote messages to ask more about tigers and where they are found.                                                                                    
Used gpt 3.5 turbo in addition to gpt 4o.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/trim-filter-messages.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/trim-filter-messages.ipynb

### MODULE 2 - VIDEO 5

<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/653a3356-3754-4f1f-8844-5e2eb0eb2ace" />

( LangGraph trace showing the messages and summary. )

**Learnings:**

Learned how to generate running summary of the conversation without changing the context and also avoiding the use of filters and trimming.
Learned to give the chatbot memory using a MemorySaver and thread ids.

**Changes:**

Changed name to "Keshav" instead of "Lance".                                                                                    
Instead of saying "i like the 49ers" i mentioned Rajasthan Royals my favorite ipl team.                                           
Instead of "Nick Bosa", I mentioned "Yashasvi Jaiswal" and one of his IPL records in the human message.                                          

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/chatbot-summarization.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/chatbot-summarization.ipynb

### MODULE 2 - VIDEO 6

<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/0ef51541-37e9-49ec-86a2-6ecb6360c5f7" />

( Using LangGraph Studio visualised the graph. )

**Learnings:**

Learned how to build a chatbot with summarization and external memory using LangGraph and a sqlite checkpointer.                                                                            
Chatbot stored conversation in a local database allowing recovery even after restarts.                                                                            
Used LangGraph studio to visualise and run the workflow.                                                                                                                                 

**Changes:**

Changed the human message by saying I like Rajasthan Royals instead of 49ers.                                                                        
Asked who was the captain of that team in LangGraph studio.                                                                                          
Changed the name from "Lance" to "Keshav".

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module2/Studio/chatbot-external-memory.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/chatbot-external-memory.ipynb

## MODULE 3

### MODULE 3 - VIDEO 1

<img width="2869" height="1499" alt="image" src="https://github.com/user-attachments/assets/25ca1e2c-6b94-48a8-9f09-6eadec011b34" />

( Agent code with mathematical operations as tools. )

**Learnings:**

Explored different streaming modes like updates, values, and messages to monitor state changes.                                                   
Learned that .stream and .astream methods are used for synchronous and asynchronous streaming.                                                       
Learned how to stream chat model tokens live using .astream_events.                                                                                 

**Changes:**

Made a function format_tool_calls to format list of tool calls into readable string.                                                          
Changed name from "Lance" to "Keshav".                                                                                  
Changed the question "Tell me about the 49ers NFL team" to "Tell me about the Rajasthan Royals IPL team"                                 
Instead of multiplying 2 and 3, multiplied 10 and 5. 

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module3/streaming-interruption.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/streaming-interruption.ipynb

### MODULE 3 - VIDEO 1
<img width="975" height="525" alt="image" src="https://github.com/user-attachments/assets/1352930b-404f-43eb-bc5f-0cdd8a7b8939" />
( Multiplication of 2 numbers using tools in LangGraph Studio. )

**Learnings:**

Learned how to use LangGraph breakpoints to stop the agent at specific steps.                                                                      
learned that using interrupt_before pauses the graph before a specific node executes.

**Changes:**

Added a stubtract function to this list of math functions.                                                                                     
Instead of multiplying 2 and 3, multiplied 5 and 10.                                                                                                

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module3/breakpoints.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/breakpoints.ipynb

### MODULE 3 - VIDEO 3

<img width="975" height="516" alt="image" src="https://github.com/user-attachments/assets/a7c3eece-5956-45a5-a357-efd986fe27a9" />
( Changing the message from “multiply 10 and 5” to “multiply 10 and 6” in LangGraoh studio using fork )

**Learnings:**

Learned how to edit and update a LangGraph’s state when it is running, helping us to modify messages and inputs.                                                                            
Used update_state to change the conversation or add feedback.                                                                                                    
Learned that the human_feedback allows us to give input when the graph is paused.

**Changes:**

Added a subtract function to this list of math functions.                                                                                                    
Instead of multiplying 2 and 3, multiplied 5 and 10.                                                                                                    
Further updated the conversation to multiply 10 and 6 instead of 10 and 5.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module3/edit-state-human-feedback.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/edit-state-human-feedback.ipynb

### MODULE 3 - VIDEO 4

<img width="2877" height="1480" alt="image" src="https://github.com/user-attachments/assets/5479ef63-2e94-4a7f-a460-cef0dd0ea419" />
( Demonstration of interruption in LangGraph studio. )

**Learnings:**

Learned how to use dynamic breakpoints in LangGraph causing the graph to pause automatically during execution using NodeInterrupt                    
Learned how to inspect, resume, and update graph state after interruption.
Visualised the workflow on LangGraph studio.                                                                              

**Changes:**

Changed "hello world" to "hello everybody" making sure that it is still greater than 5 characters as can be seen in the edited file as well as the photo attached.                                                                                                   
Changed "hi!" to "hello" which is still not greater than 5 characters.                                                                

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module3/dynamic-breakpoints.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/dynamic-breakpoints.ipynb

### MODULE 3 - VIDEO 5

<img width="2879" height="1502" alt="image" src="https://github.com/user-attachments/assets/0f182b2f-d111-4a9a-86be-76a793e97096" />       
( Original message. )

<img width="2867" height="1516" alt="image" src="https://github.com/user-attachments/assets/a9944834-ce22-4ebc-99a7-70330bc8becd" />
( Changed calculation by forking. )


**Learnings:**

Learned how LangGraph enables debugging by viewing, re-playing, and even forking from past states.                                                 
Used get_state and get_state_history explored the agent’s progress over time.                                                                   

**Changes:**

Created a subtract function as can be seen in the edited file.                                                                        
Instead of multiplying numbers, I subtracted them.                                                                                                
Showed add function instead of multiplication in LangGraph studio.                                                                                   

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module3/time-travel.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/time-travel.ipynb


## MODULE 4

### MODULE 4 - VIDEO 1

<img width="2879" height="1508" alt="image" src="https://github.com/user-attachments/assets/dfd1fcbc-4ff9-478a-a2b8-aaa6cfe5c442" />
( AI generated answers by taking web search and wikipedia both as sources. )

<img width="2876" height="1530" alt="image" src="https://github.com/user-attachments/assets/743edb3d-4573-4ab5-8d22-3371ceadaf14" />
( Modified question traced on LangSmith. )

**Learnings:**

Learned how parallel node execution works in LangGraph using fan-out and fan-in structures.                                                          
Learned about multi source workflow taking both web search and wikipedia as sources and then generating an output.

**Changes:**

Changed the question "How were Nvidia's Q2 2025 earnings" to "How were Apple's Q2 2025 earnings" and observed the working in LangSmith Studio as can be seen in the photo attached above.

Edited file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Module4/parallelization.ipynb

Original file: https://github.com/keshavbararia/keshavbararia-langgraph-MAT496/blob/main/Sourcecode/parallelization.ipynb
