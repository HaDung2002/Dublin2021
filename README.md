# Dublin2021
A Dataset for Traffic Prediction

Traffic flow data are collected from the website Transport Infrastructure Ireland Traffic Data (https://trafficdata.tii.ie/). Dataset contains traffic volume extracted from 33 traffic counters located in the center of Dublin, Ireland. The time period used is from 1/1/2021 to 31/12/2021 and the time interval is 5 minutes. This dataset can be applied to traffic prediction problems, especially using GNN-based approaches.

## Data structure
Dublin2021 contains multiple data files related to spatial and temporal features of traffic flow
<ol>
  <li>
    <code>./raw/</code> contains raw traffic flow data in <code>.xls</code> format. The structure of folder <code>./raw/</code> is as follows, with each sub-folder is data collected from a traffic counter, each folder contains 12 <code>.xls</code> files corresponding to each month in 2021.
      <pre><code>
      raw/
      |
      ├── TMU M01 000.0 N/
      │ └── 2021 (1).xls
      │ └── 2021 (2).xls
      │ └── ...
      ├── TMU M01 000.0 N/
      │ └── 2021 (1).xls
      │ └── 2021 (2).xls
      │ └── ...
      ├── ...
      </code></pre>
  </li>
  <li>
    <code>adj_matrix.csv</code> is the weighted adjacency matrix of the shape [33, 33]. The value at i-th row and j-th column is the road distance from counter i to counter j.
  </li>
  <li>
    <code>counter_information.csv</code> contains the mapping index, longitude and latitude of each traffic counter.
  </li>
  <li>
    <code>distances.csv</code> contains information about road distance from one traffic counter to another.
  </li>
  <li>
    <code>traffic_flow.csv</code> has 34 columns, the first one is <code>datetime</code> and the remaining represents traffic flow recorded at each counter every 5 minutes from 1/1/2021 to 31/12/2021.
  </li>
</ol>


