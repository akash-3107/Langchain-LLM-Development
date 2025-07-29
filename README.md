# Langchain-LLM-Development

Developed an understanding of Langchain in LLM Application Development.

Touch based on following topics until now :

1. Models, Prompts and Parsers (Model_Prompt_Parser.ipynb)
   
2. Memory (Memory.ipynb)
   - Conversation Buffer Memory            : Allows storing of messages and extracts the messages in a variable
   - Conversation Buffer Window Memory     : Keeps a list of the interactions of conversations over time. It only uses the last 'K' interactions
   - Conversation Token Buffer Memory      : Keeps a buffer of recent interactions in memory and uses token length rather than number of interactions to determine when to flush interactions
   - Conversation Summary Memory           : Creates a summary of the conversation over time
   - Vector Data Memory                    : Stores text(conversations) in a vector database
   - Entity Memory                         : Remembers details about specific entities
   - Multiple memories can be used in combination
   - Conversations can also be stored in SQL databases
     
3. Chains (Chains.ipynb)
   - LLMChain             : Simple Chain Structure
   - SequentialChain      : Combination of multiple chains where output of one chain is input to another chain
   - RouterChain          : After reading the input, the Router Chain decides which next simple or sequential chain to route to
  
4. Question and Answer Format (QnA.ipynb)
   - RetrievalQA (Document Retrieval)
   - DocArrayInMemorySearch (In Memory Vector Store)
   - Require Embeddings and Vector Databases for Large Incoming Documents
   - Methods for querying (in case of multiple large documents)
        - Stuff method (Basic)
        - Map Reduce (Passes chunks through queries to LLMs and finally uses another language model to combine the answers to get a final response)
        - Refine (Builds upon the answer from the previous document)
        - Map Re-rank (Assigns scores to response and then builds a final response)
          
5. Evaluation (Evaluation.ipynb)
   - Evaluation of chains
   - QAGenerationChain (Input documents and create question answer pair from it. It uses a language model to do that)
   - QAEvalChain

6. Agents (Agents.ipynb)
   - Can be integrated with built-in tools, wikipedia or python (PythonREPL) agents