# CECS-399-Section-001-Transdisciplinary-Capstone
Senior AI capstone

2. Collect Documents
• Government / NGO Reports:
o U.S. CRS Reports (PDFs with metadata).
o World Bank Open Knowledge Repository.
• News Articles:
o BBC News Archive on Kaggle.
o Use a news API (e.g., NewsAPI.org) to fetch ~200 recent articles.
• Research Articles:
o arXiv (export abstracts + PDFs).
o PubMed Central.
• Books / Literature:
o Project Gutenberg for plain text. (over 75,000 ebooks)
*Pick ONE domain for consistency (e.g., “US CRS Reports” corpus).
3. Convert to Text
• PDF/DOCX → text: use tools like pdfminer, PyMuPDF, or docx2txt.
• HTML → text: strip tags with BeautifulSoup.
• Scanned PDFs → text: run OCR with Tesseract.
• Save outputs in /text/ as doc001.txt, doc002.txt, etc.
5. Extract Metadata
For each document, record:
• doc_id
• title
• author(s)
• publication_date
• source_url
• file_format
Save this in a CSV or JSON (e.g., corpus_metadata.csv).
6. Clean & Normalize
• Basic cleaning: remove headers/footers, strange characters.
• Optionally, sentence segmentation (spaCy, NLTK).
7. Enable Search & Retrieval
• Index documents for fast keyword and semantic search.
• Support queries like “find all reports mentioning XXXX between 2005–2010.”
• Link related documents together (citations, references, similar content).
8. Discover Insights & Relationships
• Identify intra-document links (e.g., section references).
• Identify inter-document relationships (e.g., one report citing another, entities appearing
across many documents).
9. Summarization & Visualization
• Produce concise summaries of documents.
• Visualize entities, trends, and relationships.
Abstract
This project aims to design and implement a document processing pipeline to automatically
extract key insights, metadata, and inter- and intra-document relationships2. Leveraging natural
language processing (NLP) techniques and data science workflows, the project will parse a
collection of documents, extract structured metadata (such as title, author, date, entities), and
uncover semantic relationships 3 both within documents (intra-document) and across documents
(inter-document). The outcome will be a prototype system capable of summarizing content,
visualizing entity relationships, and providing a searchable knowledge graph. This project is
scoped for a 15 week timeline suitable for undergraduate data science coursework, emphasizing
applied NLP, data wrangling, and visualization.
Proposed Timeline (2 Months)
Week 1–2: Research & Planning
• Define scope and dataset (academic papers, reports, or open-source document sets).
• Literature review on document processing & relationship extraction.
• Identify tools & libraries (e.g., Python, spaCy, NLTK, Hugging Face Transformers,
NetworkX, Pandas, Neo4j optional).
• Draft project plan and success criteria.
Week 3–4: Implementation Phase 1 (Core Extraction)
• Preprocessing: text cleaning, OCR (if needed), tokenization.
• Metadata extraction: titles, authors, dates, keywords.
• Key insights extraction: summaries (using extractive or abstractive summarization).
• Entity recognition: people, places, organizations.
Week 5–6: Implementation Phase 2 (Relationships & Insights)
• Intra-document relationships: co-occurrence of entities, topic modeling.
• Inter-document relationships: cross-referencing entities across documents.
2 An intra-document relationship refers to the connection or links between different components, sections,
or elements within the same document.
3 A semantic relationship is a connection between words, phrases, or concepts based on their meanings.
• Build a simple knowledge graph or relational visualization.
• Develop evaluation metrics (precision/recall for entity extraction, quality of summaries).
Week 7: Integration & Visualization
• Combine metadata, summaries, and relationships into a unified pipeline.
• Build a simple dashboard/visualization (e.g., interactive graphs or search).
• Document results and challenges.
Week 8: Finalization & Reporting
• Testing and validation of the pipeline on the dataset.
• Prepare final report and presentation (including technical approach, results, limitations,
and future work).
• Wrap-up and submission.
Typical Project Components
• Dataset selection: (Open-source articles, PDF reports, Wikipedia dumps, etc.)
• Tools: Python, PDF file format reader library (PdfReader), NLP libraries, Visualization
libraries (Matplotlib, Plotly, D3.js, or Gephi)
• Deliverables: code, documentation, final report, and a short presentation/demo.
• Challenges expected: noisy text, evaluation of summaries, ensuring meaningful
relationship extraction within the scope of the project.
