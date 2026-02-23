# AutoTrader Vehicle Listings Dataset

![Updated](https://img.shields.io/badge/updated-2026--02--23-brightgreen?style=flat-square)&nbsp;![Records](https://img.shields.io/badge/records-1.3M-blue?style=flat-square)&nbsp;[![Rebrowser](https://img.shields.io/badge/full%20dataset-rebrowser.net-orange?style=flat-square)](https://rebrowser.net/products/datasets/autotrader)

New, used, and certified pre-owned vehicle listings from AutoTrader with pricing, KBB valuations, dealer info, drivetrain specs, and listing placement data.


This repository contains a preview sample of the [AutoTrader dataset](https://rebrowser.net/products/datasets/autotrader) published by Rebrowser. If you're doing academic research, you may be eligible for free access to a much larger slice — see [Free Datasets for Research](https://rebrowser.net/free-datasets-for-research).


This dataset contains **1** entity, each in its own folder: Car Listings (`car-listings`). See below for a full field breakdown, sample counts, and data distributions for each.

*Found this useful? ⭐ Star this repo to help us keep publishing fresh data. Found an error? [Let us know](https://rebrowser.net/contact-us).*


---

### Car Listings
AutoTrader vehicle listings with make, model, trim, body style, mileage, MSRP, KBB fair price range, deal rating, drivetrain, fuel type, seller location, and listing priority.




> **1,334,959** total records from 2025-11-16 to 2026-02-22, **up to 30,000** rows in this sample (2.2% of full dataset).
> Exported as one file per day, up to 1,000 rows each, last undefined days retained.

![Data Growth](car-listings/chart-growth.svg)

| Field | Type | Fill Rate | Description |
| --- | --- | --- | --- |
| `_primaryKey` | `string` | 100% | Unique identifier for this record |
| `_firstSeenAt` | `datetime` | 100% | First time this record was seen |
| `_lastSeenAt` | `datetime` | 100% | Last time this record was updated |
| `listingId` | `string` | 100% | Unique Autotrader listing ID |
| `vin` 🔒 | `string` | 100% | Vehicle Identification Number (17-character unique code) |
| `stockNumber` | `string` | 99% | Dealer stock number |
| `year` | `float` | 100% | Vehicle model year |
| `makeCode` | `string` | 100% | Make code (e.g., BMW, TOYOTA, GENESIS) |
| `makeName` | `string` | 100% | Make display name (e.g., BMW, Toyota, Genesis) |
| `modelCode` | `string` | 100% | Model code (e.g., X3, CAMRY, GENGV80) |
| `modelName` | `string` | 100% | Model display name (e.g., X3, Camry, GV80) |
| `trim` | `string` | 96% | Vehicle trim level (e.g., xDrive30i, 3.5T Prestige) |
| `bodyStyle` | `string` | 96% | Body style (e.g., SUV, Sedan, Truck) |
| `listingType` | `string` | 100% | Listing type (New, Used, Certified) |
| `listingTitle` | `string` | 100% | Full listing title (e.g., "Used 2025 BMW X3 xDrive30i w/ Convenience Package") |
| `mileage` | `float` | 100% | Odometer reading in miles |
| `salePrice` 🔒 | `float` | 99% | Listed sale price in USD |
| `msrp` | `float` | 8% | Manufacturer Suggested Retail Price in USD (for New vehicles) |
| `dealIndicator` | `string` | 67% | KBB deal rating (Great, Good, Fair, High, Overpriced) |
| `kbbFairPurchasePrice` 🔒 | `float` | 98% | KBB Fair Purchase Price estimate in USD |
| `kbbFairPriceLow` | `float` | 98% | KBB Fair Purchase Price low range in USD |
| `kbbFairPriceHigh` | `float` | 98% | KBB Fair Purchase Price high range in USD |
| `exteriorColor` | `string` | 99% | Exterior color name (e.g., Alpine White, Capri Blue) |
| `exteriorColorSimple` | `string` | 99% | Simplified exterior color (e.g., WHITE, BLUE, BLACK) |
| `interiorColor` | `string` | 96% | Interior color name (e.g., Espresso Brown, Blue) |
| `interiorColorSimple` | `string` | 96% | Simplified interior color (e.g., BROWN, BLUE, BLACK) |
| `engineCode` | `string` | 100% | Engine code (e.g., 4CLDR, 6CLDR) |
| `engine` | `string` | 100% | Engine description (e.g., 4-Cylinder Turbo, 6-Cylinder Turbo) |
| `drivetrain` | `string` | 90% | Drivetrain type (e.g., All wheel drive, Front-wheel drive) |
| `transmissionCode` | `string` | 99% | Transmission code (e.g., AUT, MAN) |
| `transmission` | `string` | 99% | Transmission type (e.g., 8-Speed Automatic) |
| `transmissionGroup` | `string` | 99% | Transmission type group (Automatic, Manual) |
| `fuelTypeCode` | `string` | 91% | Fuel type code (e.g., G, D, E) |
| `fuelType` | `string` | 91% | Fuel type (e.g., Gasoline, Diesel, Electric) |
| `fuelTypeGroup` | `string` | 91% | Fuel type group (Gas, Diesel, Electric, Hybrid) |
| `mpgCity` | `float` | 80% | City fuel economy in MPG |
| `mpgHighway` | `float` | 80% | Highway fuel economy in MPG |
| `displacementUOM` | `float` | 100% | Engine displacement in liters (e.g., 2.0, 3.5) |
| `hasLeatherSeats` | `bool` | 100% | Whether vehicle has leather seats |
| `daysOnMarket` | `float` | 98% | Number of days listing has been on market |
| `isHot` | `bool` | 100% | Hot listing flag (high interest) |
| `isNewlyListed` | `bool` | 100% | Recently listed flag |
| `isReducedPrice` | `bool` | 100% | Price recently reduced flag |
| `isNoHagglePrice` | `bool` | 100% | No-haggle/fixed price flag |
| `hasSpecialOffer` | `bool` | 100% | Has special offer/promotion |
| `moneyBackGuarantee` | `bool` | 100% | Money-back guarantee offered |
| `mainImageIsStock` | `bool` | 100% | Main image is stock photo (not actual vehicle) |
| `priority` | `string` | 100% | Listing priority/tier (PREMIUM, STANDARD, BASIC) |
| `sellerId` | `float` | 100% | Seller/dealer ID |
| `sellerName` 🔒 | `string` | 100% | Seller/dealer name |
| `sellerPhone` 🔒 | `string` | 97% | Seller phone number |
| `sellerRating` 🔒 | `float` | 96% | Seller KBB rating (1-5 scale) |
| `sellerReviewCount` | `float` | 96% | Number of seller reviews |
| `sellerWebsite` 🔒 | `string` | 96% | Seller website URL |
| `isPrivateSeller` | `bool` | 100% | Whether seller is a private seller (true) or dealer (false) |
| `sellerContractLevel` | `string` | 97% | Seller contract level (PARTNER, STANDARD, etc.) |
| `kbbVehicleId` | `float` | 94% | KBB vehicle ID for price lookup |
| `kbbConsumerRatings` | `float` | 100% | KBB consumer rating (1-5 scale) |
| `kbbConsumerReviewCount` | `float` | 100% | Number of KBB consumer reviews |
| `safetyRecallCount` | `float` | 89% | Number of open safety recalls |
| `vhrPreview` | `string` | 98% | Vehicle history report preview flags (JSON array: NO_SALVAGE_TITLE, NO_ACCIDENTS_REPORTED, ONE_OWNER, etc.) |
| `options` | `string` | 98% | Vehicle options object with subcategories: exterior, interior, safety, mechanical, technology, other |
| `optionsCount` | `float` | 98% | Total number of options across all categories |
| `description` | `string` | 99% | Full marketing description text (HTML tags stripped except br) |
| `images` 🔒 | `string` | 99% | All listing image URLs as JSON array |
| `imagesCount` | `float` | 99% | Number of listing images |
| `sellerAddress` | `string` | 97% | Seller address line 1 |
| `sellerCity` | `string` | 100% | Seller city |
| `sellerState` | `string` | 100% | Seller state |
| `sellerZip` | `string` | 100% | Seller ZIP code |
| `listingUrl` 🔒 | `string` | 100% | Full URL to the Autotrader listing page |



> 🔒 **Premium fields** are included in the data files but their values are replaced with `[PREMIUM]`. To access real values, [use our website](https://rebrowser.net/products/datasets/autotrader).



#### Field Distributions


<details>
<summary><strong>Listing Type (New / Used / Certified)</strong> (<code>listingType</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Used | 1,065,046 | `████████████████░░░░` 79.8% |
| Certified | 164,549 | `██░░░░░░░░░░░░░░░░░░` 12.3% |
| New | 105,364 | `██░░░░░░░░░░░░░░░░░░` 7.9% |

</details>


<details>
<summary><strong>Body Style Distribution</strong> (<code>bodyStyle</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| SUV | 629,806 | `██████████░░░░░░░░░░` 49.2% |
| TRUCKS | 270,968 | `████░░░░░░░░░░░░░░░░` 21.1% |
| SEDAN | 222,288 | `███░░░░░░░░░░░░░░░░░` 17.3% |
| COUPE | 47,049 | `█░░░░░░░░░░░░░░░░░░░` 3.7% |
| HATCH | 45,414 | `█░░░░░░░░░░░░░░░░░░░` 3.5% |
| VANS | 31,652 | `░░░░░░░░░░░░░░░░░░░░` 2.5% |
| CONVERT | 28,351 | `░░░░░░░░░░░░░░░░░░░░` 2.2% |
| WAGON | 5,698 | `░░░░░░░░░░░░░░░░░░░░` 0.4% |

</details>


<details>
<summary><strong>Fuel Type Distribution</strong> (<code>fuelTypeGroup</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| Gas | 1,102,573 | `██████████████████░░` 91.1% |
| Hybrid: Gas/Electric | 51,522 | `█░░░░░░░░░░░░░░░░░░░` 4.3% |
| Electric | 40,839 | `█░░░░░░░░░░░░░░░░░░░` 3.4% |
| Plug-in Hybrid: Gas/Electric | 15,321 | `░░░░░░░░░░░░░░░░░░░░` 1.3% |

</details>


<details>
<summary><strong>Top States by Listing Count</strong> (<code>sellerState</code>)</summary>


| Value | Count | Share |
| --- | --- | --- |
| TX | 169,458 | `████░░░░░░░░░░░░░░░░` 21.3% |
| CA | 152,995 | `████░░░░░░░░░░░░░░░░` 19.2% |
| FL | 136,894 | `███░░░░░░░░░░░░░░░░░` 17.2% |
| NC | 57,371 | `█░░░░░░░░░░░░░░░░░░░` 7.2% |
| OH | 55,333 | `█░░░░░░░░░░░░░░░░░░░` 7.0% |
| GA | 53,135 | `█░░░░░░░░░░░░░░░░░░░` 6.7% |
| IL | 45,225 | `█░░░░░░░░░░░░░░░░░░░` 5.7% |
| AZ | 44,163 | `█░░░░░░░░░░░░░░░░░░░` 5.6% |
| PA | 40,985 | `█░░░░░░░░░░░░░░░░░░░` 5.2% |
| WA | 39,801 | `█░░░░░░░░░░░░░░░░░░░` 5.0% |

</details>






---

## Pre-built Views on Rebrowser

Rebrowser web viewer lets you filter, sort, and export any slice of this dataset interactively. These pre-built views are ready to open:


### Car Listings


[Listings with Pricing Data](https://rebrowser.net/products/datasets/autotrader/car-listings/views/listings-with-pricing) — 1,102,980 records

↳ `[{"field":"salePrice","op":"gt","value":0},{"sort":"salePrice DESC"}]`

[Certified Pre-Owned Listings](https://rebrowser.net/products/datasets/autotrader/car-listings/views/certified-preowned-listings) — 139,117 records

↳ `[{"field":"listingType","op":"is","value":"Certified"},{"sort":"salePrice DESC"}]`

[New Vehicle Listings](https://rebrowser.net/products/datasets/autotrader/car-listings/views/new-vehicle-listings) — 98,977 records

↳ `[{"field":"listingType","op":"is","value":"New"},{"sort":"msrp DESC"}]`

[Used Vehicle Listings](https://rebrowser.net/products/datasets/autotrader/car-listings/views/used-vehicle-listings) — 864,763 records

↳ `[{"field":"listingType","op":"is","value":"Used"},{"sort":"salePrice DESC"}]`

[Premium and Sponsored Listings](https://rebrowser.net/products/datasets/autotrader/car-listings/views/premium-listings) — 989,943 records

↳ `[{"field":"priority","op":"is","value":"PREMIUM"},{"sort":"salePrice DESC"}]`


*[See all 34 views →](https://rebrowser.net/products/datasets/autotrader/car-listings)*




---

## Code Examples

```python
import pandas as pd
from pathlib import Path

# ── Car Listings ──────────────────────────────────────────────────────────────
# Load the last 7 days of listings
files = sorted(Path('rebrowser/autotrader-dataset/car-listings/data').glob('*.parquet'))[-7:]
listings = pd.concat([pd.read_parquet(f) for f in files])

# Median KBB fair price midpoint by make for new vehicles
listings['kbbMidpoint'] = (listings['kbbFairPriceLow'] + listings['kbbFairPriceHigh']) / 2
new_cars = listings[listings['listingType'] == 'New']
print(new_cars.groupby('makeName')['kbbMidpoint'].median()
      .sort_values(ascending=False).head(15).to_string())

# Certified pre-owned listing count by body style
cpo = listings[listings['listingType'] == 'Certified']
print(cpo['bodyStyle'].value_counts().to_string())

# Average days on market by fuel type group for used vehicles
used = listings[listings['listingType'] == 'Used']
print(used.groupby('fuelTypeGroup')['daysOnMarket'].mean().sort_values().to_string())

# Listing volume and premium-placement rate by state
state_stats = listings.groupby('sellerState').agg(
    total=('listingId', 'count'),
    premium=('priority', lambda x: (x == 'PREMIUM').sum())
).assign(pct_premium=lambda d: (d['premium'] / d['total'] * 100).round(1))
print(state_stats.sort_values('total', ascending=False).head(15).to_string())
```

---

## Use Cases


### Market Pricing Analysis

Compare MSRP and KBB fair price ranges across makes, models, and trim levels to identify over- and under-priced listings. Filter by body style and state to benchmark regional pricing gaps.


### Inventory Trend Tracking

Monitor which makes and body styles dominate dealer inventory by state. Track days-on-market to identify slow-moving segments and spot seasonal inventory shifts.


### EV & Fuel Type Research

Filter by fuelTypeGroup to analyze electric, hybrid, and diesel vehicle availability and regional adoption patterns relative to gasoline alternatives.


### Deal Quality Scoring

Use KBB deal indicator ratings alongside KBB price ranges to rank listings by value. Identify which markets and vehicle types produce the most "Great Deal" inventory.



---

## Full Dataset on Rebrowser


This repo is a 1,000-row preview sample. The full dataset is at [rebrowser.net/products/datasets/autotrader](https://rebrowser.net/products/datasets/autotrader)

Doing academic research? You may qualify for free access to a larger slice. See [Free Datasets for Research](https://rebrowser.net/free-datasets-for-research).

On Rebrowser you can:
- **Filter before you buy** — use the web UI to apply filters on any field and sort by any column. Preview results before purchasing. You only pay for records that match your criteria.
- **Export in your format** — CSV, JSON, JSONL, or Parquet depending on your plan.
- **Access via API** — integrate dataset queries into your pipelines and workflows.
- **Choose your freshness** — plans range from a 14-day lag to real-time data with no delay.
- **Select only the fields you need** — keep exports lean. Premium fields with richer data are available on higher plans.

[Pricing](https://rebrowser.net/pricing) starts at **$2 per 1,000 rows** with volume discounts.

---

## License & Terms

**Free for research and non-commercial use** with attribution. See [license terms](https://rebrowser.net/free-datasets-for-research#license) and [how to cite](https://rebrowser.net/free-datasets-for-research#citation).

```bibtex
@misc{rebrowser_autotrader,
  author       = {Rebrowser},
  title        = {AutoTrader Vehicle Listings Dataset},
  year         = {2026},
  howpublished = {\url{https://rebrowser.net/products/datasets/autotrader}},
  note         = {Accessed: YYYY-MM-DD}
}
```

Commercial use requires a paid license — see [pricing](https://rebrowser.net/pricing). Use of this data is governed by the [Rebrowser Terms of Use](https://rebrowser.net/terms-of-use), which may be updated at any time independently of this repository.

---

## Disclaimer

Rebrowser is an independent data provider and is not affiliated with, endorsed by, or sponsored by AutoTrader. Any trademarks are the property of their respective owners. This dataset is compiled from publicly available information; we do not request or collect AutoTrader user credentials. By using this dataset, you agree to comply with AutoTrader's Terms of Service and all applicable laws and regulations. Images, logos, descriptions, and other materials included in this dataset remain the intellectual property of their respective owners and are provided solely for informational purposes. Rebrowser makes no warranties regarding the accuracy, completeness, or legality of the data and assumes no liability for how the data is used. You are solely responsible for ensuring that your use of this dataset does not infringe on the rights of any third party.


You can also find this data on [Kaggle](https://www.kaggle.com/datasets/rebrowser/autotrader-dataset), [HuggingFace](https://huggingface.co/datasets/rebrowser/autotrader-dataset), [Zenodo](https://doi.org/10.5281/zenodo.18715857).


