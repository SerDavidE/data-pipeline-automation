# Gans E-Scooter Data Pipeline Project

## Overview

Gans is a nascent e-scooter-sharing system aiming to thrive in major cities globally. Competing against giants like TIER and Bird, Gans plans to carve out its niche not just with its sustainable mobility approach, but by optimizing scooter placement based on real-time user needs.

While many e-scooter firms prioritize the eco-friendliness narrative, Gans believes that its operational success lies in ensuring scooters are strategically placed. Various factors such as city topography, daily commuter patterns, and tourist behavior influence scooter placement.

To systematically address this challenge, Gans endeavors to set up a comprehensive and automated data pipeline in the cloud. This initiative aims to utilize real-time data for predictive modeling, ensuring users always find a scooter when they need one.

## Project Phases

### Phase 1: Local Pipeline

The journey begins with data collection and storage on a local environment.

#### 1.1 Web Scraping

- **Objective**: Extract data from the web.
- **Tools**: Mainly Python's `beautifulsoup` library.
- **Data Sources**: Websites with relevant e-scooter data.

#### 1.2 API Data Collection

- **Objective**: Obtain specific datasets from online providers.
- **Tools**: Python’s `requests` library for API interactions.
- **Data Sources**: External platforms offering data via APIs.

#### 1.3 Database Model Creation

- **Objective**: Establish a logical database structure.
- **Tasks**: Determine necessary tables and their interrelations.
- **Outcome**: A blueprint of the database tailored for Gans's operational needs.

#### 1.4 Local MySQL Data Storage

- **Objective**: Validate the designed database model.
- **Tasks**: Initiate a local MySQL instance and populate with curated data.
- **Outcome**: A database on a local server filled with relevant datasets.

### Phase 2: Cloud Pipeline

Transitioning to the cloud, we aim to leverage its scalability, flexibility, and automation capabilities.

#### 2.1 Cloud Database Setup

- **Objective**: Establish the database in a cloud environment.
- **Tools**: Amazon Web Services' Relational Database Service (RDS) for MySQL setup.
- **Outcome**: A scalable and flexible cloud-hosted database.

#### 2.2 Script Migration to Lambda

- **Objective**: Execute code effortlessly in the cloud.
- **Tools**: AWS Lambda for migrating data collection scripts from Jupyter Notebooks.
- **Outcome**: Cloud-based scripts ready for scheduled execution.

#### 2.3 Pipeline Automation

- **Objective**: Harness cloud capabilities for seamless automation.
- **Tools**: AWS CloudWatch Events / EventBridge for triggering data collection tasks.
- **Outcome**: A fully automated data collection process running on predefined schedules.

---

## Dive Deeper with Medium Articles

Visit individual Medium articles for a deeper dive into each section of this journey: **[The Pulse of Innovation: Unfolding a Seamless Data Pipeline Journey](https://medium.com/@sergio_david/the-pulse-of-innovation-unfolding-a-seamless-data-pipeline-journey-e40e786720c9)**

- **[The Great Data Hunt: Scraping the Web and Unlocking APIs](https://medium.com/@sergio_david/the-great-data-hunt-scraping-the-web-and-unlocking-apis-514251a7e97f)**: The process initiates with data gathering from diverse sources, including APIs and web pages.
- **[From Chaos to Clarity: The Art of Data Cleaning and Transformation](https://medium.com/@sergio_david/from-chaos-to-clarity-the-art-of-data-cleaning-and-transformation-c57920de19cf)**: Raw data undergoes rigorous cleaning and transformation to be rendered usable.
- **[Building Castles in the Cloud: A Guide to Database Design and AWS RDS](https://medium.com/@sergio_david/building-castles-in-the-cloud-a-guide-to-database-design-and-aws-rds-1aabc3ad654d)**: The heart of the system, the relational data model, is implemented in MySQL.
- **[The Automation Orchestra: Scheduling Harmony with AWS Lambda](https://medium.com/@sergio_david/the-automation-orchestra-scheduling-harmony-with-aws-lambda-521d2a55bd5f)**: Automation ensures a seamless, continuous flow of data.
- **[Navigating the Maze: Reflections and Wisdom from a Data Pipeline Odyssey](https://medium.com/@sergio_david/navigating-the-maze-reflections-and-wisdom-from-a-data-pipeline-odyssey-94dd38ab94c1)**: Insights into the intricacies and learnings from the project.

---

## License

[MIT License](LICENSE)
