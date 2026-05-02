# CIND110 — Data Organization for Data Analysts
**Toronto Metropolitan University** · Winter 2025

> Covers the design, management, and querying of structured data systems—from relational databases to hierarchical formats and NLP-driven text analytics pipelines.

---

## 🛠 Skills & Tools
**Database Management:** MySQL, MySQL Workbench, MongoDB, BaseX  
**Languages & Querying:** SQL (Advanced Joins & Aggregates), XQuery/XPath, Python (NLTK, Scikit-learn)  
**Data Formats:** Relational (SQL), Hierarchical (XML), Document-oriented (JSON), Unstructured Text  
**Techniques:** Schema Validation, Referential Integrity, NLP Preprocessing, Cosine Similarity, Data Privacy Auditing

---

## 📂 Featured Projects

---

### [Assignment 2: Multi-Format Data Pipeline (XML, JSON & NLP)](./CIND110/Assignment_2/)
![Individual](https://img.shields.io/badge/type-Individual-1565c0)

**Overview:** Designed and implemented an end-to-end data pipeline serving three distinct business teams — inventory operations, web development, and research analytics — using a self-constructed botanical dataset as the foundation. The pipeline spanned three data paradigms: hierarchical XML storage, document-based JSON modeling, and NLP-driven text mining.

Built and queried a structured XML database in BaseX using XPath/XQuery to answer operational reporting questions such as seasonal stock availability and unstocked inventory. Migrated the schema to JSON and re-implemented equivalent queries in MongoDB, making explicit design decisions around embedding vs. referencing to optimize for the web team's read patterns. Developed a Python IR pipeline in Jupyter that extracted family descriptions, applied text preprocessing (stopword removal, lemmatization), constructed unigram and bigram term-document matrices, and used cosine similarity to surface relationships between plant families. Deliverables included a formal technical brief for each team justifying design decisions, a data privacy audit of customer fields, and a written self-assessment critiquing the pipeline's real-world limitations and ethical considerations.

**Tech stack:** XML/XQuery (BaseX), JSON, MongoDB, Python (NLTK, Scikit-learn), Jupyter Notebook

**Key result:** Delivered a unified multi-format data system with parity across XML and JSON query outputs, and identified the most botanically similar plant families using cosine similarity scoring.

---

### [Assignment 1: Relational Database Engineering (FlowerDB)](./CIND110/Assignment_1/)
![Individual](https://img.shields.io/badge/type-Individual-1565c0)

**Overview:** Acted as a data analyst on a cloud migration team for a scaling floral distribution company, transitioning operations from fragmented spreadsheets to a centralized relational database. The work spanned three phases: schema validation, SQL-driven business intelligence, and strategic retrospective.

Reverse-engineered the existing FlowerDB schema in MySQL Workbench to produce a logical data model, verified referential integrity across six interrelated tables (Flowers, Families, Shops, Customers, Orders, Inventory), and documented how foreign key constraints prevent phantom data entries during rapid scaling. Developed and executed seven optimized SQL queries addressing real operational questions — including multi-location customer loyalty, inventory gap detection, and family-level stock aggregation — then translated each result into plain-language recommendations for non-technical stakeholders. Concluded with a formal strategic retrospective connecting query findings to the company's national expansion decisions.

**Tech stack:** MySQL, MySQL Workbench, SQL (joins, aggregates, subqueries, HAVING clauses)

**Key result:** Produced an end-to-end business intelligence report identifying high-value inventory and customer patterns, with actionable schema improvement recommendations for enterprise scalability.

---

## ⚠️ Limitations & Future Work

- Both assignments use fictional datasets (FlowerDB / botanical consortium) designed to simulate business relationships — findings are illustrative rather than drawn from production data.
- The IR pipeline's similarity results are sensitive to the corpus size; with only ~10 plant family descriptions, bigram analysis has limited discriminatory power.
- Future work could extend the relational schema with time-series sales data to support demand forecasting alongside the existing inventory queries.

---

## 🤝 Contributing & License

Suggestions and feedback welcome — open an issue or pull request.

Licensed under the [MIT License](LICENSE).
