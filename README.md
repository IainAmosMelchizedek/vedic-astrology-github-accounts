# Vedic Astrology GitHub Accounts

Curated list and dataset of GitHub accounts associated with Vedic astrology, Jyotish, and related projects.

## About

This repository contains a curated dataset of GitHub accounts whose public profile names, handles, or related terms appear connected to Vedic astrology, Jyotish, or adjacent concepts.

## Files

- data/accounts.csv — structured dataset of account handles
- README.md — project overview

## Dataset fields

- login — GitHub username
- category — current classification label
- notes — brief note about why the account is included
- source — where the account came from

## Notes

This is a curated candidate list based on public GitHub account discovery and keyword matching. Inclusion in this dataset does not by itself prove expertise, authenticity, or active project work in Vedic astrology.

## Methodology & Data Collection

This dataset was created using the GitHub API through the GitHub CLI (gh) and keyword-based account discovery.

### Approach

Candidate accounts were collected by searching GitHub users with terms such as:
- vedic astrology
- jyotish
- vedic

### Example API command

gh api --method GET search/users -f q="vedic astrology" --jq '.items[].login'

### Post-processing

- Combined results from multiple queries  
- Removed duplicate usernames  
- Filtered invalid API response lines  
- Exported the final list into a structured dataset  

### Limitations

- Based on keyword matching only  
- Inclusion does not guarantee relevance or activity  
- False positives are expected  
- This is a candidate dataset, not an authoritative registry

## Dataset Formats

This repository provides the dataset in multiple formats to support different use cases:

### CSV (`data/accounts.csv`)
- Best for spreadsheets, Excel, and quick inspection
- Tabular format with headers
- Easy to filter, sort, and analyze manually

### JSON (`data/accounts.json`)
- Structured format for APIs and general programming use
- Easily consumed by JavaScript, Python, and other languages
- Suitable for loading the entire dataset at once

### JSONL (`data/accounts.jsonl`)
- Line-delimited JSON format (one record per line)
- Optimized for machine learning and data pipelines
- Enables streaming processing without loading the entire dataset into memory
- Compatible with tools like Spark, BigQuery, and embedding pipelines

## Why Multiple Formats?

Providing the dataset in CSV, JSON, and JSONL ensures accessibility across:

- Analysts (CSV)
- Developers (JSON)
- Machine learning workflows (JSONL)

This multi-format approach increases usability, portability, and integration potential across different systems and workflows.
