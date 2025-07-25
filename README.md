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
     
3. Chains
