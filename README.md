Secure Data Exchange & Database Normalization Project
Author

Hiral Maharjan
BSc Hons Ethical and Cyber Security
Softwarica College of IT & E-commerce

Overview

This project contains two main tasks:

Task 1: Secure Data Exchange

Description:
In modern computing, secure data exchange is critical for emails, cloud services, and APIs. This task focuses on:

Understanding encoding formats: ASCII, Base64, Hexadecimal, and URL encoding

Implementing encryption and secure transmission protocols: TLS, HTTPS, and SMTP over TLS (STARTTLS)

Ensuring integrity and confidentiality of data during transmission

Key Features:

Encoding Formats

ASCII: Simple, lightweight, supports basic English characters

Base64: Encodes binary data into text for safe email transmission

Hexadecimal: Represents binary data as readable text for debugging and cryptography

URL Encoding: Ensures safe web transmission by converting special characters

Secure Protocols

TLS: Encrypts communication between client and server, ensuring privacy and integrity

HTTPS: Combines HTTP with TLS for secure web browsing

SMTP + STARTTLS: Secures email transmission using TLS encryption over SMTP

Real-World Example

An email with attachments is encoded in Base64 and sent via SMTP over a TLS-encrypted channel. The receiver decrypts TLS to access the encoded message safely.

Task 3: Club Membership Table Analysis and Normalization

Description:
The original club membership table combined multiple entities (Students, Clubs, Memberships), causing:

Data redundancy

Duplicate data

Update and deletion anomalies

Database normalization was applied to improve structure and integrity.

Normalization Steps
1NF (First Normal Form)

Eliminated repeating groups and ensured atomic values

2NF (Second Normal Form)

Removed partial dependencies by separating Students, Clubs, and Membership tables

3NF (Third Normal Form)

Removed transitive dependencies by creating a separate Staff table for club mentors and rooms

Benefits

Reduced redundancy and duplication

Improved data accuracy

Easier updates and management

JOIN operations allow combining related data for queries

E-R Diagram

The E-R diagram shows relationships between Students, Clubs, Staff, and Membership tables.

Many-to-Many relationship between Students and Clubs via Membership

SQL Operations Included

Creating tables: Students, Clubs, Staff, Registration

Inserting data into normalized tables

JOIN operations to display combined student and club information

Technologies Used

MySQL (via Docker)

SQL for database operations

Base64, ASCII, Hexadecimal, URL encoding

TLS / HTTPS protocols for secure transmission
