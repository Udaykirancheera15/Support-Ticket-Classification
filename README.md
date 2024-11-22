# Support Ticket Classification

An AI-based solution to automate the classification of support tickets, reducing manual efforts and enhancing the efficiency of IT and support teams.

## Overview
The **Support Ticket Classification** project leverages text mining and machine learning to classify incoming support tickets. The solution predicts the platform responsible for a submitted ticket and provides a topic classification to diagnose the issue, enabling faster resolutions.

## Features
- **Platform Prediction:** Identifies the responsible team or department.
- **Topic Modeling:** Helps classify tickets by diagnosing the issue.
- **Dashboard Integration:** Provides real-time insights through a Grafana-powered dashboard.
- **Rapid Deployment:** Supports production setups with AI Hub and PostgreSQL.

## Technology Stack
- **Tools:**  ALTAIR AI Studio( Previously RapidMiner Studio)(Operator Toolbox , Text Processing )
- **Database:** PostgreSQL
- **Visualization:** Grafana
- **Languages:** No-code solution using RapidMiner workflows.

## Project Goals
- Automate ticket classification to reduce manual efforts.
- Deliver accurate platform and topic predictions for efficient ticket resolution.
- Achieve at least 90% accuracy to minimize reclassification.

## Data
The dataset was inspired by Stack Overflow posts and consists of support ticket data simulated from topics such as 3D Printing, Android, Apple, Database Administration (DBA), and Unix. The raw dataset is extensive but includes a sampled version for rapid prototyping.

### Example Data Attributes
- **Post Title** and **Body:** Text-based ticket content.
- **Tags:** Classification metadata.
- **TicketType:** Predicted label.
- **Other Features:** View Count, Score, Answer Count, etc.

## Key Processes
1. **Preprocessing:** Cleans and prepares the raw data for modeling.
2. **Text Mining:** Converts unstructured text into structured data using techniques like TF-IDF and n-grams.
3. **Modeling:** Builds classification models using Naïve Bayes for platform prediction.
4. **Topic Modeling:** Utilizes LDA (Latent Dirichlet Allocation) to classify issues into topics.

## Deployment
- **AI Hub Integration:** Deploy workflows as REST APIs.
- **Dashboard:** Visualizes ticket classifications and predictions in Grafana.
- **Database Integration:** Stores and retrieves tickets from a PostgreSQL database.

## Setup Instructions
### Development Setup
1. Install ALTAIR AI Studio( Previously RapidMiner Studio).
2. Add required extensions:
   - **Operator Toolbox **
   - **Text Processing **
3. Load the provided repository in RapidMiner Studio.
4. Use `AllTicketsSample` for development to avoid handling large datasets.

### Production Setup
1. Deploy the processes in the `Deployments` folder to RapidMiner AI Hub.
2. Connect to a PostgreSQL database for data storage and retrieval.
3. Configure Grafana to interact with the deployed web services.

## Dashboard
The dashboard provides:
- **Platform Predictions**
- **Topic Classifications**
- **Recent Ticket Logs**
- **Key Insights into Ticket Trends**

## Next Steps
- Monitor performance with new tickets and retrain models if accuracy drops.
- Expand the LDA model to accommodate new topics.
- Optimize workflows for improved runtime efficiency.

## References
- [RapidMiner Academy](https://academy.rapidminer.com/)
- [Cross-Validation Introduction](https://academy.rapidminer.com/learn/video/cross-validation-introduction)
