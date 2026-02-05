# Alibaba Supplier Scraper

[![Apify Actor](https://img.shields.io/badge/Apify-Actor-blue)](https://apify.com/devcake/alibaba-supplier-scraper)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.10+-blue)](https://www.python.org/)
[![B2B Scraping](https://img.shields.io/badge/purpose-b2b--scraping-orange)](#)

**Extract Alibaba supplier profiles with Gold Supplier status, verification level, response rate, and contact details.** Crucial for vendor vetting and B2B sourcing.

---

## What is Alibaba Supplier Scraper?

**Alibaba Supplier Scraper** is a specialized tool for extracting **supplier and company profiles** from Alibaba.com. Retrieve comprehensive supplier data including Gold Supplier status, verification levels, business type, production capacity, response rates, trade history, and contact information. Essential for due diligence, supplier qualification, and B2B lead generation.

## Why Use Alibaba Supplier Scraper?

### Business Use Cases:
- **Supplier Vetting** - Verify supplier credentials before placing orders
- **Due Diligence** - Research supplier background and verification status
- **Lead Generation** - Build databases of verified suppliers in your industry
- **Competitor Analysis** - Monitor competitor supplier relationships
- **Sourcing Decisions** - Compare suppliers across multiple criteria
- **Risk Assessment** - Evaluate supplier reliability and trade history

## How to Scrape Alibaba Suppliers

1. **Open the [Alibaba Supplier Scraper on Apify](https://apify.com/devcake/alibaba-supplier-scraper)**
2. **Enter supplier URLs** or search for suppliers by keyword
3. **Configure options** (include products, contact details)
4. **Click "Start"** and wait for extraction
5. **Download data** with verification and contact info

**Pro Tip**: Use Alibaba Products Scraper first to find products, then extract supplier URLs from those results to get detailed supplier profiles.

## Features

✅ **Gold Supplier Status** - Check years as Gold Supplier and membership level

✅ **Verification Level** - Extract verified business information and credentials

✅ **Response Rate** - Get supplier response times and rates

✅ **Business Type** - Identify manufacturer, trader, or hybrid

✅ **Production Capacity** - Extract factory capabilities and output

✅ **Trade History** - Get transaction history and export data

✅ **Contact Details** - Extract emails, phone numbers, and addresses

✅ **Product Count** - See total products listed by supplier

## Pricing

| Plan | Price | Results |
|------|-------|---------|
| Pay-per-event | **$0.005** | 1 supplier profile |
| Bulk | Custom | Thousands of suppliers |

**Try it free** with Apify's trial credits!

## Input Example

```json
{
  "supplierUrls": [
    "https://www.alibaba.com/profile/abc-electronics-co.html"
  ],
  "includeProducts": true,
  "includeContactInfo": true,
  "proxy": {
    "useApifyProxy": true
  }
}
```

## Output Example

```json
{
  "supplierId": "220123456789",
  "companyName": "Shenzhen ABC Electronics Co., Ltd.",
  "supplierUrl": "https://www.alibaba.com/profile/abc-electronics-co.html",
  "isGoldSupplier": true,
  "goldSupplierYears": 8,
  "isVerified": true,
  "verificationLevel": "Business License Verified",
  "businessType": "Manufacturer",
  "responseRate": "97%",
  "responseTime": "Within 24 hours",
  "productionCapacity": "100,000 Pieces per Month",
  "totalProducts": 342,
  "tradeAssurance": true,
  "mainMarkets": ["North America", "Western Europe", "Domestic Market"],
  "contact": {
    "address": "Floor 3, Building 5, Shenzhen, Guangdong, China",
    "phone": "+86-755-12345678",
    "email": "sales@abcelectronics.com"
  },
  "website": "https://www.abcelectronics.com"
}
```

## Related Actors

| Actor | Description |
|-------|-------------|
| [Alibaba Products Scraper](https://github.com/Bahm9919/alibaba-products-scraper) | Scrape product listings with MOQ |
| [GlobalSources Supplier Scraper](https://github.com/Bahm9919/globalsources-supplier-scraper) | Extract 6-level verified suppliers |
| [GlobalSources Products Scraper](https://github.com/Bahm9919/globalsources-products-scraper) | Scrape product listings with specs |

## FAQ

### What is Gold Supplier status?
Gold Supplier is Alibaba's premium membership for verified suppliers. Years as Gold Supplier indicates established business presence and reliability.

### How do I verify supplier credibility?
Look for suppliers with: (1) Business license verification, (2) 3+ years as Gold Supplier, (3) High response rates (90%+), (4) Trade Assurance coverage, (5) On-site check verification.

### Can I get supplier contact information?
Yes, when available, the scraper extracts emails, phone numbers, addresses, and company websites from supplier profiles.

### What's the difference between manufacturers and traders?
Manufacturers produce products directly and typically offer lower prices. Traders are middlemen who source from manufacturers. Both have advantages depending on your needs.

### How do I find suppliers in my industry?
Search for products in your industry using Alibaba Products Scraper, then extract supplier URLs to get detailed profiles using this scraper.

## Get it on Apify

[![Run on Apify](https://img.shields.io/badge/Run_on-Apify-informational?style=for-the-badge&logo=apify)](https://apify.com/devcake/alibaba-supplier-scraper)

**Start extracting Alibaba supplier profiles in minutes!**

---

## Also by @devcake

Check out my other scraping tools:

- [Pinterest Search Scraper](https://github.com/Bahm9919/pinterest-search-scraper)
- [Pinterest Profile Scraper](https://github.com/Bahm9919/pinterest-profile-scraper)
- [AlternativeTo Data Scraper](https://github.com/Bahm9919/alternativeto-data-scraper)

---

**License**: MIT | **Author**: [@devcake](https://apify.com/u/devcake)

[![GitHub stars](https://img.shields.io/github/stars/Bahm9919/alibaba-supplier-scraper?style=social)](https://github.com/Bahm9919/alibaba-supplier-scraper)
