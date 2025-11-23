# Customer-Support-Ticket-Analyzer
The Customer Support Ticket Analyzer is a Python-based application built to automate the classification and extraction of crucial information from customer support tickets.
Customer Support Ticket Analyzer
The Customer Support Ticket Analyzer is an intelligent machine learning application designed to automatically process and categorize customer support tickets while extracting valuable information. This system leverages natural language processing (NLP) techniques and classification models to streamline ticket management and improve support efficiency.​

Working Process
The analyzer operates through a systematic pipeline beginning with data loading and preprocessing. It reads support ticket data containing text descriptions, issue types, urgency levels, and product information. The raw text undergoes rigorous cleaning—converting to lowercase, removing special characters, tokenizing into individual words, eliminating common stopwords, and applying lemmatization to normalize word variations. This cleaned text is then transformed into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization, converting 5,000 key features into a machine-readable format.​

Core Functionality
The system employs dual Logistic Regression models trained separately for two critical classifications. The first model predicts the issue type (such as technical problems, billing inquiries, or product defects), while the second determines the urgency level (categorizing tickets as critical, high, medium, or low priority). This dual-classification approach enables support teams to prioritize responses effectively.​

Beyond classification, the analyzer incorporates entity extraction to identify important information within tickets. It detects product mentions, extracts temporal references (dates), and recognizes complaint-related keywords like "broken," "error," or "delayed." These extracted entities provide actionable insights for faster issue resolution.​

User Interface
The system features a Gradio-based web interface offering an intuitive user experience. Support agents simply input customer ticket text, and the analyzer instantly returns three outputs: the predicted issue category, urgency classification, and a structured JSON object containing extracted entities (products, dates, complaint keywords). This real-time analysis capability eliminates manual ticket sorting, reduces response time, and ensures consistent categorization across all support interactions, ultimately enhancing customer satisfaction and operational efficiency.​

only the file having on it

Customer Support Ticket Analyzer: Working and Functionality
The Customer Support Ticket Analyzer is a Python-based application built to automate the classification and extraction of crucial information from customer support tickets. The system utilizes several natural language processing (NLP) and machine learning tools to streamline the handling of support requests.

The process starts with text preprocessing. The raw messages from support tickets are converted to lowercase, stripped of special characters, tokenized, and reduced to their linguistic roots through lemmatization. Common English stopwords are removed to highlight only relevant information. This cleaned text is then vectorized using the TF-IDF (Term Frequency-Inverse Document Frequency) method, turning it into numerical features suitable for machine learning models.

The analyzer uses logistic regression classifiers to perform two main tasks:

Issue Type Classification: The first model predicts the category of the ticket, such as technical issues or billing queries.

Urgency Level Detection: The second model assigns a priority level (e.g., critical, high, medium, low) to each ticket, helping support teams manage workflow.

A key feature is the entity extraction module. This component scans ticket content for specific entities:

Product mentions (using a product list from the dataset)

Date references

Complaint keywords (such as "broken," "error," or "delayed")

The extracted entities are bundled into a structured JSON-like object for further processing and display.

The application provides a Gradio-powered web interface where users can input ticket text and instantly receive predicted issue categories, urgency levels, and extracted entities. This end-to-end solution reduces manual ticket handling, ensures consistent prioritization, and accelerates resolution—all directly within one easy-to-use interface, as described and implemented in the source file.
