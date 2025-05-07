Create me a new file called tictactoe.ipynb under src folder of HVEAGENT2 which plays tic tac toe using the template below with a new cell for each step:

- Import the libraries such as random

- Uses the FunctionTool from autogen_core.tools, AzureOpenAIChatCompletionClient from autogen_ext.models.openai, uses AssistantAgent from autogen_agentchat.agents, uses AgentEvent, ChatMessage from autogen_agentchat.messages, SelectorGroupChat from autogen_agentchat.teams

- Define the tic tac toe Board of [" "] * 9 and functions for below:
		- display board()
		- make move(position: int, symbol: str) -> str
		- get best move(symbol: str) -> int without boardstate 
		use display board() in both make move and get best move functions

- Wrap the tools with function tool using above functions created using default data types defined

- use load_dotenv from dotenv and create model client using AzureOpenAIChatCompletionClient() with endpoint details from local env file

- create 2 agents player_x_agent, player_o_agent using AssistantAgent along with system message for each below
	- """You are a Tic-Tac-Toe player and you play as X. First call get_best_move(symbol) to get the best move. Then call make_move(position, symbol) to make a move."""
	- """You are a Tic-Tac-Toe player and you play as O. First call get_best_move(symbol) to get the best move. Then call make_move(position, symbol) to make a move."""

- create selector_func(messages: List[AgentEvent | ChatMessage]) -> str | None: and create team using SelectorGroupChat using model client

- Start the game using team.run_stream(task="Play a game of Tic-Tac-Toe.")

