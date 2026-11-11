# AUC Library: Cross-API Bibliographic Data Integration

Python and Pandas system built during my internship at AUC Libraries and Learning Technologies (Jul to Aug 2024). It finds overlaps between AUC's roughly 500,000 printed books and electronic collections on HathiTrust and Open Library, using their APIs.

## What it does
- Loads the AUC library catalogue in batches (`Data/batches.csv`) and cleans the identifiers (OCLC, LCCN, ISBN)
- Queries the HathiTrust catalogue API for each identifier and extracts the title, view status, view link and MARC XML record
- Experiments with Open Library as a second source for books HathiTrust does not cover
- Compiles the results into structured Excel sheets so the library team can expand digital access to the collection

## Files
- `Group4.ipynb`: the full pipeline (data loading, exploratory analysis, HathiTrust batch processing, Open Library experiments)
- `Data/batches.csv`: input batches of catalogue records

## Stack
Python, Pandas, Requests, pymarc, XlsxWriter, Google Colab
