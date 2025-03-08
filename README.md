# STREAMLINING REAL ESTATE WITH CREWAI AND GROQ
The retail property analysis system developed in this project demonstrates the application of autonomous AI agents to identify promising investment opportunities. By integrating real-time web search capabilities via SerperDevTool and advanced natural language processing with Groq’s Mixtral model, the system delivers comprehensive market insights and financial projections. While the system excels in synthesizing complex data, ongoing improvements aim to enhance real-time data integration and scalability.

## METHODOLOGY

This project utilizes a simulated real estate dataset and web-sourced data (via SerperDevTool) due to limited access to proprietary real estate databases. The methodology focuses on two key agents:

1. **Senior Retail Property Investment Analyst**:
   - Identifies top retail investment locations (e.g., 5 areas in Khammam, Telangana).
   - Analyzes foot traffic, accessibility, market trends, and ROI potential.
   - Combines quantitative metrics (e.g., rental yields, cap rates) with qualitative insights (e.g., emerging corridors).

2. **Senior Investment Property Research Analyst**:
   - Synthesizes research into concise, investor-focused reports.
   - Performs financial modeling (ROI, cash flow) and risk assessment.

Key features analyzed include:
- Location demographics
- Rental yields and vacancy rates
- Property appreciation potential
- Market competition and e-commerce impact

Irrelevant or redundant data is filtered out to optimize agent performance and report clarity.

## PROPOSED IMPLEMENTATION
![image](https://github.com/user-attachments/assets/d6bc3008-548d-413f-b981-7393d7ce32fb)

**Instructions to Follow for Proposed Implementation:**

- **Agent Collaboration**: Ensure the `property_researcher` and `property_analyst` agents work sequentially—research data must be fully collected and written to output files before analysis begins.
- **Tool Integration**: Configure the `SerperDevTool` with a valid API key in `tools.py` to enable real-time web searches; test with sample queries to verify data retrieval accuracy.
- **Output Formatting**: Standardize report formats in `tasks.py`—use structured text (e.g., bullet points, headers) for readability and ensure all output files are saved in the `output/` directory.
- **Scalability**: Design the system to handle multiple markets by parameterizing the `research_task` description (e.g., replace "Khammam" with a variable for dynamic location input).
- **Error Handling**: Implement try-catch blocks in `crew.py` to manage API timeouts or data retrieval failures, ensuring the crew process continues gracefully.

## SAMPLE OUTPUT

Here’s an example of the expected output from the `internet_property_researcher_output.txt` file:
![image](https://github.com/user-attachments/assets/f15f9162-5b3e-4b4b-a3e8-077b22108685)

![image](https://github.com/user-attachments/assets/76314394-3c0c-4818-9281-08d59489b230)

OUTPUT: specifically represents key features mentioned above with repect to specified location or region Real Estate evluation
Given location- Khammam city, Telangana state, India country
These summarized reports are saved in same directory automatically.

![image](https://github.com/user-attachments/assets/5fef2723-3e67-4615-803f-3d84e1e9142a)

![image](https://github.com/user-attachments/assets/6c653dbe-375b-4f9d-81b7-d177aa55d445)

![image](https://github.com/user-attachments/assets/eeed8e42-4909-41c8-81bc-fe3b8baf5e80)












