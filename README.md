# Optimising Airbnb Fee Structures to Maximise Host Revenue (Excel)

Excel-based analysis of Airbnb listings to recommend a host fee structure (nightly price, cleaning fees, extra guest fees, security deposits) that supports higher yearly revenue.

## Business problem
As an analyst working for Airbnb, the goal is to recommend a fee structure for hosts that maximises yearly revenue. Fees include:
- Nightly price
- Minimum nights
- Cleaning fees
- Security deposits
- Extra guest fees

## Dataset
- Airbnb listings dataset (Amsterdam region)
- ~14.9k listings after cleaning (14,884 rows) and 37 columns used for analysis

> Data source notes:
> - This project was completed using an Amsterdam Airbnb listings extract.  
> - If you are reproducing this project, use an Inside Airbnb extract for Amsterdam:
>   http://insideairbnb.com/get-the-data.html

## Tools
- Microsoft Excel (Power Query, PivotTables, PivotCharts)
- PowerPoint (stakeholder deck)

## Workflow
1. **Data cleaning & preparation**
   - Removed inactive listings, extreme price outliers, and unnecessary columns
   - Standardised data types and created derived features
   - Created binary flags for top amenities and category bands (price, capacity, bathroom count)

2. **Exploratory analysis**
   - Price distribution and market norms
   - Room type and guest capacity effects on nightly pricing
   - Bathroom count/type and impact on price
   - Amenity premiums (which features justify higher pricing)

3. **Recommendations**
   - Proposed baseline nightly prices by room type
   - Suggested cleaning fees scaled by bathroom count
   - Amenity premiums for high-value features (e.g., kitchen, washer, workspace)
   - Extra guest fees + security deposit scaling by property size

## Key findings
- Most active listings cluster around a mid-range nightly price band.
- Entire homes dominate the market and command higher nightly prices than private rooms.
- Bathroom count correlates strongly with price (2–3 bathrooms show large premiums).
- Certain amenities show meaningful price uplift (kitchen/washer/workspace).

## Recommendations
- Set nightly price baselines by room type, then adjust for capacity/bathrooms/amenities
- Increase cleaning fees with bathroom count (simple tiering)
- Add premiums for high-value amenities and implement extra guest fees
- Scale security deposits based on property size

## Repo contents
- `/deliverables/`  
  - Slide deck (final presentation)  
  - Excel workbook (cleaning log, analysis sheets, data dictionary, clean data)
- `/screenshots/`  

## How to view
1. Open the PowerPoint deck in `/deliverables/`
2. Open the Excel workbook in `/deliverables/`
   - Start with the **Data Handling Summary** sheet for cleaning rationale
   - Then review **Analysis & Charts** for pivots/visuals and insight captions

## Author
Jamie Tighe
