# Information Retrieval

## 1. Introduction

### 1.1 The task of IR (information retrieval)

find documents that are 'relevant' to a user query.

- Given: a large, static document collection
- Given: an information need (keyword-based query)
- Task: find all and only documents relevant to query

### 1.2 Issues in IR

- formulate a query: `keyword`, `natural language`
- documents representation: `indexing`
- find the best-matching document: `retrieval model`
- find efficiently:
- present result: `unsorted list`, `ranked list`, `clusters`
- evaluate IR system: evaluation

## 2. Document Indexing

Task: finding terms that describe documents well

|           | Manual                                                       | Automatic                                                    |
| --------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
|           | - indexing by humans<br />- labour & training intensive      | - term manipulation<br />- term weighting<br />- index terms must only derive from text |
| Trait     | large vocabularies                                           | - no predefined set of index terms<br />- natural language as indexing language<br />- words in the document give information about its content<br />- inverted files<br /> |
|           | - Dewey Decimal System<br />- Library of Congress Subject Headings<br />- ACM - subfield of CS<br />- MeSH - Medical Subject Headings | Google's IR system                                           |
| Advantage | - high precision search<br />- work well for closed collections |                                                              |
| Problem   | - search need to know terms to achieve high precision<br />- labeler need to trained to achieve consistency<br />- collection are dynamic |                                                              |

### 2.1 Manual

### 2.2 Automatic

#### 2.2.1 Inverted files

##### A basic inverted file index

- records for each term, the ids of the documents in which it appears
- only matters if it does or does not appear - not how many times

##### Variant inverted file 1

-  also record count of occurrences within each document
- help find documents ***more relevant*** to query

##### Variant inverted file 2

- also record position of each term occurrence with documents
- may be useful for searching for ***phrases*** in documents

## 3. Automated Retrieval Models

### 3.1 Boolean Search

 ````````````````````````````````A basic inverted file index

- records for each term, the ids of the documents in which it appears
- only matters if it does or does not appear - not how many times

#### Variant inverted file 1

-  also record count of occurrences within each document
- help find documents ***more relevant*** to query

#### Variant inverted file 2

- also record position of each term occurrence with documents
- may be useful for searching for ***phrases*** in documents

### 3.2 Ranked Algorithms



## 4. Term Manipulation

## 5. Web Search Ranking

## 6. Evaluation