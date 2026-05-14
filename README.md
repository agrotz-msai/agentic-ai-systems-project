# agentic_ai_systems_project
This my sixth project in the capstone course of Udacity's Master's Degree in AI (https://www.udacity.com/masters-artificial-intelligence). 

## Overview
In this project, we design, implement, and evaluate a small-scale agentic AI system using agent design and orchestration techniques from Udacity's Agentic AI Nanodegree. 
Our use case is a web-based competitor analysis in marketing research. We define a research agent with limited memory and access to a web search tool that produces the report, 
as well as a stateless review agent that checks the report for specific criteria and provides feedback. 
The workflow is then set up as a research-review loop that runs until the review agent accepts the report.

We start by some imports and initializations. Then we define the research and the review agent, tie them together in an agentic workflow, 
and evaluate that workflow for different scenarios. A short summary concludes the notebook.

## How to run the project
The main component of the project is the Jupyter notebook 'agentic_system.ipynb'.
Note that in order to run the notebook, valid API keys for OpenAI and Tavily are required, which need to be set in the ".env" file contained in the repository.

The repository contains a 'requirements.txt' file with all required dependencies, which was generated via the command
	
	pip freeze > requirements.txt
	
It can be used e.g. in a virtual Anaconda environement by opening an Anaconda prompt window in the project directory and running the following commands:

	conda create -n env_msai_cap_6 python
	conda activate env_msai_cap_6
	pip install -r requirements.txt
	python -m ipykernel install --user --name=env_msai_cap_6
	jupyter notebook
	
The last command opens a Jupyter GUI, where one needs to click on the notebook 'agentic_system.ipynb' and then click on Run... -> Run All Cells

In addition, the repository contains a mermaid script 'workflow-diagram.mmd', which can be used to generate a workflow diagram e.g. on https://mermaid.ai/live/edit

