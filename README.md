# PostgreSQL Data Model for FIFA 23 Complete Player Dataset

## Introduction

This is the step-by-step tutorial about how to construct Relational Data Model in PostgreSQL from large .csv files (~5GB, 10 millions rows).

## Source Data

- Source Dataset Url: [FIFA 23 Complete Player Dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-23-complete-player-dataset)

You can also use `dataset_downloader.sh` to download data in Unix-like environment (e.g. Ubuntu, MacOS). Below the file structures of data:

```
fifa-23-complete-player-dataset/
│
├── female_players.csv - 5.3K
├── male_players.csv   - 5.3G
│
├── female_players (legacy).csv - 1.7M
├── male_players (legacy).csv   - 87M
│
├── female_teams.csv - 2.2M
├── male_teams.csv   - 108M
│
├── female_coaches.csv - 5.3K
└── male_coaches.csv   - 130K
```