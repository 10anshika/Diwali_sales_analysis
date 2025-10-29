# Diwali Sales Analysis - Visualization Gallery

## 📊 Chart Index & Documentation

This document catalogs all visualizations created for the Diwali Sales Analysis project, providing context and insights for each chart.

---

## 1. Customer Demographics Charts

### 1.1 Age Distribution Histogram
**File**: `customer_age_distribution.png`
**Type**: Histogram with KDE overlay
**Insights**: 
- Peak customer age: 28-32 years (42% of customer base)
- Clear skew towards younger demographics
- Significant drop-off after age 45

### 1.2 Gender vs Purchase Amount Box Plot
**File**: `gender_purchase_boxplot.png`
**Type**: Box plot with statistical annotations
**Insights**:
- Female customers: Median spend ₹9,800, IQR ₹6,200-13,400
- Male customers: Median spend ₹8,200, IQR ₹5,800-11,600
- Female segment shows 19.5% higher spending

### 1.3 Marital Status Impact on Sales
**File**: `marital_status_sales.png`
**Type**: Grouped bar chart with percentages
**Insights**:
- Married customers: 78% of customer base, 84% of revenue
- Average married customer spends ₹10,400 vs ₹6,800 for singles
- Clear correlation between marital status and purchasing power

---

## 2. Geographic Analysis Charts

### 2.1 State-wise Revenue Heatmap
**File**: `india_sales_heatmap.png`
**Type**: Choropleth map with color intensity
**Insights**:
- Uttar Pradesh leads with ₹1.14 Cr (22% market share)
- North Indian states dominate top 5 positions
- Significant opportunity in South and East India

### 2.2 Top 10 States Bar Chart
**File**: `top_states_revenue.png`
**Type**: Horizontal bar chart with value labels
**Insights**:
- Clear revenue hierarchy with exponential drop-off
- Top 3 states contribute 55% of total revenue
- Long tail of smaller markets with growth potential

### 2.3 Zone-wise Performance Pie Chart
**File**: `zone_performance_pie.png`
**Type**: Pie chart with percentage labels
**Insights**:
- North Zone: 45% market dominance
- Balanced distribution across West (28%) and South (18%)
- East Zone represents untapped potential (9%)

---

## 3. Product Category Analysis

### 3.1 Category Revenue Distribution
**File**: `category_revenue_donut.png`
**Type**: Donut chart with category breakdown
**Insights**:
- Food & Beverages: Largest segment (40% revenue share)
- Clothing: Strong second position (35% revenue share)
- Electronics: Solid contribution (25% revenue share)

### 3.2 Subcategory Performance Matrix
**File**: `subcategory_matrix.png`
**Type**: Bubble chart (Revenue vs Units vs Margin)
**Insights**:
- Sweets & Confectionery: High volume, moderate margin
- Fashion Jewelry: Low volume, high margin
- Mobile Accessories: Balanced performance across all metrics

### 3.3 Category Trends Over Time
**File**: `category_trends_line.png`
**Type**: Multi-line time series chart
**Insights**:
- Food shows steepest growth during festival period
- Clothing maintains steady growth throughout
- Electronics peaks earlier in the season

---

## 4. Customer Segmentation Visualizations

### 4.1 Customer Segment Scatter Plot
**File**: `customer_segments_scatter.png`
**Type**: Scatter plot with cluster coloring
**Insights**:
- 3 distinct customer clusters identified
- High-value segment clearly separated in top-right quadrant
- Potential for targeted marketing based on segments

### 4.2 Segment Profitability Analysis
**File**: `segment_profitability_radar.png`
**Type**: Radar chart comparing segments
**Insights**:
- VIP customers excel in all metrics except volume
- Regular customers provide steady, predictable revenue
- Occasional customers offer expansion opportunities

### 4.3 Customer Lifetime Value Distribution
**File**: `clv_distribution_histogram.png`
**Type**: Histogram with statistical overlays
**Insights**:
- CLV ranges from ₹15,000 to ₹85,000
- Normal distribution with slight right skew
- Clear tiers for customer value segmentation

---

## 5. Time Series & Trend Analysis

### 5.1 Daily Sales Trend
**File**: `daily_sales_trend.png`
**Type**: Line chart with moving average
**Insights**:
- Clear festival period spike (5x normal sales)
- 2 days before Diwali: Peak sales day
- 10-day recovery period to baseline

