# HospitalProviderInfoWebScrape
Jupyter Notebooks with webscraping/NPI query code

## Objective:
These two notebooks have the code for the functions I used to scrape healthcare provider demographics information for a work project.  THe goal of this project was to collect hospital affiliation and provider contact information from several hospital group websites.  The code in these two notebooks was adapted for several other hospital networks, but the general structure was the same.

As the project progressed, I focused only on the provider specialties associated with hospital-based physicians (Anesthesiology, Radiology, Pathology, Neonatology, Emergency Medicine, and Hospitalist)

## General steps:
Each site was a bit different, but the general steps to this project were
1. Get a provider roster from a series of Find-A-Provider pages; these rosters often had links to the individual provider profile site.
2. Use the roster as a guide to scrape each provider site, which included hospital affiliations or practice locations.
3. Use the physician name, state, zip, and specialty as query parameters to pull NPI (national provider ID number) from NPPES (https://npiregistry.cms.hhs.gov)
