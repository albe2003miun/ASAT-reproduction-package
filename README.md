# Reproduction Package for "Studying the Relationship between Architectural Smells and Maintainability"

This repository contains the reproduction package for the study "Studying the Relationship between Architectural
Smells and Maintainability". The main goal of this package is to facilitate the replication and verification of the results presented in the study.

## Contents

1. `expected_results/`: This directory contains the expected results. Each subdirectory represents a project and contains all the csv files for that project that were used in the study.

## How to Reproduce the Results

To reproduce the results of the study, please follow these steps:

1. Clone or download the source code of the Architectural Smell Analysis Tool (ASAT) from its original repository: [link to original repository](https://github.com/albe2003miun/ASAT).

2. Follow the instructions in the README of the ASAT repository to set up and configure the tool.

3. Ensure that you use the tool on the same projects that were used in the original study. The GitHub URLs of these projects are:
   - [Alibaba Sentinel](https://github.com/alibaba/Sentinel)
   - [Srikanth Lingala Zip4j](https://github.com/srikanth-lingala/zip4j)
   - [Networknt Light-4j](https://github.com/networknt/light-4j)
   - [Seata](https://github.com/seata/seata)
   - [LinShunKang MyPerf4J](https://github.com/LinShunKang/MyPerf4J)
   - [Weibocom Motan](https://github.com/weibocom/motan)
   - [Making Yavi](https://github.com/making/yavi)
   - [Sofastack Sofa-rpc](https://github.com/sofastack/sofa-rpc)


4. In the `config.properties` file (located at `src/constants/src/main/resources/config.properties`), replace the placeholder text in the `projectUrls` property with the URLs of the aforementioned projects, separated by a comma.

5. Run the main method of the Downloader module to download all snapshots needed.

6. Run the main method of the Analyzer module to analyze all snapshots and generate the CSV files.

7. Run the main method of the DataExtractor module to extract the relevant data.


After following these steps, the output of the tool should closely align with the results presented in the study. The results may vary
slightly depending on the user environment, and the inherent variability of the open-source projects.
