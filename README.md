# IMuG: Iterative Mutual-Guidance for Traffic Forecasting

This repository provides information about the publicly available datasets used in our paper:

**Bridging Frequency and Time: Iterative Encoding with Mutual Guidance for Accurate Traffic Forecasting**

## Datasets

We evaluate IMuG on eight public traffic forecasting benchmarks, including four traffic-flow datasets and four traffic-speed datasets. All datasets contain traffic observations sampled at 5-minute intervals.

### Traffic-Flow Datasets

- PEMS03
- PEMS04
- PEMS07
- PEMS08

**Data source:** https://github.com/guoshnBJTU/ASTGNN/tree/main/data

### Traffic-Speed Datasets

- **METR-LA and PEMS-BAY:** https://github.com/liyaguang/DCRNN
- **PeMSD7(M):** https://github.com/VeritasYin/STGCN_IJCAI-18
- **LOOP_SEATTLE:** https://github.com/zhiyongc/Seattle-Loop-Data

## Experimental Settings

For all eight datasets, we use 12 historical time steps to predict the following 12 time steps. Traffic measurements are standardized using the training-set mean and standard deviation.

The chronological train/validation/test split ratios are:

- PEMS03, PEMS04, PEMS07, PEMS08: 6:2:2
- METR-LA, PEMS-BAY: 7:1:2
- PeMSD7(M), LOOP_SEATTLE: 6:2:2

For PeMSD7(M), prediction windows crossing Friday-to-Monday gaps are excluded.

## Data Availability

The datasets used in this study are publicly available from the original sources linked above. This repository provides a centralized index of these sources and does not redistribute the original datasets.
