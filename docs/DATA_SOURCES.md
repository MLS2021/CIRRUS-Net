# Data Sources, Citations, and Usage Terms

This document records the provenance of the datasets used in the CIRRUS-Net study. The statements below summarize the terms published by the original providers; they do not replace the upstream licenses or legal notices.

## 1. SpaceNet 6 Expanded Dataset

- **Use in this study:** primary high-resolution benchmark; RGB optical imagery, four-channel HH/HV/VH/VV SAR intensity imagery, and building-footprint annotations from AOI 11 Rotterdam.
- **Official source:** [SpaceNet 6: Multi-Sensor All-Weather Mapping](https://www.spacenet.ai/sn6-challenge/)
- **Data access:** `s3://spacenet-dataset/AOIs/AOI_11_Rotterdam/`
- **Provider-stated license:** [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)
- **Citation:** Shermeyer et al., *SpaceNet 6: Multi-Sensor All-Weather Mapping Dataset*, CVPR Workshops, 2020. [DOI: 10.1109/CVPRW50498.2020.00106](https://doi.org/10.1109/CVPRW50498.2020.00106)

The degradation preview in this repository is based on a modified SpaceNet 6 optical patch. SpaceNet 6 ownership and attribution remain with the SpaceNet Partners.

## 2. HRC_WHU Cloud Dataset

- **Use in this study:** real cloud appearance and expert cloud masks are used to construct spatial cloud-opacity patterns for synthetic optical degradation.
- **Official source:** [HRC_WHU: High-Resolution Cloud Detection Dataset](https://github.com/dr-lizhiwei/HRC_WHU)
- **Dataset description:** 150 high-resolution RGB images collected from Google Earth over five land-cover categories, with cloud masks digitized by remote-sensing experts at Wuhan University.
- **Provider-stated usage term:** the official repository states that the dataset is shared **for academic purposes only**. It does not provide a standard open-data license file.
- **Citation:** Li et al., *Deep learning based cloud detection for medium and high resolution remote sensing images of different sensors*, ISPRS Journal of Photogrammetry and Remote Sensing, 2019. [DOI: 10.1016/j.isprsjprs.2019.02.017](https://doi.org/10.1016/j.isprsjprs.2019.02.017)

The original HRC_WHU images and masks are **not redistributed** in this repository. The four preview images contain processed cloud effects derived for academic demonstration. They are not covered by a source-code license and must not be treated as a replacement for the original HRC_WHU dataset.

## 3. Copernicus Sentinel-1 and Sentinel-2

- **Use in this study:** Sentinel-1 VV/VH annual median composites and Sentinel-2 B2/B3/B4/B8 annual median composites provide the cross-region transfer data.
- **Official access and legal terms:** [Copernicus Sentinel Data Legal Notice](https://cds.climate.copernicus.eu/licences/ec-sentinel)
- **Usage summary:** Copernicus provides free, full, and open access for lawful reproduction, distribution, communication, adaptation, modification, and combination.
- **Required source notice for modified products:** `Contains modified Copernicus Sentinel data [Year].`
- **Sentinel-1 citation:** Torres et al., *GMES Sentinel-1 Mission*, Remote Sensing of Environment, 2012. [DOI: 10.1016/j.rse.2011.05.028](https://doi.org/10.1016/j.rse.2011.05.028)
- **Sentinel-2 citation:** Drusch et al., *Sentinel-2: ESA's Optical High-Resolution Mission for GMES Operational Services*, Remote Sensing of Environment, 2012. [DOI: 10.1016/j.rse.2011.11.026](https://doi.org/10.1016/j.rse.2011.11.026)

## 4. ESA WorldCover 2021

- **Use in this study:** WorldCover 2021 built-up class is converted to a binary built-up-area mask for the 10 m cross-region experiment.
- **Official source:** [ESA WorldCover data access](https://esa-worldcover.org/en/data-access)
- **License:** [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)
- **Citation:** Zanaga et al., *ESA WorldCover 10 m 2021 v200*, 2022. [DOI: 10.5281/zenodo.7254221](https://doi.org/10.5281/zenodo.7254221)
- **Provider attribution:** `© ESA WorldCover project 2021 / Contains modified Copernicus Sentinel data (2021) processed by ESA WorldCover consortium.`

## Redistribution Boundary

This preview repository provides only a small number of derived visual examples and research figures. It does not host the complete SpaceNet 6, HRC_WHU, Sentinel, or WorldCover datasets. Users must obtain the original datasets from their respective providers and comply with the corresponding licenses, legal notices, attribution requirements, and usage restrictions.

