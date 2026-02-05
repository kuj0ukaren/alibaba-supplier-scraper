# Alibaba Supplier Scraper

[![Apify Actor](https://img.shields.io/badge/Apify-Actor-blue)](https://apify.com/devcake/alibaba-supplier-scraper)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.10+-blue)](https://www.python.org/)
[![B2B Scraping](https://img.shields.io/badge/purpose-b2b--scraping-orange)](#)

**Find verified, trustworthy suppliers on Alibaba.com in minutes.** Extract factory information, Gold Supplier years, verification status, and response rates to identify reliable partners for your dropshipping or Amazon FBA business.

---

## What is Alibaba Supplier Scraper?

**Alibaba Supplier Scraper** is a specialized tool for extracting **detailed supplier profiles** from Alibaba.com. Stop wasting hours on unreliable suppliers - this high-speed scraper finds verified manufacturers with Gold Supplier years, verification status, and real response rates perfect for dropshipping and Amazon FBA. Extract factory information, staff count, annual revenue, product portfolios, and ratings.

## Why Use Alibaba Supplier Scraper?

### Business Use Cases:
- **New Dropshippers** - Verifying suppliers before placing first orders
- **Amazon FBA Sellers** - Needing suppliers with proper verification for brand protection
- **Product Researchers** - Validating factory capabilities before ordering samples
- **Profit Hunters** - Finding suppliers with OEM services for custom branding
- **E-commerce Entrepreneurs** - Avoiding scams with verified supplier data

This scraper extracts the EXACT verification data you need:

| Your Need | What We Extract | Why It Matters |
|-----------|----------------|----------------|
| **Trust Verification** | `is_assessed_supplier`, `is_verified_supplier_pro` | Avoid scams with Alibaba's verification system |
| **Quality Assurance** | Gold Supplier years, review scores | Find suppliers with proven track records |
| **Fast Communication** | `response_rate` (≤3h) | Identify responsive suppliers |
| **Factory Reliability** | `factory_size`, `total_employees` | Verify actual manufacturing capacity |
| **Service Capabilities** | OEM/ODM service tags | Find suppliers who offer private labeling |
| **Product Match** | `products_offered` data | Confirm suppliers actually make what they claim |

## How to Find Verified Suppliers

1. **Open the [Alibaba Supplier Scraper on Apify](https://apify.com/devcake/alibaba-supplier-scraper)**
2. **Enter search queries** (e.g., "wireless earbuds", "phone cases")
3. **Set max pages** (1-50, 20 suppliers per page)
4. **Click "Start"** and download supplier data

**Pro Tip**: Look for Gold Supplier years ≥5 and response rates ≤3h for reliable suppliers.

## Features

### Supplier Verification Data
- **Gold Supplier Years** - Years as Gold Supplier (critical metric)
- **Verified Status** - Assessed Supplier & Verified Pro flags
- **Response Rate** - Typical response time (≤3h = good)
- **Review Count** - Number of buyer reviews
- **Review Score** - Average review rating (1-5)

### Factory Intelligence
- **Total Employees** - Staff count (indicates capacity)
- **Factory Size** - Production space (m²)
- **Annual Revenue** - Estimated revenue volume
- **Products Offered** - Actual products manufactured
- **Service Tags** - OEM, ODM, customization capabilities

## Pricing

**Pay-per-event pricing** for maximum cost efficiency:

| Event | Price |
|-------|-------|
| **Actor Start** | $0.01 |
| **Per Supplier** | $0.005 |

### Cost Examples
- Extract 100 suppliers: $0.51
- Extract 500 suppliers: $2.51
- Extract 1,000 suppliers: $5.01

## Input

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `queries` | array | ✅ Yes | Search queries to scrape suppliers for |
| `max_pages` | integer | No | Max pages per query (default: 1, 20 suppliers/page) |

### Input Example

```json
{
  "queries": ["phone cases manufacturer"],
  "max_pages": 10
}
```

## Output Example

```json
{
  "search_query": "phone case manufacturer",
  "company_id": 50056289,
  "name": "Guangzhou Sinatech Technology Co., Ltd.",
  "country": "China",
  "country_code": "CN",
  "years_as_gold_supplier": 23,
  "company_icon": "https://s.alicdn.com/@sc04/...",
  "profile_url": "https://sinatech.en.alibaba.com/company_profile.html",
  "total_employees": "60+ staff",
  "factory_size": "1,800+ m²",
  "annual_revenue": "US $20,000+",
  "response_rate": "≤3h",
  "is_assessed_supplier": true,
  "is_verified_supplier_pro": false,
  "products_offered": "Leather Phone Case, Leather Phone Bag, Leather Tablets Case",
  "review_count": 6,
  "review_score": 4.5,
  "service_tags": [
    "Customized packaging",
    "Graphic customization",
    "Online support",
    "OEM Service"
  ]
}
```

## Related Actors

| Actor | Description | Pricing |
|-------|-------------|---------|
| [Alibaba Products Scraper](https://github.com/devcake/alibaba-products-scraper) | Find profitable products with low MOQ | $0.005/supplier |
| [GlobalSources Products Scraper](https://github.com/devcake/globalsources-products-scraper) | Source from 10M+ verified suppliers | $0.005/supplier |
| [GlobalSources Supplier Scraper](https://github.com/devcake/globalsources-supplier-scraper) | 6-level verification data | $0.005/supplier |

## FAQ

### What is Gold Supplier status?
Gold Supplier is Alibaba's premium membership for verified suppliers. Years as Gold Supplier indicates established business presence and reliability.

### How do I verify supplier credibility?
Look for suppliers with: (1) Business license verification, (2) 3+ years as Gold Supplier, (3) High response rates (90%+), (4) Trade Assurance coverage, (5) On-site check verification.

### Can I get supplier contact information?
Yes, when available, the scraper extracts emails, phone numbers, addresses, and company websites from supplier profiles.

### What's the difference between manufacturers and traders?
Manufacturers produce products directly and typically offer lower prices. Traders are middlemen who source from manufacturers.

### How do I find suppliers in my industry?
Search for products in your industry using search queries like "wireless earbuds manufacturer" or "phone case supplier".

## Get it on Apify

[![Run on Apify](https://img.shields.io/badge/Run_on-Apify-informational?style=for-the-badge&logo=apify)](https://apify.com/devcake/alibaba-supplier-scraper)

**Start finding verified suppliers in minutes!**

---

## Also by @devcake

Check out my other scraping tools:

### Pinterest Suite
- [Pinterest Search Scraper](https://github.com/devcake/pinterest-search-scraper) - Search Pinterest by keywords
- [Pinterest Board Scraper](https://github.com/devcake/pinterest-board-scraper) - Download complete boards
- [Pinterest Profile Scraper](https://github.com/devcake/pinterest-profile-scraper) - Extract user profiles with emails
- [Pinterest Pin Scraper](https://github.com/devcake/pinterest-pin-scraper) - Scrape pins with product data

### Other Tools
- [AlternativeTo Data Scraper](https://github.com/devcake/alternativeto-data-scraper) - Extract software alternatives with license filters

---

**License**: MIT | **Author**: [@devcake](https://apify.com/u/devcake)

[![GitHub stars](https://img.shields.io/github/stars/devcake/alibaba-supplier-scraper?style=social)](https://github.com/devcake/alibaba-supplier-scraper)
