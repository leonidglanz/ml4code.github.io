---
layout: publication
title: Investigating Next Steps inStatic API-Misuse Detection
authors: Sven Amann, Hoan Anh Nguyen, Sarah Nadi, Tien N. Nguyen, Mira Mezini
conference: MSR
year: 2019
bibkey: amann2019investigating
additional_links:
   - {name: "Paper", url: "http://sven-amann.de/publications/mudetect-msr19.pdf"}
   - {name: "website", url: "http://www.st.informatik.tu-darmstadt.de/artifacts/mudetect/"}
   - {name: "code", url: "https://github.com/stg-tud/StringHound"}
tags: ["api misuse", "constraint mining", "machine learning", "bug detection"]
---
Application Programming Interfaces (APIs) often impose constraints such as call order or preconditions. API mis-uses, i.e., usages violating these constraints, may cause software crashes, data-loss, and vulnerabilities. Researchers developed several approaches to detect API misuses, typically still resulting in low recall and precision. In this work, we investigate ways to improve API-misuse detection. We design MUDETECT, an API-misuse detector that builds on the strengths of existing detectors and tries to mitigate their weaknesses. MUDETECT uses a new graph representation of API usages that captures different types of API misuses and a systematically designed ranking strategy that effectively improves precision. Evaluation shows that MUDETECT identifies real-world API misuses with twice the recall of previous detectors and 2.5x higher precision. It even achieves almost 4x higher precision and recall, when mining patterns across projects, rather than from only the target project.