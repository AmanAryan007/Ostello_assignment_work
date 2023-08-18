# Ostello_assignment_work
#In lm_assignments_updated.ipynb  i Added Time of User input And  LLm response

LLM Wrapper
This code implements an LLM wrapper that can be used to interact with a large language model (LLM). The wrapper handles rate limit errors and token limit errors, and it maintains the history of the conversation.
Rate Limit Handling
Rate limiting is used to prevent excessive requests being made to a service or API in a short period of time. It's a common practice to ensure that the service remains available, prevent abuse, and avoid overloading the system.
The handle_rate_limit() function handles rate limit errors by sleeping for the remaining time until the rate limit is lifted.
Token Limit Handling
The truncate_to_token_limit() function truncates a text string to a specified number of tokens. This is useful for ensuring that the LLM response does not exceed the token limit.
Conversation History
The conversation_history list stores the history of the conversation. This is used to format the prompt for the LLM and to track the number of tokens used.
Formatting Prompts
The format_prompt() function truncates the conversation history to the remaining number of tokens. This ensures that the prompt does not exceed the token limit.
Custom LLM-like Response Generator
The generate_custom_response() function generates a response based on the conversation history. The responses are hardcoded in the function, but you can customize them to fit your needs.
Simulating User Inputs
The user_inputs list contains a list of user inputs. The code iterates through this list and simulates a conversation with the LLM.
Main Loop
The main loop iterates through the user_inputs list and performs the following steps for each input:
Formats the prompt.
Generates a response from the LLM.
Updates the tokens used.
Adds the user input and LLM response to the conversation history.
Prints the conversation history and remaining tokens.
Running the Code
To run the code, you can use Google Colab Or Convert This file Extensions into .py and Run By Using Command python File_name.py
