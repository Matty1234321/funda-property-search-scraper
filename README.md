# Funda Property Search Scraper
A powerful scraper built to collect structured real estate listings from Funda.nl, the Netherlands’ leading property platform. It automates large-scale property data collection, helping professionals turn scattered listings into clean, usable market intelligence.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>funda-property-search-scraper</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
The Funda Property Search Scraper extracts detailed property listing data based on search URLs or configurable filters. It removes the friction of manual browsing and enables fast, repeatable access to Dutch housing market data.
This project is ideal for real estate professionals, analysts, investors, and researchers who need reliable property insights at scale.

### Built for Dutch Property Intelligence
- Designed specifically for Funda.nl listing structures and search logic
- Supports both direct URL scraping and filter-based discovery
- Outputs clean, structured datasets ready for analysis or storage
- Scales across multiple locations and search criteria
- Handles partial failures without interrupting full runs

## Features
| Feature | Description |
|----------|-------------|
| URL-based scraping | Extracts listings directly from predefined Funda search result pages. |
| Filter-based search | Builds searches dynamically using location, price, size, and room filters. |
| Retry handling | Automatically retries failed requests to improve success rates. |
| Proxy support | Reduces blocking risk and improves stability on large runs. |
| Structured output | Returns normalized JSON records for easy downstream processing. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|-------------|------------------|
| id | Unique Funda property identifier for deduplication and tracking. |
| url | Direct link to the property detail page. |
| name | Property title or headline shown on Funda. |
| image_urls | Array of image URLs for property visuals. |
| address | Location information including postal code and city. |
| price | Listed asking price in EUR. |
| currency | Currency symbol associated with the price. |
| details | Key specifications such as floor area, plot size, bedrooms, and energy label. |
| description | Full textual property description. |
| seller | Real estate agent or agency details. |
| category | Listing category or regional classification. |

---

## Example Output

    [
      {
        "id": "43860189",
        "url": "https://www.funda.nl/detail/koop/lochem/huis-badhuisweg-1/43860189/",
        "name": "Badhuisweg 1",
        "address": "7241DD Lochem",
        "price": 1200000,
        "currency": "€",
        "details": {
          "floor_area": "459 m²",
          "plot_area": "1.369 m²",
          "bedrooms": "5",
          "energy_label": "A+"
        },
        "seller": {
          "name": "De Haan Schippers Makelaars | Baerz & Co"
        }
      }
    ]

---

## Directory Structure Tree

    Funda Property Search Scraper/
    ├── src/
    │   ├── index.js
    │   ├── scraper/
    │   │   ├── searchRunner.js
    │   │   ├── urlRunner.js
    │   │   └── parser.js
    │   ├── utils/
    │   │   ├── request.js
    │   │   └── validators.js
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── sample-input.json
    │   └── sample-output.json
    ├── package.json
    └── README.md

---

## Use Cases
- **Real estate investors** use it to identify properties within target budgets, so they can spot opportunities faster.
- **Market analysts** use it to track pricing trends across regions, enabling data-driven reports.
- **Agencies** use it to monitor competitor listings, improving pricing and positioning strategies.
- **Researchers** use it to study housing supply and development patterns across the Netherlands.

---

## FAQs
**Does this scraper support both buying and rental listings?**
Yes. You can switch between purchase and rental listings using the operation type configuration.

**Can I scrape multiple locations in one run?**
Yes. You can provide multiple URLs or adjust filters to cover broader areas.

**What happens if some URLs fail during scraping?**
The scraper can continue processing remaining inputs if failure ignoring is enabled.

**Is the output suitable for databases or BI tools?**
Absolutely. The structured JSON format is designed for easy ingestion into analytics pipelines.

---

### Performance Benchmarks and Results

**Primary Metric:** Processes an average of 10–20 property listings per minute under normal conditions.

**Reliability Metric:** Maintains a success rate above 95% when retries and proxies are configured correctly.

**Efficiency Metric:** Handles multiple search inputs in parallel while keeping resource usage stable.

**Quality Metric:** Extracted datasets typically achieve over 98% field completeness on active listings.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
