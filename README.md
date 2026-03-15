# Medicare-Project

**Team Member**: Emmanuel Ameh, Blessing Adeleye, Aly Boyd, Malsha Jayasinghe, Junqing Qian

## Dataset
Our main dataset is [Medicare Physician & Other Practitioners - by Provider
](https://data.cms.gov/provider-summary-by-type-of-service/medicare-physician-other-practitioners/medicare-physician-other-practitioners-by-provider) from the [Data.CMS.gov](https://data.cms.gov/) website. We will use data from 2013 to 2023 for this project.

## Backgrounds and Objectives
Medicare is the U.S. federal health insurance program primarily serving individuals aged 65 and older, as well as certain younger individuals with disabilities. Medicare Part B mainly covers outpatient and other medical services, including physician services, outpatient hospital care, many preventive services, durable medical equipment, ambulance services, some home health care, and certain limited outpatient prescription drugs, such as specific infusions. The cost of Medicare Part B has shown an upward trend over time, directly affecting beneficiaries. At the same time, providers are concerned with maintaining adequate equipment for patient care, appropriate staffing levels, and efficient scheduling, while the federal government seeks to control Medicare spending to preserve the program’s long-term sustainability and regulate drug costs.

In this project, we use Medicare provider datasets from 2013 through 2023 to predict future Medicare Part B total spending, specifically for 2024. Our modeling framework uses provider information from the previous year to predict spending in the current year, that is, a one-year lag structure. As a result, our analysis is restricted to providers that appear in two consecutive years of data. We use data from 2013 through 2022 for training and reserve 2023 for validation.

Our analysis does not attempt to account for current or historical policy changes that may influence Medicare costs, nor does it address incentives affecting pharmaceutical companies. In addition, we do not model geographic factors such as population size or urban versus rural status, although we do include state-level geographic features. We also do not incorporate beneficiaries’ diagnostic information or broader demographic characteristics.