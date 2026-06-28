# Chart Selection & UI Design Justification

## 1. Global UI/UX Philosophy (SaaS Dark Mode)
* **Design Principle Applied:** High Signal-to-Noise Ratio & Cognitive Ease.
* **Justification:** The dashboard is engineered using a modern `#121212` dark mode aesthetic with padded layout containers ("Cards"). This reduces eye strain, elevates the visual hierarchy of the neon data points, and forces the user's attention onto the metrics rather than the Tableau interface. Gridlines, axis rulers, and borders were ruthlessly removed to maximize Edward Tufte's "Data-Ink Ratio."

## 2. Sales Trend View
* **Question Answered:** How are sales fluctuating over time, and is there seasonal variance?
* **Chart Type:** Transparent Area Chart (Dual-Axis).
* **Design Principle:** While standard line charts are acceptable, an Area chart with 30% opacity anchors the data to the X-axis, providing a stronger visual "weight" to total volume. A secondary crisp line was overlaid to define the exact peaks.

## 3. Regional Performance View
* **Question Answered:** Which geographic areas drive the highest revenue and profit?
* **Chart Type:** Filled Map (Diverging Color Scale).
* **Design Principle:** Maps leverage spatial recognition. I applied a strict diverging color palette (Red to Green) centered precisely at `0`. This allows the executive to instantly spot unprofitable states (Red) without needing to read individual tooltips, avoiding the mistake of using meaningless categorical "rainbow" colors.

## 4. Customer Segment Breakdown
* **Question Answered:** Which segments drive our core business?
* **Chart Type:** Donut Chart.
* **Design Principle:** Standard pie charts are cognitively difficult to read and look dated. By layering a background-colored circle over a pie chart, I created a modern Donut chart. This achieves the part-to-whole comparison while keeping the aesthetic aligned with premium web applications.

## 5. Category & Sub-Category Profitability
* **Question Answered:** Which specific product lines are eroding our margins?
* **Chart Type:** Horizontal Bar Chart.
* **Design Principle:** Sorting allows for instant ranking. Coloring by margin rather than total profit exposes "volume traps"—sub-categories that sell high volumes but actually lose money. 

## 6. Discount vs. Profit Correlation
* **Question Answered:** Are heavy discounts cannibalizing our profits?
* **Chart Type:** Scatter Plot with Trend Line.
* **Design Principle:** Scatter plots are the mathematically correct visualization for observing correlations between two continuous variables. I avoided a line chart, which would falsely imply a sequential relationship.
