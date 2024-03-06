## The ESA CIMR L2PAD project

The Level-2 Product Algorithm Development (L2PAD) project is a four-years activity initiated by the
European Space Agency (ESA) to prepare Level-2 algorithms and Ground Processing Prototype (GPP) for
the Copernicus Imaging Microwave Radiometer (CIMR) mission.

<img src="./profile/static_imgs/CIMRL2PAD_logo_blue_lite.png" alt="The CIMR L2PAD logo" width="512" class="center">

The CIMR L2PAD project is implemented by a consortium of European and Canadian partners, under the
lead of the Norwegian Meteorological Institute (METNO). CIMR L2PAD started in November 2023, and
is initially planned to last four years (2023-2027).

All software, data, and algorithm documentations from CIMR L2PAD will be open, in particular the 
Algorithm Theoretical Basis Documents (ATBDs) and the Level-2 prototype algorithms and GPP.

This page serves as a public entry-point for the project and its results. It will be developed further as results
are available. Repositories holding the ATBDs and prototype algorithms will be available at the bottom of this page.

### The CIMR L2PAD community: interacting with us

We are looking forward to creating a welcoming, supportive and diverse community of enthusiasts, experts, and users
around the the Copernicus Imaging Microwave Radiometer (CIMR) satellite mission. The primary focus of this community
is to develop and improve algorithms and prototype ground-processing software for the CIMR Level-2 products.

We do not have much to share at this point, but do not hesitate to contact us while we get started 😅.

At this stage, we are not ready to answer detailed questions about the algorithms we will use, nor how the Level-2 products
from the CIMR L2 GPP will look like. We are also not ready to take on board community contributions.

But this time will eventually come, so please visit our [Discussions page](https://github.com/orgs/CIMR-L2PAD/discussions) to say
'hi', ask your questions, and stay informed about our progress.

*Important:* This is a community we build together. Please be welcoming, open minded, and respectful in your interactions, and adhere
to our [code of conduct](./CODE_OF_CONDUCT.md).

### Level-2 variables covered by CIMR L2PAD

The CIMR L2PAD project focuses on Level-2 products under ESA's operational responsibility, that is
Level-2 products in the *Polar Oceans* (incl. sea ice) and *Global Land* (incl. lakes) family. The
*Global Oceans* and *Atmosphere* products are not covered, as they are under EUMETSAT's operational
responsibility.

The table below lists the Level-2 products that are covered by the CIMR L2PAD team (-P: Polar Oceans, -L: Global Land).

Depending on the Level-2 product, different delivery timeliness are specified:
* *Near-Real-Time-3-Hour (NTR3H)*: Product delivered in <3 hour to the point of user pickup after data acquisition by
   the satellite. This is the nominal timeliness for the Copernicus Space Component.
* *Near-Real-Time-1-Hour (NRT1H)*: Product delivered in <1 hour to the point of user pickup after data acquisition by
   the satellite. In the case of CIMR, NRT1H targets support to safe Arctic navigation.
* *Non-Time-Critical (NTC)*: Product delivered in less than 30 days to the point of user pickup after data acquisition by
   the satellite.

`MRD-XXXX` refers to the requirement number in the [CIMR Mission Requirement Document v5](https://esamultimedia.esa.int/docs/EarthObservation/CIMR-MRD-v5.0-20230211_(Issued).pdf).

| L2 Variable ID | Description | Coverage Domain | Delivery Timeliness | MRD-XXXX |
| ---            | ---         | ---             | ---                 | ---      |
| SIC-P | Sea Ice Concentration | Polar Regions and Adjacent Seas | NRT1H/NRT3H/NTC | MRD&#8209;890, MRD&#8209;1110 |
| SIT-P | Thin Sea Ice Thickness | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;910 |
| SIED-P | Sea Ice Edge | Polar Regions and Adjacent Seas | NRT1H/NRT3H/NTC | MRD&#8209;915, MRD&#8209;1110 |
| SID-P | Sea Ice Drift | Polar Regions and Adjacent Seas | NRT1H/NRT3H/NTC | MRD&#8209;920, MRD&#8209;1110 |
| ITY-P | Ice stage of development / type | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;930 |
| SND-P | Snow Depth on Sea Ice | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;940 |
| SIST-P | Sea Ice Surface Temperature | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;970 |
| SST-P | Sea Surface Temperature | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;905 |
| SSS-P | Sea Surface Salinity | Polar Regions and Adjacent Seas | NRT3H/NTC | MRD&#8209;985 |
| OWV-P | Ocean Surface Wind Vector | Polar Regions and Adjacent Seas | NRT3H/NTC (+ Speed as NRT1H) | MRD&#8209;995, MRD&#8209;1110 |
| TSA-L | Terrestrial Snow Area | Global land | NRT3H/NTC | MRD&#8209;950 |
| SWE-L | Terrestrial Snow Water Equivalent | Global land | NRT3H/NTC | MRD&#8209;960 |
| LIC-L | Lake Ice Cover | Global land according to Hydrology mask | NRT3H/NTC | MRD&#8209;1010 |
| FT-L | Soil Freeze/thaw state | Global land | NRT3H/NTC | MRD&#8209;1020 |
| SM-L | Soil Moisture | Global land | NRT3H/NTC | MRD&#8209;1040 |
| MMVI-L | Multi-frequency Microwave Vegetation Indicators | Global land | NRT3H/NTC | MRD&#8209;1050 |
| SWF-L | Surface Water Fraction | Global land | NRT3H/NTC | MRD&#8209;1060 |
| LSWT-L | Lake Surface Water Temperature | Global land according to Hydrology mask | NRT3H/NTC | MRD&#8209;1000 |
| LST-L | Land Surface Temperature | Global land | NRT3H/NTC | MRD&#8209;1030 |

### The CIMR mission

CIMR is the Copernicus Imaging Microwave Radiometer mission, a multi-frequency, conically-scanning passive microwave imager
designed by ESA to support EU's Arctic Policy, among others. Its launch is scheduled in 2029.
More info about CIMR [here](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Copernicus_Sentinel_Expansion_missions).

![CIMR in flight (artist view, credit: ESA/mlabspace)](./profile/static_imgs/CIMR_inflight.jpg)

ESA has prepared videos introducing the mission, find them [here](https://www.esa.int/esatv/content/search?SearchText=CIMR&result_type=videos_broadcast&SearchButton=Go).

The [CIMR Mission Requirement Document v5](https://esamultimedia.esa.int/docs/EarthObservation/CIMR-MRD-v5.0-20230211_(Issued).pdf) is available online.

### The CIMR L2PAD team

The CIMR L2PAD project is implemented by a consortium of European and Canadian partners, under the
lead of the Norwegian Meteorological Institute (METNO). CIMR L2PAD started in November 2023, and
is initially planned to last four years (2023-2027).

![The CIMR L2PAD consortium](./profile/static_imgs/CIMRL2PAD_Consortium_Logos.png)


This webpage was developed in the context of the ESA-funded CIMR L2PAD project (2023-2027) (ESA 4000143081/23/I-NS).
