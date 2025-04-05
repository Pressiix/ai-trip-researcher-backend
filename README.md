<div align="center">

![Logo of CrewAI](./crewai_logo.png)


</div>

## Introduction for AI Trip Planner 

This is a project that I personally researched to create an API and service for using multiple AI agents to work together to search information from the internet to help me plan my travel itinerary. I just tell them the name of my origin city and destination city, what interests me when I travel, and the travel period. All the AIs will help me search and recommend travel plans for me, such as:
1. Which airlines can I fly to my destination with? and how much does it cost?
2. What is the weather like at my destination during my arrival? What kind of clothes should I bring?
3. Search and make recommendations about things I'm interested in and related to that place, such as street foods and art toys.
4. Recommend interesting accommodation names in that city.
5. Recommend festivals that will be held during my travel period.
6. Recommend places that are highlights and are worth visiting in that city.

## Tech Stack
- Python 3
- Poetry
- Virtual Environment
- Flask Framework (API)
- CrewAI Framework (Multi AI Agents Framework)
- Langchain
- LiteLLM (Chat with multiple LLM like OpenAI, Gemini, Claude and etc...)
- Langfuse (LLM Chat tracing log)

## Setup
1. Create file `.env` and add the same variables as the `.env.example` file

2. Prepare environment
   ```
   make prepare
   ```

4. Activate virtual environment
   ```
   source venv/bin/activate
   ```

6. Install dependencies
   ```
   make i
   ```

## Start LiteLLM Proxy
1. Open your terminal

2. Activate virtual environment by running the following command in your terminal
   ```
   source venv/bin/activate
   ```
   
4. Start LiteLLM proxy by running the following command in your terminal 
   ```
   litellm
   ```
   
4.You will see the url `http://localhost:4000` (default port is `4000`)


## Start Trip Planner Services
1. Open your terminal

2. Activate virtual environment by running the following command in your terminal
   ```
   source venv/bin/activate
   ```
   
4. Start Trip Planner Services by running the following command in your terminal
   ```
   make r
   ```

6. You will see the url `http://localhost:3001` (default port is `3001`)
