# Plagiarism-Detector

# Architecture Design

The architecture design for the Simple Plagiarism Detection Utility can be divided into four major components:

Document Collection: This component includes classes and interfaces that handle the collection of existing documents and the potentially plagiarized document. It will include classes for storing and managing the documents, such as DocumentCollection and Document classes.

String Matching Algorithms: This component includes classes that implement different string matching algorithms such as Brute Force with Hamming Distance, Rabin-Karp Algorithm, KMP Algorithm, and Boyer-Moore Algorithm.

Plagiarism Detector: This component includes the main classes and interfaces that run the plagiarism detection process. It includes classes that take in the input, perform string matching using different algorithms, and output the set of documents from which the document was plagiarized.

Performance Comparison: This component includes classes and interfaces for comparing the performance of different string matching algorithms used in the plagiarism detection process.

# UML Diagram

Below is the UML diagram that shows the relationships between the different classes and interfaces in the architecture design:

python
Copy code
+-----------------+        +-----------------+          +-----------------+          +-------------------+
| Document        |        | DocumentReader  |          | StringMatcher   |          | PerformanceTester|
+-----------------+        +-----------------+          +-----------------+          +-------------------+
| -id: int        |        | -filename: str  |          | -algorithm: str |          | -algorithm: str   |
| -text: str      |        |                 |          |                 |          | -documents: list  |
+-----------------+        +-----------------+          |                 |          |                   |
| +getId(): int   |        | +read(): str     |          | +match(): list  |          | +test(): dict     |
| +getText(): str |------->|                 |--------->|                 |          |                   |
+-----------------+        |                 |          |                 |          |                   |
                           |                 |          |                 |--------->|                   |
                           +-----------------+          +-----------------+          +-------------------+
# Development Workflow

The development workflow for the Simple Plagiarism Detection Utility can be divided into several steps:

Requirements Gathering: Gather the requirements and specifications of the project from the client or stakeholders.

Architecture Design: Based on the requirements, design the architecture of the project, including the UML diagram and class/interface specifications.

Implementation: Implement the different classes and interfaces according to the design specifications.

Integration: Integrate the different components and classes to form a functional system.

Testing: Test the system for functionality, performance, and accuracy. Use the PerformanceTester class to compare the performance of different string matching algorithms.

Deployment: Deploy the system to the client or stakeholders and provide necessary support.

Maintenance: Provide maintenance and support for the system as required.



