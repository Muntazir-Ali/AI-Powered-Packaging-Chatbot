# Project Report – AI-Powered Packaging Chatbot

## 1. Introduction

For my Week 3 project, I developed an AI-Powered Packaging Chatbot for a fictional emerging packaging company called PackPro Solutions. The main purpose of this project was to create a simple chatbot that can answer common customer questions related to packaging products and services. The chatbot provides information about packaging materials, custom boxes, minimum order quantity, printing, samples, production time, delivery and quotations. I developed and tested the project using Python in Google Colab.

## 2. Project Objective

The main objective of this project was to build a simple customer-support chatbot that can understand different customer questions and provide relevant answers from a predefined knowledge base. I also wanted to add some practical features such as fallback responses, quotation information collection and conversation logging.

## 3. Company Background

PackPro Solutions is a fictional packaging company created for this project. The company provides customized packaging solutions for businesses, startups, retailers and e-commerce brands. The chatbot is designed to answer basic questions about products such as custom boxes, mailer boxes, gift boxes, food packaging, kraft packaging and other customized packaging solutions.

## 4. Technologies Used

The main programming language used in this project is Python. Google Colab was used as the development and testing environment. Scikit-learn was used for TF-IDF vectorization and Cosine Similarity. JSON files were used to store the knowledge base, quotation requests and conversation logs. Pandas was also used where needed for working with data.

## 5. Knowledge Base

A packaging-related knowledge base was created and stored in `packaging_knowledge.json`. It contains common questions and answers related to PackPro Solutions. The questions cover topics such as available products, materials, customization, printing, MOQ, samples, production time, delivery and quotations. This knowledge base gives the chatbot the information it needs to answer customer questions.

## 6. How the Chatbot Works

When a customer enters a question, the chatbot first checks the input and then compares the question with the questions stored in the knowledge base. TF-IDF is used to convert the text into numerical vectors, and Cosine Similarity is used to find how closely the customer's question matches the stored questions. The chatbot then selects the most relevant answer. A similarity threshold is also used so that the chatbot does not provide an unrelated answer when the customer's question is not close enough to the available information.

## 7. Main Features

The chatbot includes several useful features. It can answer common packaging questions, handle different ways of asking similar questions, provide fallback responses for unknown questions and collect information for quotation requests. The quote feature collects details such as product type, dimensions, quantity, material, printing requirements, finishing and delivery city. Conversation logging is also included so that customer questions and chatbot responses can be saved for later use.

## 8. Quote Request Feature

The quotation feature was added to make the chatbot more practical. When a customer enters `quote`, the chatbot can collect the basic information needed for a packaging quotation. This includes the type of product, dimensions, quantity, material, printing, finishing and delivery location. The collected information can be stored in `quote_requests.json` and could be used for further processing in a future version.

## 9. Conversation Logging

A conversation logging feature was also added to the project. Customer questions and chatbot responses can be saved in `conversation_log.json`. This feature can be useful for keeping a record of conversations and could later be connected to a proper customer-support or CRM system.

## 10. Testing

I tested the chatbot with different types of customer questions to check how it responds. Some examples included questions about MOQ, packaging materials, custom boxes, logo printing, samples, production time and delivery. I also tested empty input, unrelated questions, numerical input, punctuation and different wording of similar questions. These tests helped identify areas where input validation and fallback handling were needed.

## 11. Problems and Solutions

During testing, I found that an unrelated question could sometimes be matched with a question from the knowledge base. To handle this problem, I added a similarity threshold so that the chatbot gives a fallback response when the match is not strong enough. Another problem was empty input, which was handled by adding input validation. I also needed the chatbot to understand that customers can ask the same question in different ways, so TF-IDF and Cosine Similarity were used instead of simple exact text matching.

## 12. Project Structure

The main project files include `AI_Packaging_Chatbot_Week3.ipynb`, `packaging_knowledge.json`, `quote_requests.json`, `conversation_log.json`, `README.md`, `PROJECT_REPORT.md` and `CHANGELOG.md`. The notebook contains the main Python code, while the JSON files are used for storing project data.

## 13. Limitations

The current chatbot is a basic prototype and has some limitations. It uses a predefined knowledge base and does not connect to a real company database. It does not provide live inventory information or automatically calculate final production prices. Its understanding is also mainly based on text similarity, so very different or complex questions may not always receive the correct response.

## 14. Future Improvements

In the future, this project could be improved by adding a proper web-based chatbot interface, a larger knowledge base, better natural-language understanding and multilingual support. Other possible improvements include automatic quotation calculation, live database integration, CRM integration, analytics and a human-agent handoff feature. The chatbot could also be deployed online so customers could use it directly from a company website.

## 15. Learning Outcomes

This project helped me understand how a simple domain-specific chatbot can be developed using Python. I learned how to create and use a knowledge base, process customer questions, use TF-IDF and Cosine Similarity, add fallback handling, collect quotation information and test a chatbot with different types of input. I also learned how different project files can work together to create a complete application.

## 16. Difference From Previous Projects

This Week 3 project is different from my previous internship projects. My Week 1 project focused on AI sales forecasting for a logistics startup, while my Week 2 project focused on an AI-assisted website quality auditor for accounting websites. In Week 3, I worked on conversational AI and customer support by creating a packaging chatbot that retrieves relevant information from a knowledge base.

## 17. Conclusion

The AI-Powered Packaging Chatbot is a simple working prototype that demonstrates how basic AI and Python techniques can be used to create a customer-support system. The project combines a packaging knowledge base, TF-IDF, Cosine Similarity, fallback handling, quotation collection and conversation logging. Although the current version is limited, it provides a good starting point for developing a more advanced packaging customer-support chatbot in the future.

## Project Information

Project: AI-Powered Packaging Chatbot | Company: PackPro Solutions | Week: 3 | Programming Language: Python | Development Environment: Google Colab
