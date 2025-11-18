# Customer Risk Profiling & Adverse Media Screening

## Overview
A comprehensive customer risk assessment engine that combines structured data analysis with NLP-based adverse media screening. It calculates dynamic risk scores and continuously monitors news sources for negative mentions related to financial crime.

## Key Features
- **Risk Scoring Engine**: Configurable scoring based on occupation, geography, and transaction patterns.
- **Adverse Media Screening**: NLP-based Named Entity Recognition (NER) and sentiment analysis on news articles.
- **Sanctions & PEP Screening**: Automated checking against global sanctions lists.
- **Knowledge Graph**: Neo4j integration for mapping complex entity relationships.

## Project Structure
- `src/risk_engine/`: Logic for calculating customer risk scores.
- `src/media_screening/`: Scrapers and NLP models for news analysis.
- `src/screening/`: Modules for sanctions and PEP list matching.
- `dashboards/`: Plotly Dash visualization for risk reporting.

## Getting Started

### Prerequisites
- Python 3.10+
- Neo4j Database (optional for graph features)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/SamanthaZhang25/customer-risk-profiling.git
   cd customer-risk-profiling
   ```
2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. **Run Screening**: Execute the screening pipeline.
   ```bash
   python src/main.py --mode screening
   ```
2. **View Dashboard**: Start the risk dashboard.
   ```bash
   python dashboards/app.py
   ```
