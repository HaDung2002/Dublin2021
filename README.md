# Dublin2021
A Dataset for Traffic Prediction

Traffic flow data are collected from the website Transport Infrastructure Ireland Traffic Data (https://trafficdata.tii.ie/). Dataset contains traffic volume extracted from 33 traffic counters located in the center of Dublin, Ireland. The time period used is from 1/1/2021 to 31/12/2021 and the time interval is 5 minutes. This dataset can be applied in trafffic prediction problem, especially using GNN-based approaches.

## Data structure
The structure of dataset is as follows

Dublin2021/
|
├── raw/
│ ├── TMU M01 000.0 N/
│ └── 2021 (1).xls
│ └── 2021 (2).xls
│ └── ...
│ ├── TMU M01 000.0 N/
│ └── 2021 (1).xls
│ └── 2021 (2).xls
│ └── ...
│ ├── ...
|
└── adj_matrix.csv
│
└── counter_information.csv
|
└── distances.csv
|
└── traffic_flow.csv
