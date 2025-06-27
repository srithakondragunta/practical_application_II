# Key Insights on Used Car Price Drivers

## Overview

Following the development and evaluation of several regression models, the **Random Forest Model** was selected as the most accurate, achieving an **R² score of 0.9885**. This model captures nearly all variability in used car prices, offering reliable, data-driven insights into what truly drives vehicle value in the market. This report outlines the most important features influencing price and translates these findings into actionable strategies for inventory management, pricing, and customer targeting.

---

## Top 10 Most Influential Features

| Rank | Feature                    | Importance |
|------|----------------------------|------------|
| 1    | `price_per_mile`           | 0.8786     |
| 2    | `odometer`                 | 0.0398     |
| 3    | `interaction_age_mileage` | 0.0397     |
| 4    | `mileage_per_year`        | 0.0235     |
| 5    | `drive_fwd`               | 0.0117     |
| 6    | `cylinders`               | 0.0012     |
| 7    | `car_age`                 | 0.0011     |
| 8    | `age_squared`             | 0.0010     |
| 9    | `year`                    | 0.0010     |
| 10   | `is_luxury`               | 0.0005     |

---

## Insights & What Buyers Value

### 1. `price_per_mile` (Most Dominant Feature)  
This engineered metric overwhelmingly influences pricing. It reflects the balance between vehicle cost and usage, suggesting that **buyers are highly sensitive to perceived value based on mileage efficiency**. Cars that are priced high relative to their mileage are penalized by the model.

### 2–4. `odometer`, `interaction_age_mileage`, `mileage_per_year`  
These highlight how **total mileage and its relationship to vehicle age** factor into pricing. Higher mileage generally reduces value, especially when it exceeds what would be expected for the car’s age. Even if a car is older, low yearly mileage increases value.

### 5. `drive_fwd`  
Front-wheel drive cars appear slightly favored—likely due to better fuel efficiency, lower maintenance costs, and reliability in most driving conditions.

### 6–9. Engine & Age-related Features (`cylinders`, `car_age`, `age_squared`, `year`)  
These features reflect gradual depreciation and buyer preferences for newer vehicles or specific engine sizes, though their individual impact is small compared to mileage-based metrics.

### 10. `is_luxury`  
Surprisingly, being labeled a luxury vehicle contributes less than expected, suggesting that **mileage and efficiency outweigh luxury branding** in the broader used car market.

---

## Recommendations for Dealers

- **Prioritize Efficient, Low-Mileage Vehicles**  
  Stock cars with strong price-per-mile performance. Avoid vehicles with high mileage relative to their age unless deeply discounted.

- **Use Custom Value Metrics in Pricing Tools**  
  Go beyond traditional pricing tools by incorporating `price_per_mile` and `mileage_per_year` into pricing decisions.

- **Educate Buyers with Value Comparisons**  
  Highlight cost-efficiency in listings (e.g., "Only $0.18 per mile!")—this resonates with how buyers assess value, consciously or not.

- **De-emphasize ‘Luxury’ When Stocking Inventory**  
  Unless luxury vehicles show strong value metrics, they may not return higher margins than standard vehicles with better mileage profiles.

---

