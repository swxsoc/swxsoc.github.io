---
layout: default
---

The Space Weather Science Operations Center is a multi-mission science operations center for the community.

What can we do for you?

* Pipeline process data files
* Serve as a primary and backup data center
* Provide Cloud-based science data analysis environment
* Provide Graphical interfaces to monitor processing and viewing telemetry and science data
* Provide alerts for instrument anomalies and track instrument performance metrics over time
* Work with a Mission Operations Center to capture and forward telemetry and science data

Or we can support you to use our open source tools (see below).

# Supported Missions

The SWxSOC is currently supporting the following NASA missions

* Heliophysics Environmental and Radiation Measurement Experiment (HERMES), consists of 4 in-situ instruments.
* solar PolArization and Directivity X-ray Experiment (PADRE), consists of two solar-observing x-ray instruments.

# Tools

The SWxSOC processing Pipeline makes use of AWS. The following open source tools have been developed.
* **[swxsoc](https://github.com/swxsoc/swxsoc)** : A Python package  for core functionality of all SWxSOC mission packages.
* **[sammi](https://github.com/swxsoc/sammi)** : A Python package for shared attribute and metadata management interface for CDF files.
* **[hermes_instrument](https://github.com/HERMES-SOC/hermes_instrument)** : A Python package template for instrument packages.
* **[sdc_aws_pipeline_architecture](https://github.com/HERMES-SOC/sdc_aws_pipeline_architecture)** : AWS CDK code for the file processing pipeline architecture
* **[sdc_aws_sorting_lambda](https://github.com/HERMES-SOC/sdc_aws_sorting_lambda)** : AWS Lambda code for sorting files into the instrument buckets
* **[sdc_aws_processing_lambda](https://github.com/HERMES-SOC/sdc_aws_processing_lambda)** : AWS Lambda code for processing files in the instrument buckets
* **[sdc_aws_artifacts_lambda](https://github.com/HERMES-SOC/sdc_aws_artifacts_lambda)** : AWS Lambda code for generating artifacts such as slack notifications and timestream logs.
* **[sdc_aws_base_docker_image](https://github.com/HERMES-SOC/sdc_aws_base_docker_image)** : Docker image for the base image for the processing Lambda/Development containers
* **[MetaTracker](https://github.com/HERMES-SOC/MetaTracker)** :  A python package that helps track metadata of Raw Binary and Science Files in a Relational Database
* **[FSWatcher](https://github.com/HERMES-SOC/sdc_aws_fswatcher)** : A filewatcher system that can be configured to watch a directory for new files and then upload them to an S3 bucket.
* **[S3Watcher](https://github.com/HERMES-SOC/sdc_aws_s3watcher)** : A filewatcher system that can be configured to watch an AWS S3 bucket new files and then download them onto a local machine.
* **[sdc_aws_grafana_dashboard_backups](https://github.com/HERMES-SOC/sdc_aws_grafana_dashboard_backups)** : Backs up deployed dashboards as JSON models on https://grafana.hermes.swsoc.smce.nasa.gov/ daily

For more see the [SWxSOC organization page](https://github.com/swxsoc) and the [HERMES repository list](https://github.com/HERMES-SOC/).

# Presentations and Publications
* [DASH 2023](https://dash.heliophysics.net), Robbertz, Andrew, Rager, Amy C., Barrous-Dume, Damian, Skeberdis, Daniel, Christe, Steven, Kreisler, Steve, Mercer, Tony, & Paterson, William R. (2023). The Architecture and Functionality of HERMES Core and Instrument Python Packages. Zenodo. [https://doi.org/10.5281/zenodo.8400671](https://doi.org/10.5281/zenodo.8400671)
* [DASH 2023](https://dash.heliophysics.net), Damian Barrous-Dume, Amy Catherine Rager, Andrew Robbertz, Daniel Skeberdis, Steven Christe, Steve Kreisler, Tony Mercer, & William R Paterson. (2023, October 9). Open Science in Action: SWxSOC's Role in Accelerating Data Release and Cloud Processing for Heliophysics Missions. Zenodo. [https://doi.org/10.5281/zenodo.8408028](https://doi.org/10.5281/zenodo.8408028)
* [AGU 2023 (Fall Meeting)](https://agu.confex.com/agu/fm23/meetingapp.cgi/Paper/1401056), Robbertz, Andrew, Rager, Amy C., Barrous-Dume, Damian, Skeberdis, Daniel, Christe, Steven, Kreisler, Steve, Mercer, Tony, & Paterson, William R. (2023, December 4). HERMES Core and Instrument Python Packages. Zenodo. [https://doi.org/10.5281/zenodo.10257716](https://doi.org/10.5281/zenodo.10257716)
* [AGU 2023 (Fall Meeting)](https://agu.confex.com/agu/fm23/meetingapp.cgi/Paper/1355329), Damian Barrous-Dume, Amy Catherine Rager, Andrew Robbertz, Daniel Skeberdis, Steven Christe, Steve Kreisler, Tony Mercer, & William R Paterson. (2023, December 8). Open Science in Action: SWxSOC's Role in Accelerating Data Release and Cloud Processing for Heliophysics Missions. Zenodo. [https://doi.org/10.5281/zenodo.8408028](https://doi.org/10.5281/zenodo.8408028)
* [AGU 2024 (Fall Meeting)](https://agu.confex.com/agu/agu24/meetingapp.cgi/Paper/1623653), Damian Barrous-Dume, Amy Catherine Rager, Andrew Robbertz, Daniel Skeberdis, Steven Christe, Steve Kreisler, Tony Mercer, & William R Paterson. (2023, December 8). Enhancing SWxSOC through Open Collaboration for Multi-Mission Data Processing and Expedited Release. Zenodo. [https://doi.org/10.5281/zenodo.14536415](https://doi.org/10.5281/zenodo.145364158)
* [AGU 2024 (Fall Meeting)](https://agu.confex.com/agu/agu24/meetingapp.cgi/Paper/1569918), Robbertz, Andrew, Rager, Amy C., Barrous-Dume, Damian, Skeberdis, Daniel, Christe, Steven, Kreisler, Steve, Mercer, Tony, & Paterson, William R. (2024, December 4). SWxSOC Software Architecture for Science Data Processing. Zenodo. [https://zenodo.org/records/14606063](https://zenodo.org/records/14606063)
* [AGU 2025 (Fall Meeting) - IN33E-0396 Enhancing SWxSOC through Open Collaboration for Multi-Mission Data Processing and Expedited Release](https://agu.confex.com/agu/agu25/meetingapp.cgi/Paper/1958604) [https://zenodo.org/records/18600838](https://zenodo.org/records/18600838)
* [AGU 2025 (Fall Meeting) - IN33E-0400 Standardizing and validating Solar Datasets, the SOLARNET project](https://agu.confex.com/agu/agu25/meetingapp.cgi/Paper/1910471) [https://zenodo.org/records/18600752](https://zenodo.org/records/18600752)

# Contact Us
For more information contact [steven.christe@nasa.gov](mailto:steven.christe@nasa.gov).