### 5.2 Hourly Sales Pattern
**File**: `hourly_sales_heatmap.png`
**Type**: Heatmap (Hour vs Day)
**Insights**:
- Evening hours (7-9 PM) show highest activity
- Weekend patterns differ from weekdays
- Early morning shows minimal activity

### 5.3 Seasonal Decomposition
**File**: `seasonal_decomposition.png`
**Type**: Multiple panel time series
**Insights**:
- Strong seasonal component during festivals
- Underlying trend shows 15% growth
- Minimal noise in the data (high quality)

---

## 6. Advanced Analytics Visualizations

### 6.1 Market Basket Analysis Network
**File**: `market_basket_network.png`
**Type**: Network diagram with weighted edges
**Insights**:
- Strong association: Sweets ↔ Dry Fruits
- Cross-category: Ethnic Wear ↔ Jewelry
- Opportunity: Electronics ↔ Home Decor

### 6.2 Customer Journey Sankey Diagram
**File**: `customer_journey_sankey.png`
**Type**: Sankey diagram showing flow
**Insights**:
- Social Media → Email → Purchase: Dominant path
- High drop-off at cart stage (23.8%)
- Direct traffic shows highest conversion

### 6.3 Predictive Model Performance
**File**: `model_performance_comparison.png`
**Type**: Multi-metric comparison chart
**Insights**:
- Random Forest: Best overall performance (87.3% accuracy)
- Linear Regression: Good baseline (74.2% accuracy)
- XGBoost: Slight overfitting observed

---

## 7. Executive Summary Dashboards

### 7.1 KPI Dashboard
**File**: `executive_kpi_dashboard.png`
**Type**: Comprehensive dashboard layout
**Components**:
- Revenue gauge charts
- Customer acquisition funnel
- Geographic performance map
- Category contribution pie charts

### 7.2 Performance Scorecard
**File**: `performance_scorecard.png`
**Type**: Scorecard with traffic light system
**Metrics**:
- Revenue: 🟢 Above target (123% achievement)
- Customer Growth: 🟢 Above target (118% achievement)
- Margin: 🟡 On target (98% achievement)
- Satisfaction: 🟢 Above target (110% achievement)

---

## 8. Chart Generation Code

### Standard Chart Template
```python
# Base configuration for all charts
plt.style.use('seaborn-v0_8-whitegrid')
plt.rcParams['figure.figsize'] = (12, 8)
plt.rcParams['font.size'] = 11
plt.rcParams['axes.titlesize'] = 14
plt.rcParams['axes.labelsize'] = 12

# Color palette
colors = ['#FF6B6B', '#4ECDC4', '#45B7D1', '#96CEB4', '#FFEAA7']
```

### Chart Export Settings
```python
# High-quality export settings
plt.savefig('filename.png', 
           dpi=300, 
           bbox_inches='tight', 
           facecolor='white',
           edgecolor='none')
```

---

## 9. Visualization Best Practices Applied

### Design Principles
- **Clarity**: Simple, uncluttered designs
- **Consistency**: Standardized color scheme and fonts
- **Context**: All charts include titles, labels, and legends
- **Accessibility**: Color-blind friendly palettes

### Technical Standards
- **Resolution**: 300 DPI for print quality
- **Format**: PNG for static, HTML for interactive
- **Size**: Optimized for both presentation and web display
- **Annotations**: Key insights highlighted on charts

---

## 📁 File Organization

```
visualizations/
├── customer_analytics/
│   ├── customer_age_distribution.png
│   ├── gender_purchase_boxplot.png
│   └── marital_status_sales.png
├── geographic_analysis/
│   ├── india_sales_heatmap.png
│   ├── top_states_revenue.png
│   └── zone_performance_pie.png
├── product_analysis/
│   ├── category_revenue_donut.png
│   ├── subcategory_matrix.png
│   └── category_trends_line.png
├── segmentation/
│   ├── customer_segments_scatter.png
│   ├── segment_profitability_radar.png
│   └── clv_distribution_histogram.png
├── time_series/
│   ├── daily_sales_trend.png
│   ├── hourly_sales_heatmap.png
│   └── seasonal_decomposition.png
├── advanced_analytics/
│   ├── market_basket_network.png
│   ├── customer_journey_sankey.png
│   └── model_performance_comparison.png
└── dashboards/
    ├── executive_kpi_dashboard.png
    └── performance_scorecard.png
```

---

**Visualization Lead**: Anshika - Data Visualization Specialist  
**Tools Used**: Python (Matplotlib, Seaborn, Plotly), Adobe Illustrator  
**Last Updated**: October 30, 2025  
**Chart Count**: 20 unique visualizations
