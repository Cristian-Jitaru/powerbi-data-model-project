# powerbi-data-model-project
Power BI B2B data model cleaning and restructuring using Power Query, Star Schema implementation, DAX, and Row-Level Security (RLS).
Tool: POWER BI
Date preparation and clean-up: Power Query
Modeling Method: Star Schema
Calculations: DAX

Source Data Chanllenges:
Mismatched data types
Mixed granularity
Redundant fields

Solutions:

1. ETL & Data Cleaning: 
   * Formatted all primary/foreign keys and date columns.
   * Standardized column naming
   * Filtered out unnecessary columns to optimize file memory footprint.
2. Star Schema Implementation: 
   * Separated transactional events into Fact Tables (`fact_sales`).
   * Grouped descriptive context into Dimension Tables (`dim_date`, `dim_customer`, `dim_product`).
3. Relationship Management: 
   * Re-established active `1:*` (One-to-Many) single-direction relationships from Dimensions to Facts.
   * Fixed date dimension joins by aligning data types in Power Query.
  
Also created visuals based on the finished version of the data set and added Row Level Security
