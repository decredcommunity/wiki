# Community Projects

This is a list of smaller projects developed by Decred community members.

If you're want to join any BUIDL action around Decred but couldn't find anything suitable among the main dev [projects](https://devdocs.decred.org/projects/), use this list to find inspiration.

Decred is not only about development! A common mistake is to think that if you have no dev skills you cannot contribute, but reality is the opposite. Design and art, writing, outreach and negotiations, data science, and many other skills are needed to help the project deliver a [fair financial system](https://docs.decred.org/governance/decred-constitution/).

## Development

For main projects please see the [Projects](https://devdocs.decred.org/projects/) page at the dev docs.

### lightweight Jekyll theme

- description: trimmed down version of Primer theme, reusable as a tiny orphan Git branch by any GitHub Pages website
- languages: HTML, SASS
- location: https://github.com/decredcommunity/events/tree/jekyll
- status: in service
- uses:
  - this theme is used on events index [static pages](https://decredcommunity.github.io/events/index/)
- future work:
  - not sure, maybe tweak another theme like Cayman

### index utility

- description: generates static pages from YAML files that capture info about past events, used for reporting
- languages: Python, Markdown, YAML
- location: https://github.com/decredcommunity/events/tree/code
- status: in service
- uses:
  - pages built by the tool are [here](https://decredcommunity.github.io/events/index/)
  - the index database serves as a source of info for Decred Journal Events section
- future work:
  - add schema-based validation
  - improve templates
  - improve code
  - generalize code to apply in other areas, all the way up to decentralized collaborative censorship-resistant collection of arbitrary structired data (bookmarking, research, curated lists of things, etc). In fact, this very list is deliberately authored as structured data.

### media stats

- description: The project has several parts. There is a data format based on CSV for capturing time series data. Then there is a Python utility that semi-automates the collection of data points in that format. Then there is an R tool that builds charts from the data points.
- languages: Python, R, CSV
- location: https://github.com/decredcommunity/social-media-stats
- status: in service
- uses:
  - the data and tools together deliver [charts](https://github.com/decredcommunity/social-media-stats/blob/graphs/graphs/index.md) of social media activity for dozens of Decred-related accounts
  - time series database serves as a source for Decred Journal
  - prototype the concept of "multirepos" as an alternative to Git submodules
- future work:
  - collect data from web archive snapshots
  - automate scraping from Twitter/Reddit/etc pages
  - find JSON APIs for Twitter/Reddit/etc and add those as sources
  - add entry of custom timestamps to interactive mode

### media tracker utility

- description: scrape a wonderful zoo of metadata formats from articles, normalize and save into a CSV file
- languages: Python, HTML
- location: https://github.com/RichardRed0x/decred-media-tracker/pull/24
- status: unfinished
- future work:
  - add more metadata extractors
  - update existing CSV cells without destroying any data
  - grab data from JSON LD

## Research

### proposals knowledge database

- description: A lot of information is currently not captured by Politeia in a standard way, like valid billing periods, team members, list of discussions, reports on delivered work and spent funds, analysis, etc.
- languages: Markdown
- location: https://github.com/decredcommunity/proposals
- status: in service
- uses:
  - dozens of reports scattered across Reddit, GitHub and Matrix have been collected and polished
  - several analysis documents are hosted
  - a few scattered proposals drafts have been saved so that anyone can continue them if original authors stop developing the ideas
- future work:
  - much more scattered data can be collected for Politeia's 100+ processed proposals
  - develop what data to capture and in what format
  - generate index pages usable by humans to navigate the repository, possibly adopting the [index utility](#index-utility)

## Translations
