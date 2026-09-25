# Changelog – AI-Powered Packaging Chatbot

## Week 3 – Initial Version

### Added

* Created the basic AI-powered packaging chatbot using Python.
* Added a packaging knowledge base with common customer questions and answers.
* Added TF-IDF for converting customer questions into numerical vectors.
* Added Cosine Similarity for finding the most relevant question.
* Added a similarity threshold for better answer matching.
* Added fallback responses for unknown or unrelated questions.
* Added input validation for empty customer messages.
* Added a quote request feature for collecting packaging requirements.
* Added fields for product type, dimensions, quantity, material, printing, finishing and delivery city.
* Added conversation logging for customer questions and chatbot responses.
* Added JSON files for storing project data.
* Tested the chatbot with normal, unknown, empty and differently worded questions.

### Fixed

* Improved handling of questions that do not match the knowledge base.
* Added better handling for empty input.
* Improved matching when customers ask the same question using different words.
* Reduced the chance of returning unrelated answers by using a similarity threshold.

### Tested

The chatbot was tested with questions about packaging products, materials, MOQ, customization, printing, samples, production time, delivery and quotations. It was also tested with empty input, unrelated questions, numbers, punctuation and different question wording.

### Future Updates

Possible future improvements include a web-based interface, a larger knowledge base, multilingual support, automatic quotation calculation, live database integration, CRM integration and human-agent support.
