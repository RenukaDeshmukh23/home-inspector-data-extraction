# Home Inspector Contact and Business Data Extraction

A completed client project using website-specific Python scripts to collect home inspector contact and business information from public directories and deliver formatted Excel batches.

**This repository documents the project and includes a synthetic output example. Original client datasets and scraping scripts are not included.**

## Business problem

The client needed contact and business information gathered from multiple websites and organized into structured spreadsheets. Requested fields included names, companies, phone numbers, emails, websites, addresses and services. Available fields differed between sources.

## My contribution

I researched public directories and a Google business directory, inspected page elements, identified XPath selectors and wrote a separate extraction script for each source website. Manual work focused on selector configuration; extraction ran automatically after configuration.

I also checked the outputs for missing and repeated values and formatted the Excel files for review. Each source was handled as a separate batch.

## Technology used

Python, Scrapy, Selenium, Beautiful Soup, Requests and XPath.

This stack describes the tools I used for the engagement. The original scripts are not part of this repository, so this is a case study rather than a runnable scraper package.

## Approach and decisions

1. Research directories containing relevant inspector and business information.
2. Inspect each website and configure XPath selectors for its page structure.
3. Build a dedicated extraction script for that source.
4. Run automated extraction after configuration.
5. Check missing and repeated values and prepare formatted Excel output.
6. Deliver separate batches reflecting the fields available from each source.

Dedicated scripts allowed the extraction logic to vary with each website. Separate batches preserved differing source schemas.

## Challenges

Page structures and available fields varied across sources, requiring individual configurations. Some websites were inaccessible from my region. Outputs also required checks for missing and repeated values.

## Deliverables and outcome

- Delivered Excel files containing the extracted information. The client received spreadsheet outputs only.
- Reviewed project materials include nine batch workbooks and a separate final workbook containing 1,454 data rows.
- Completed the assignment in approximately one month.
- The client accepted the delivery and subsequently hired me again.

Workbook counts and the final row count were checked against the project files. Duration, tools used, delivery acceptance and repeat hiring reflect my account of the engagement. Row counts are not counts of verified unique contacts or sales-qualified leads.

## Synthetic output example

See [samples/synthetic-output.json](samples/synthetic-output.json). Every record, contact placeholder, company, location and website in this example is fictional. The example follows the five-field structure of the final workbook; other batches used different fields.

| Company_Name | Phone | Name | Location | Website |
| --- | --- | --- | --- | --- |
| Example Inspection Company 01 | SYNTHETIC_PHONE_001 | Demo Inspector 01 | Example City A | https://inspector-01.example |
| Example Inspection Company 02 | Missing in demonstration | Demo Inspector 02 | Example City B | https://inspector-02.example |
| Example Inspection Company 03 | SYNTHETIC_PHONE_003 | Demo Inspector 03 | Example City C | https://inspector-03.example |

The missing phone value illustrates an output condition. It does not reproduce a client record or measure historical missingness.

## Viewing and setup

No installation is required to read this case study. Open the README and JSON example directly, or follow the optional local viewing instructions in [docs/SETUP.md](docs/SETUP.md).

There is no scraper entry point, dependency manifest or runnable demo in this repository. Original environment versions and setup commands have not been established.

## Limitations and confidentiality

Field availability depended on the source. Checks for missing and repeated values do not establish complete deduplication or a quantified accuracy rate. No measured time savings, revenue or lead-conversion results are claimed. The actual number of sources processed and the regional-access workaround are omitted because they have not been confirmed.

Original client files remain private. The included sample is newly created demonstration material. See [docs/SAFE_SAMPLE_GUIDANCE.md](docs/SAFE_SAMPLE_GUIDANCE.md) before adding other assets.

## Relevant capabilities

Python automation, web scraping, directory research, data extraction, data mining, XPath configuration, output checking and Excel delivery.
