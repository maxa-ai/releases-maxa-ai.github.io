# Analyst Hub: Marts & Dashboard Builder - Release Notes

## Release Overview

The Analyst Hub is a new tool for business analysts designed to integrate data structuring and visualization needs into a cohesive platform. With its Mart Builder, users can create customized data subsets by selecting specific data sources and applying transformations like filtering and aggregation. The Dashboard Builder allows them to craft personalized visualizations, connect data marts to dashboard tabs, and implement filter options for refined data insights.

## Key Features

### Mart Builder

- **Data Subset Creation**: Initiate the mart-building process by selecting a data source based on a specific business activity or by utilizing an existing mart.

  - _Example: Source Selection_
      <p align="center">
        <img src="/analyst_hub/image0.png" alt="Add Source Button" width="70%" />
        <p>Add Source Button</p>
        <img src="/analyst_hub/image1.png" alt="Edit Source Modal" width="70%" />
        <p>Edit Source Modal</p>
        <img src="/analyst_hub/image2.png" alt="Edit Source Preview" width="70%" />
        <p>Edit Source Preview</p>
        <img src="/analyst_hub/image3.png" alt="Add Source Result" width="70%" />
        <p>Add Source Result</p>
        <img src="/analyst_hub/image4.png" alt="Select Column Action" width="70%" />
        <p>Select Column Action</p>
        <img src="/analyst_hub/image5.png" alt="Add Column Result" width="70%" />
        <p>Add Column Result</p>
      </p>

- **Data Transformations**: Apply various transformations to your mart:
  - **Filtering**: Narrow down data to meet criteria relevant to your business needs.
  - **Aggregation**: Consolidate data for easier analysis and reporting.
  - _Example: Transformations_
      <p align="center">
        <img src="/analyst_hub/image6.png" alt="Open the Transformation Modal" width="40%" />
        <p>Open the Transformation Modal</p>
        <img src="/analyst_hub/image7.png" alt="Select your Transformation Type" width="60%" />
        <p>Select your Transformation Type</p>
      </p>
      
      For Filters
      <p align="center">
        <img src="/analyst_hub/image8.png" alt="Select your Column to filter, your operator and your operand" width="60%" />
        <p>Select your Column to filter, your operator and your operand</p>
      </p>
      
      For Aggregation
      <p align="center">
        <img src="/analyst_hub/image9.png" alt="Select the dimensions to Group, the aggregation function and the column to aggregate" width="60%" />
        <p>Select the dimensions to Group, the aggregation function and the column to aggregate</p>
        <img src="/analyst_hub/image10.png" alt="Use layers to modify the order in which transformations are applied to your data" width="60%" />
        <p>Use layers to modify the order in which transformations are applied to your data</p>
      </p>

### Dashboard Builder

- **Visualization Creation**: Start by linking a mart to your dashboard tab. While one mart per tab is allowed, there are no limits to the number of tabs.

  - _Example: Mart Connection_
      <p align="center">
        <img src="/analyst_hub/image11.png" alt="image.png.p" width="40%" />
        <p></p>
        <img src="/analyst_hub/image12.png" alt="image.png" width="60%" />
        <p></p>
        <img src="/analyst_hub/image13.png" alt="image.png" width="60%" />
        <p></p>
      </p>

  - _Example: Add Visualization_
      <p align="center">
        <img src="/analyst_hub/image14.png" alt="image.png" width="15%" />
        <p></p>
        <img src="/analyst_hub/image15.png" alt="image.png" width="80%" />
        <p></p>
        <img src="/analyst_hub/image16.png" alt="image.png" width="80%" />
        <p></p>
        <img src="/analyst_hub/image17.png" alt="image.png" width="80%" />
        <p></p>
        <img src="/analyst_hub/image18.png" alt="image.png" width="80%" />
        <p></p>
      </p>

- **Customizable Filters**: Enhance your visual dashboards with:

  - **Tab Filters**: Apply specific conditions to all visualizations within a tab.

    - _Example: Tab Filter_
        <p align="center">
          <img src="/analyst_hub/image25.png" alt="image.png" width="40%" />
          <p></p>
          <img src="/analyst_hub/image19.png" alt="image.png" width="60%" />
          <p></p>
          <img src="/analyst_hub/image26.png" alt="image.png" width="60%" />
          <p></p>
          <img src="/analyst_hub/image20.png" alt="image.png" width="60%" />
          <p></p>
          <img src="/analyst_hub/image21.png" alt="image.png" width="60%" />
          <p></p>
        </p>

  - **Global Filters**: Impose universal conditions across the dashboard to maintain consistent data views.
    - _Example: Global Filter_
        <p align="center">
          <img src="/analyst_hub/image22.png" alt="image.png" width="40%" />
          <p></p>
        </p>

- **Multi-tab Support**: Cater to a wide array of analytical needs by creating multiple tabs, each with its unique data mart and visualizations.
  - _Example: Multi-tab_
      <p align="center">
        <img src="/analyst_hub/image23.png" alt="image.png" width="90%" />
        <p></p>
        <img src="/analyst_hub/image24.png" alt="image.png" width="60%" />
      </p>
