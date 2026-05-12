# AI Shopping Agent: Multi-Agent E-commerce Deal Finder

This project is an AI-powered shopping agent that helps users find the best product deals across multiple e-commerce websites in Egypt (such as Amazon.eg, Jumia, and Noon). It uses a crew of specialized agents to generate targeted search queries, collect product pages, scrape product details, and build a professional HTML procurement report using Bootstrap. [file:1]

## Features

- Generates specific product search queries optimized for e-commerce product pages, not blogs or generic listings. [file:1]  
- Searches multiple websites for product links and filters out low-relevance or spammy results based on a score threshold. [file:1]  
- Scrapes product pages to extract title, price, discount, image URL, and key specifications. [file:1]  
- Ranks products and provides recommendation notes to support procurement decisions. [file:1]  
- Creates a structured HTML procurement report (with Bootstrap) including: executive summary, methodology, findings, analysis, recommendations, and conclusion. [file:1]  
- Simple Gradio interface where the user enters a product name and gets aggregated results. [file:1]

## Tech Stack

- Python (Jupyter/Colab notebook) [file:1]  
- CrewAI for multi-agent orchestration (planner, search agent, search-engine agent, scraper, report generator, procurement report author) [file:1]  
- Tavily search client for web search tool integration [file:1]  
- ScrapeGraph / web scraping client for structured product extraction [file:1]  
- Bootstrap for the final HTML report UI [file:1]  
- Gradio for a simple web interface to run the agent workflow. [file:1]

## How It Works

1. **Search query generation**  
   A Search Query Generator agent creates several specific queries (including brands like Samsung, Apple, Lenovo) tailored to buy a given product (e.g., Tablet) in Egypt. [file:1]

2. **Search engine agent**  
   A Search Engine Agent calls a Tavily-based search tool to get product links only, discarding blogs and non-product pages, and keeps only results above a given relevance score. [file:1]

3. **Web scraping agent**  
   A Scraper Agent uses a smart scraping tool to extract structured product data (title, URLs, prices, specs) from each product page. [file:1]

4. **Procurement report author**  
   A Procurement Report Author Agent and Report Generator Agent take all extracted products and generate a detailed HTML procurement report with Bootstrap styling. [file:1]

5. **User interface**  
   A Gradio app wraps the whole pipeline so the user can type a product name and receive summarized, ranked results and reports. [file:1]

## Use Cases

- Internal procurement teams comparing prices across multiple online stores. [file:1]  
- Market research for specific product categories (e.g., tablets, electronics). [file:1]  
- Educational demo of multi-agent AI workflows for search, scraping, and reporting. [file:1]

## Future Improvements

- Support more countries and e-commerce websites. [file:1]  
- Add dashboards and charts directly into the HTML report. [file:1]  
- Integrate more LLM models and smarter ranking logic. [file:1]
