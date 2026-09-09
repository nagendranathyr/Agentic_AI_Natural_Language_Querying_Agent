# Agentic_AI_Natural_Language_Querying_Agent

This project aims to convert Natural Language into SQL Query, execute and get the answer.

* SQLite is used for database
* 2 tools are created - one to get the schema from table metadata, other to execute sql
* User gives a question --> LLM --> get the schema from tool --> LLM generates SQL --> use execute tool to run query on database table --> LLM presents output in clean manner
* Schema is obtained in the below manner
  * table_name1(col_name1 data_type1, col_name2 data_type2.........)
  * table_name2(col_name1 data_type1, col_name2 data_type2.........)
* Agent using tools and loop back to llm for further processing is called "ReAct Agent"
