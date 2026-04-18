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
