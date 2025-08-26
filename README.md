# Wiland Internship Projects – Summer 2025

This repository contains a summary and select code examples from my **Software Engineering Internship at Wiland (June–August 2025)**. My work focused on backend development, data movement pipelines, API endpoint design, and cross-functional collaboration in a production Agile environment.

---

## Projects

### 1. Mart Replication QC Script Modernization (Python)
- **Converted legacy code** from Python 3.11 to 3.9 to ensure compatibility with production environments  
- Refactored functions (`match`, `dataclass`, etc.), replaced `fetchmany()` with `fetchall()` to resolve data truncation issues  
- Verified outputs using SQL (test vs. backup tables) and ensured clean merge requests via Git

---

### 2. Tableau Hyper File Generator (Python + C++)
- Updated C++ tool to support `.hyper` file format (Tableau API) instead of deprecated `.tde` format  
- Wrote a Python wrapper script (`write_hyper.py`) to convert SQL query output → CSV → `.hyper` file  
- Integrated CLI parameter parsing, output type validation, and error handling logic  
- Collaborated with internal teams to test file output, manage deployments, and validate data formatting

---

### 3. Generic DataMover Wrapper for MariaDB → HDFS (Python + Spark + Scala)
- Built a flexible command-line wrapper script to automate DataMover job generation using manifest templates  
- Parsed and validated parameters (server ID, table name, HDFS path, partition columns, memory settings)  
- Used Spark and HDFS to test data movement across clusters, handling both base tables and views  
- Added partition detection and fallbacks (ComputePredicates vs. Auto), incorporating primary key checks and dynamic overrides  
- Wrote documentation and validated manifests across multiple QA environments

---

### 4. Calculator SQL Metadata & Endpoint Refactoring (TypeScript + SQL)
- Worked on both the simple and complex version fixes for updating dynamic calculator endpoint logic in the `mxctlapi` backend  
- Modified TypeScript files (`PostCalculationWorker.ts`, `GetCalculationWorker.ts`) to update endpoint routing and SQL behavior  
- Implemented recursive SQL insert logic to support aggregation input templates  
- Verified SQL queries and Protobuf schema changes using a local SOA test server and gRPC-style API calls

---

## Tools & Technologies Used
- **Languages:** Python, TypeScript, SQL, C++, Scala  
- **Tools/Frameworks:** Git, JIRA, Bash, Vim, REST APIs, Protobuf, Tableau Hyper API  
- **Systems:** Linux, MariaDB, HDFS, Spark, Kubernetes, Agile/Scrum, SOA (Service-Oriented Architecture)

---

## Collaboration & Workflow
Throughout the internship, I:
- Worked closely with engineers and product owners across data, platform, and QA teams  
- Participated in daily standups, sprint planning, and code reviews  
- Prioritized clean, testable code and detailed documentation to support long-term maintainability  

---

_Code, internal scripts, and specific details have been redacted to protect proprietary data and infrastructure._
