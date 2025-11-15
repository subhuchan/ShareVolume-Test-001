# APA Corporation Stock Data

This web application fetches and displays the maximum and minimum shares outstanding for APA Corporation (CIK: 0001841666) from the SEC EDGAR database.  It uses the `EntityCommonStockSharesOutstanding` concept from the `dei` taxonomy.  The application filters the data to only include years after 2020.

## Features

*   Displays the entity name, maximum shares outstanding, and minimum shares outstanding.
*   Fetches data from the SEC API.
*   Handles errors gracefully.
*   Supports a `CIK` query parameter to fetch data for other companies.
*   Renders a visually appealing interface.

## Usage

1.  Open `index.html` in a web browser.
2.  To view data for APA Corporation, simply open `index.html`.
3.  To view data for a different company, append `?CIK=<10-digit CIK>` to the URL (e.g., `index.html?CIK=0001018724`).

## Files

*   `index.html`: The main HTML file that displays the data.
*   `data.json`: A JSON file containing sample data (overwritten by the fetch). Not committed dynamically.
*   `uid.txt`: A text file containing the unique identifier.
*   `README.md`: This file.

## Dependencies

*   None (pure HTML, CSS, and JavaScript)

## API Used

*   SEC EDGAR API: `https://data.sec.gov/api/xbrl/companyconcept/CIK<CIK>/dei/EntityCommonStockSharesOutstanding.json`

## License

MIT License
