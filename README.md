# OSINT: Open Source Intelligence

Open source intelligence is not internet searching with better tools. It is a disciplined methodology - a complete cycle from requirements through collection, processing, analysis, and dissemination - that transforms publicly available information into actionable intelligence. This book covers that full cycle across 30 chapters: from the legal and ethical foundations that bound all professional OSINT practice, through advanced technical collection techniques, specialized domain applications, operational tradecraft, and multi-intelligence fusion with HUMINT, SIGINT, and GEOINT.

The book is built for practitioners. Every chapter addresses the actual work - what to collect, how to collect it, how to validate it, how to protect yourself while doing it, and how to turn it into something a decision-maker can use.

---

## Who This Is For

**Primary:** Security analysts, intelligence professionals, and detection engineers who conduct open source research as part of their operational responsibilities and need a systematic, end-to-end framework for professional OSINT practice.

**Secondary:** Investigators, researchers, and technical practitioners from adjacent fields - cybersecurity, journalism, law enforcement support, competitive intelligence - who need rigorous methodology, not just tools.

---

## What You Will Learn

- The intelligence cycle and where OSINT fits within the broader intelligence community alongside HUMINT, SIGINT, GEOINT, and MASINT
- Technical collection techniques: protocol analysis, TLS certificate intelligence, email header forensics, P2P network analysis, infrastructure reconnaissance, and network flow analysis
- Automation and scale: building systematic collection pipelines with appropriate rate limiting, error handling, and data quality controls
- Specialized domain applications: financial intelligence, cyber threat intelligence, business intelligence, academic research, and media analysis
- Operational tradecraft: collection management, OPSEC, digital footprint minimization, source diversification, and counterintelligence awareness
- Advanced integration: fusing OSINT with HUMINT, SIGINT, and GEOINT through structured analytical techniques and information sharing protocols
- Legal and ethical frameworks across jurisdictions, with practical guidance on privacy law compliance, data protection, and professional conduct standards

---

## Table of Contents

The book is in `book/`: an index per chapter (`chapter_NN_index.yaml`) and one YAML file per section (`section_NN_MM_<topic>.yaml`), with the book index (`osint_book_index.yaml`) and an overview of every chapter (`osint_book_overview.yaml`). Appendices A-D are chapters 31-34.

### Part 1 - Fundamentals
- [Chapter 1: Foundations of OSINT](book/chapter_01_index.yaml)
- [Chapter 2: Information Theory and Data Analysis](book/chapter_02_index.yaml)
- [Chapter 3: Network Fundamentals](book/chapter_03_index.yaml)
- [Chapter 4: Data Structures and Formats](book/chapter_04_index.yaml)
- [Chapter 5: Web Technologies](book/chapter_05_index.yaml)
- [Chapter 6: Search Methodologies](book/chapter_06_index.yaml)

### Part 2 - Advanced Techniques
- [Chapter 7: Protocol Analysis and Traffic Inspection](book/chapter_07_index.yaml)
- [Chapter 8: Cryptographic Intelligence](book/chapter_08_index.yaml)
- [Chapter 9: Advanced Data Mining](book/chapter_09_index.yaml)
- [Chapter 10: Infrastructure Reconnaissance](book/chapter_10_index.yaml)
- [Chapter 11: Advanced Social Engineering Analysis](book/chapter_11_index.yaml)
- [Chapter 12: Geospatial Intelligence](book/chapter_12_index.yaml)
- [Chapter 13: Temporal Analysis](book/chapter_13_index.yaml)
- [Chapter 14: Communication Pattern Analysis](book/chapter_14_index.yaml)

### Part 3 - Specialized OSINT Domains
- [Chapter 15: Automation and Systematic Collection](book/chapter_15_index.yaml)
- [Chapter 16: Financial Intelligence](book/chapter_16_index.yaml)
- [Chapter 17: Cyber Threat Intelligence](book/chapter_17_index.yaml)
- [Chapter 18: Business Intelligence](book/chapter_18_index.yaml)
- [Chapter 19: Academic and Research Intelligence](book/chapter_19_index.yaml)
- [Chapter 20: Media and Information Analysis](book/chapter_20_index.yaml)

### Part 4 - Operational Considerations
- [Chapter 21: Collection Management](book/chapter_21_index.yaml)
- [Chapter 22: Analysis Frameworks](book/chapter_22_index.yaml)
- [Chapter 23: Counterintelligence Awareness](book/chapter_23_index.yaml)
- [Chapter 24: Technical Operations](book/chapter_24_index.yaml)
- [Chapter 25: Legal and Ethical Frameworks](book/chapter_25_index.yaml)

### Part 5 - Advanced Integration
- [Chapter 26: Multi-Intelligence Fusion](book/chapter_26_index.yaml)
- [Chapter 27: Artificial Intelligence Integration](book/chapter_27_index.yaml)
- [Chapter 28: Emerging Technologies](book/chapter_28_index.yaml)
- [Chapter 29: Scalability and Performance](book/chapter_29_index.yaml)
- [Chapter 30: Quality Assurance and Tradecraft Standards](book/chapter_30_index.yaml)

### Appendices
- [A: Technical Reference](book/chapter_31_index.yaml)
- [B: Legal and Ethical Guidelines](book/chapter_32_index.yaml)
- [C: Mathematical and Statistical Reference](book/chapter_33_index.yaml)
- [D: Protocol and Standards Reference](book/chapter_34_index.yaml)

---

## How to Read This Book

**Sequential path:** Start with Part 1 for the foundational concepts - the intelligence cycle, legal frameworks, and technical vocabulary - that every subsequent chapter assumes. Move through Part 2 for technical collection skills, Part 3 for domain specialization, and Part 4 for operational tradecraft. Part 5 and the appendices are reference material for practitioners already working at advanced integration levels.

**Reference path:** Jump to the chapter that matches your immediate requirement. Each chapter is self-contained with its own methodology and procedural guidance. Use the appendices for quick technical lookups - port numbers, HTTP status codes, DNS record types, file signatures, regex patterns, and protocol header structures.

**Domain path:** If your work is primarily in a specific area, the Part 3 chapters (15–20) cover financial, cyber threat, business, academic, and media intelligence as standalone domains. Each references back to the foundational collection and analytical techniques in Parts 1 and 2.

---

## License

Prose content: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  
Code examples: [MIT](LICENSE)

---

## Author

**Raghav Dinesh** | [github.com/ruwgxo](https://github.com/ruwgxo)

Security architect with experience building production security systems since 2012. *OSINT: Open Source Intelligence* draws on professional intelligence tradecraft, publicly documented methodologies from the intelligence community, and practical experience applying open source collection and analysis at enterprise scale.
