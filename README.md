# open-civic-datasets

A curated collection of verified open source government and civic datasets for exploration and community impact projects.

## Datasets Overview
This repository provides direct access to government datasets with working links, API endpoints, and documentation. All links verified September 2025.
<div align="center">

| **Category** | **Count** | **Key Sources** | **Geographic Scope** | ** % With API** |
|:---------------:|:------------:|:------------------:|:------------------------:|:-----------:|
| 🏥 **Health** | `8` | CDC PLACES • SVI | County → Census Tract | 100% |
| 🏠 **Housing** | `6` | HUD CHAS • Affordability | Tract → National | 100% |
| 🏛️ **Government** | `6` | 311 Requests • Federal | City → National | 100% |
| 🌍 **Environment** | `5` | NOAA • EPA AQI | Station → Global | 100% |
| 💰 **Economic** | `5` | BLS • BEA Statistics | County → National | 100% |
| 👥 **Demographics** | `5` | Census ACS • Decennial | Block → National | 100% |
| 🎓 **Education** | `4` | College Scorecard • IPEDS | Institution → National | 75% |
| 🚗 **Transportation** | `4` | DOT Stats • NYC Taxi | Route → National | 50% |
| 🚨 **Crime** | `2` | Gun Violence • Missing Persons | County → National | 50% |

**Total: 45 datasets across 9 domains • 🔧 37/45 with APIs (82%)**


</div>

## Complete Dataset Catalog

<details>
<summary><mark><strong>Click to expand full dataset table (45 datasets)</strong></mark></summary>

| Dataset Name | Category | Primary Link | Additional API or Data Link | Description | Geographic Levels | Update Frequency | Has API | Key Features | Record Count |
|:-------------|:---------|:-------------|:----------------------------|:------------|:------------------|:-----------------|:--------|:-------------|:-------------|
| CDC Social Vulnerability Index (SVI) | Health | https://www.atsdr.cdc.gov/place-health/php/svi/svi-data-documentation-download.html | https://svi.cdc.gov/data/ | 16 census variables measuring social vulnerability across 4 themes: socioeconomic status, household characteristics, racial/ethnic minority status, housing/transportation. Critical for emergency preparedness and health equity analysis. | National, State, County, Census Tract, ZIP Code | Biennial | Yes | Emergency preparedness, health equity, disaster response, vulnerability assessment, 4 vulnerability themes | 80,000+ census tracts |
| CDC PLACES Health Data - County | Health | https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb | https://data.cdc.gov/resource/swc5-untb.json | 40 health measures: 12 health outcomes, 7 preventive services, 4 risk behaviors, 7 disabilities, 3 health status, 7 social needs. Small area estimation for all US counties. | County | Annual | Yes | Chronic disease indicators, health outcomes, preventive care, community health assessment | 3,100+ counties |
| CDC PLACES Health Data - Census Tract | Health | https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-Census-Tract-D/cwsq-ngmh | https://data.cdc.gov/resource/cwsq-ngmh.json | Neighborhood-level health indicators for 83,522 census tracts. Same 40 health measures as county data but at granular neighborhood level. | Census Tract | Annual | Yes | Neighborhood health, environmental justice, health equity, community interventions | 83,522 census tracts |
| CDC PLACES Health Data - ZIP Code | Health | https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-ZCTA-Data-2024/qnzd-25i4 | https://data.cdc.gov/resource/qnzd-25i4.json | ZIP Code level health data covering 32,520 ZCTAs. Perfect for healthcare delivery planning and community health assessments. | ZIP Code | Annual | Yes | Healthcare planning, insurance analysis, community health centers, population health | 32,520 ZIP codes |
| CDC PLACES Health Data - Place Level | Health | https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-Place-Data-20/eav7-hnsx | https://data.cdc.gov/resource/eav7-hnsx.json | City and town level health data. Same 40 health measures for incorporated places and census designated places. | Place/City | Annual | Yes | Municipal health planning, city comparisons, local health departments | 29,923 places |
| CDC WONDER Mortality Data | Health | https://wonder.cdc.gov/ | https://wonder.cdc.gov/wonder/help/wonder-api.html | Death certificates, cause of death, mortality trends, age-adjusted death rates by geography and demographics. | National, State, County | Annual | Yes | Mortality analysis, public health surveillance, cause of death tracking | Millions of death records |
| CDC BRFSS Behavioral Risk Factors | Health | https://www.cdc.gov/brfss/annual_data/annual_data.htm | https://www.cdc.gov/brfss/data_tools.htm | Adult health behaviors, chronic disease prevalence, preventive service use from 400,000+ annual interviews. | National, State, Metro | Annual | Yes | Health behavior surveillance, risk factor monitoring, prevention planning | 400,000+ interviews/year |
| CDC Environmental Health Tracking | Health | https://ephtracking.cdc.gov/DataExplorer/ | https://ephtracking.cdc.gov/apihelp | Environmental health data linking environmental hazards with health outcomes. Air quality, water quality, climate. | National, State, County | Varies | Yes | Environmental health, climate health, exposure assessment | Varies by indicator |
| HUD CHAS Housing Affordability API | Housing | https://www.huduser.gov/portal/dataset/api-terms-of-service.html | https://www.huduser.gov/portal/dataset/chas-api.html | Comprehensive Housing Affordability Strategy data. Housing problems by income level (30%, 50%, 80% AMI), cost burden analysis. | National, State, County, City, Census Tract | Annual | Yes | Housing affordability, cost burden, HUD program eligibility, housing needs assessment | Millions of households |
| HUD CHAS Census Tract Data | Housing | https://hudgis-hud.opendata.arcgis.com/datasets/HUD::acs-5yr-chas-estimate-data-by-tract/about | https://services.arcgis.com/VTyQ9soqVukalItT/arcgis/rest/services/ | Census tract-level housing affordability and housing problems data. Essential for neighborhood-level housing analysis. | Census Tract | Annual | Yes | Neighborhood housing, local planning, community development, housing equity | 80,000+ census tracts |
| HUD Fair Market Rents | Housing | https://www.huduser.gov/portal/datasets/fmr.html | https://www.huduser.gov/portal/dataset/fmr-api.html | Section 8 Housing Choice Voucher payment standards and rental market analysis by metro area and county. | National, Metro Area, County, ZIP Code | Annual | Yes | Section 8 vouchers, rental market analysis, affordable housing development | 3,000+ areas |
| HUD Income Limits | Housing | https://www.huduser.gov/portal/datasets/il.html | https://www.huduser.gov/portal/dataset/fmr-api.html | Area median income calculations, housing program eligibility thresholds by geography. | National, State, County, Metro | Annual | Yes | Housing program eligibility, income qualification, affordable housing development | 3,000+ areas |
| HUD Physical Inspection Scores | Housing | https://www.huduser.gov/portal/datasets/pis.html |  | HUD's Real Estate Assessment Center physical property inspection results for HUD-owned, insured, or subsidized properties including public housing and multifamily assisted housing. Point-in-time property scores ensuring decent, safe, sanitary housing conditions. | National, State, County, Property | Annual | No | Property condition assessment, housing quality scores, compliance monitoring, property management | 20,000 inspections/year |
| American Housing Survey | Housing | https://www.census.gov/programs-surveys/ahs.html | https://www.census.gov/programs-surveys/ahs/data.html | Comprehensive national housing stock data: housing quality, costs, neighborhoods, demographics. | National, Metro | Biennial | Yes | Housing stock analysis, housing quality, neighborhood characteristics | 50,000+ housing units |
| Federal 311 Service Requests | Government | https://catalog.data.gov/dataset/?tags=311 |  | Non-emergency municipal service requests: potholes, graffiti, noise complaints, streetlight outages across cities. | City, Ward, District, Point | Daily | Yes | Municipal services, government efficiency, community needs, service delivery | Millions of requests |
| NYC 311 Service Requests | Government | https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9 |  | Real-time NYC service requests since 2010. Incident location, agency response times, complaint types. | City, Borough, Community Board, Point | Real-time | Yes | NYC services, agency performance, neighborhood patterns, emergency response | 30M+ requests |
| Chicago 311 Service Requests | Government | https://data.cityofchicago.org/Service-Requests/311-Service-Requests/v6vf-nfxy |  | Chicago service requests with location, type, status, response times since 2011. | City, Ward, Point | Daily | Yes | Chicago municipal services, response analysis, community needs | 5M+ requests |
| OpenFEMA Disaster Data | Government | https://www.fema.gov/about/openfema/api | https://www.fema.gov/about/openfema/developer-resources | Disaster declarations, individual assistance, public assistance, hazard mitigation grants, National Risk Index. | National, State, County, Tribal | Daily | Yes | Emergency management, disaster response, risk assessment, recovery programs | Millions of records |
| FEMA National Risk Index | Government | https://www.fema.gov/flood-maps/products-tools/national-risk-index | https://hazards.fema.gov/nri/ | Natural hazard risk assessment for all US counties and census tracts. 18 hazard types. | County, Census Tract | Annual | Yes | Risk assessment, emergency planning, community resilience, hazard mitigation | 70,000+ geographies |
| USA Spending Federal Contracts | Government | https://www.usaspending.gov/ | https://api.usaspending.gov/ | Federal spending, contracts, grants, direct payments with recipient and location data. | National, State, County, Recipient | Daily | Yes | Government spending analysis, contract tracking, transparency, economic impact | Millions of transactions |
| DOT Transportation Statistics | Transportation | https://data.transportation.gov/ | https://data.transportation.gov/browse?sortBy=relevance&page=1&pageSize=20 | Traffic safety, aviation data, freight movement, highway performance, transit ridership, infrastructure condition. | National, State, County, Route | Monthly | Yes | Transportation planning, infrastructure investment, safety programs, economic impact | Millions of records |
| NYC Taxi & Limousine Data | Transportation | https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page |  | Trip records since 2009: pickup/dropoff locations, trip distance, fare amounts for yellow/green taxis and FHV. | City, Borough, Taxi Zone | Monthly | No | Urban mobility, transportation demand, economic impact, traffic patterns | Billions of trips |
| GTFS Transit Data | Transportation | https://transitfeeds.com/ | https://developers.google.com/transit/gtfs | Public transit schedules, routes, stops, service patterns for transit agencies nationwide. | Agency, Route, Stop | Real-time | Yes | Transit planning, accessibility analysis, multimodal transportation | 1,000+ agencies |
| Highway Performance Monitoring | Transportation | https://www.fhwa.dot.gov/policyinformation/hpms.cfm | https://www.fhwa.dot.gov/policyinformation/hpms/shapefiles.cfm | Highway conditions, traffic volumes, pavement quality, bridge conditions by road segment. | National, State, County, Segment | Annual | No | Infrastructure planning, pavement management, traffic analysis | 4M+ road segments |
| NOAA Climate Data Records | Environment | https://www.ncei.noaa.gov/products/climate-data-records | https://www.ncei.noaa.gov/data/ | Long-term climate measurements: temperature, precipitation, ocean data, satellite observations spanning 30+ years. | Global, National, State, County, Station | Daily | Yes | Climate research, weather forecasting, agricultural planning, environmental monitoring | Billions of observations |
| EPA Air Quality Monitoring | Environment | https://www.epa.gov/outdoor-air-quality-data | https://aqs.epa.gov/aqsweb/documents/data_api.html | Air Quality Index, pollutant concentrations (PM2.5, ozone, NO2), health advisories, trends analysis. | National, State, County, Station | Hourly | Yes | Public health, environmental compliance, air quality forecasting, health impact | Millions of measurements |
| EPA Toxic Release Inventory | Environment | https://www.epa.gov/toxics-release-inventory-tri-program |  | Chemical releases and transfers from industrial facilities. Pollution prevention, waste management data. | National, State, County, Facility | Annual | Yes | Environmental compliance, pollution tracking, community health, industrial monitoring | 20,000+ facilities |
| USGS Water Data | Environment | https://waterdata.usgs.gov/nwis | https://waterservices.usgs.gov/ | Real-time and historical water data: streamflow, groundwater, water quality from monitoring stations. | National, State, County, Station | Real-time | Yes | Water resources, flood monitoring, drought assessment, water quality | 1.5M+ monitoring sites |
| NOAA Storm Events Database | Environment | https://www.ncdc.noaa.gov/stormevents/ | https://www.ncdc.noaa.gov/stormevents/ftp.jsp | Severe weather events: tornadoes, hurricanes, floods, with damage estimates and casualties. | National, State, County | Monthly | No | Disaster planning, insurance, climate research, emergency management | 1M+ events |
| Gun Violence Archive | Crime | https://www.gunviolencearchive.org/ | https://www.gunviolencearchive.org/methodology | Gun violence incidents, mass shootings, officer-involved shootings with casualty data. | National, State, County, City | Daily | No | Gun violence research, policy analysis, public safety | 60,000+ incidents/year |
| National Missing Persons Database | Crime | https://www.namus.gov/ | https://www.namus.gov/api/CaseSets | Missing persons cases, unidentified remains, unclaimed persons with demographic details. | National, State, County | Real-time | Yes | Missing persons investigations, cold cases, victim identification | 100,000+ cases |
| Census American Community Survey | Demographics | https://www.census.gov/data/developers/data-sets/acs-1year.html | https://api.census.gov/data/key_signup.html | Demographics, economics, housing, social characteristics. 1-year estimates (65k+ pop) and 5-year estimates (all areas). | National, State, County, City, Tract, Block Group | Annual | Yes | Demographic analysis, market research, policy planning, resource allocation | Millions of estimates |
| Census Decennial Census | Demographics | https://www.census.gov/data/developers/data-sets/decennial-census.html | https://api.census.gov/data/key_signup.html | Complete population and housing counts every 10 years with detailed demographic characteristics. | National, State, County, City, Tract, Block | Decennial | Yes | Population counts, redistricting, demographic baselines, historical trends | 300M+ people |
| Census Geographic Services | Demographics | https://geocoding.geo.census.gov/geocoder/ |  | Address geocoding, geographic boundary files, TIGER/Line shapefiles, coordinate conversion. | National, State, County, Tract, Block | Annual | Yes | Address standardization, geographic analysis, spatial mapping, GIS applications | Millions of addresses |
| Current Population Survey | Demographics | https://www.census.gov/data/datasets/time-series/demo/cps/cps-basic.html |  | Monthly labor force data, employment, unemployment, demographics, income, poverty. | National, State, Metro | Monthly | Yes | Labor statistics, employment trends, demographic monitoring | 60,000+ households/month |
| American Time Use Survey | Demographics | https://www.bls.gov/tus/ |  | How Americans spend their time: work, leisure, household activities, care giving by demographics. | National, Demographic Groups | Annual | Yes | Time use research, work-life balance, social policy, economic analysis | 10,000+ respondents/year |
| College Scorecard | Education | https://collegescorecard.ed.gov/data/ |  | Higher education outcomes: graduation rates, earnings, debt, demographics, completion rates by program. | National, State, Institution | Annual | Yes | College selection, higher education policy, institutional assessment, ROI analysis | 7,000+ institutions |
| IPEDS Higher Education Data | Education | https://nces.ed.gov/ipeds/use-the-data | https://nces.ed.gov/ipeds/datacenter/ | Comprehensive higher education data: enrollment, finances, staff, graduation rates, student aid. | National, State, Institution | Annual | No | Higher education research, institutional analysis, policy development | 6,000+ institutions |
| School & District Navigator | Education | https://www.nces.ed.gov/ccd/districtsearch/ | https://educationdata.urban.org/documentation/ | K-12 school and district characteristics: enrollment, demographics, finances, performance. | National, State, District, School | Annual | Yes | School research, district analysis, education policy, parent information | 130,000+ schools |
| Civil Rights Data Collection | Education | https://www2.ed.gov/about/offices/list/ocr/data.html | https://www2.ed.gov/about/offices/list/ocr/data.html | School discipline, access to courses, teacher equity, harassment and bullying data. | National, State, District, School | Biennial | No | Education equity, civil rights monitoring, discipline analysis | 100,000+ schools |
| Bureau of Labor Statistics API | Economic | https://www.bls.gov/developers/ | https://api.bls.gov/ | Employment statistics, wages, inflation (CPI), productivity, workplace injuries, occupational outlook. | National, State, Metro, County | Monthly | Yes | Economic analysis, labor market research, policy development, business planning | Millions of data points |
| Bureau of Economic Analysis API | Economic | https://apps.bea.gov/api/signup/ | https://apps.bea.gov/api/ | GDP, personal income, international trade, regional economic data, input-output accounts. | National, State, County, Metro | Quarterly | Yes | Economic forecasting, regional development, policy analysis, business intelligence | Millions of estimates |
| Census Business Dynamics | Economic | https://www.census.gov/data/developers/data-sets/business-dynamics.html |  | Business formation, job creation/destruction, establishment dynamics by industry and geography. | National, State, County, Metro | Annual | Yes | Entrepreneurship research, economic development, business lifecycle analysis | Millions of establishments |
| County Business Patterns | Economic | https://www.census.gov/data/developers/data-sets/cbp-nonemp-zbp.html |  | Business establishment counts, employment, payroll by industry and geography. | National, State, County, ZIP Code | Annual | Yes | Economic development, industry analysis, market research | 7M+ establishments |
| Quarterly Census Employment Wages | Economic | https://www.bls.gov/cew/ |  | Employment and wage data by industry, county, and ownership sector from unemployment insurance. | National, State, County, Industry | Quarterly | No | Local economic analysis, wage research, industry trends | 10M+ establishments |

</details>


## Download the Dataset Catalog as a Spreadsheet

**[Download Complete Dataset Catalog (Excel)](open-civic-datasets.xlsx)**

The spreadsheet contains all datasets organized by category with:
- Direct links to data sources
- API endpoints where available  
- Dataset descriptions and key features
- Geographic coverage levels
- Update frequencies

## Categories Included

- **Health & Public Health** - CDC health indicators, social vulnerability, environmental health
- **Housing & Real Estate** - HUD affordability data, fair market rents, housing conditions  
- **Government & Civic Services** - 311 requests, emergency management, federal spending
- **Transportation** - DOT statistics, transit data, traffic safety
- **Environment & Climate** - NOAA climate data, EPA monitoring, water resources
- **Public Safety** - local incident data
- **Demographics & Census** - Population data, economic indicators, geographic boundaries
- **Education** - School performance, higher education outcomes
- **Economic & Business** - Employment statistics, business data, economic indicators

## Key Datasets

- **CDC Social Vulnerability Index** - Community vulnerability assessment
- **HUD CHAS Housing Data** - Housing affordability by income level
- **CDC PLACES Health Data** - Health measures for all US communities
- **311 Service Requests** - Municipal service delivery tracking
- **OpenFEMA Disaster Data** - Emergency management information


## Additional Dataset Discovery Resources

### **Government Data Portals**
| **Portal** | **Focus** | **Key Features** |
|:-----------|:----------|:-----------------|
| **[Data.gov](https://data.gov/)** | Federal datasets | 300,000+ datasets across all agencies |
| **[Census.gov Data](https://data.census.gov/)** | Demographics & economics | Interactive data explorer, APIs |
| **[CDC Data & Statistics](https://www.cdc.gov/datastatistics/)** | Public health | Disease surveillance, health behaviors |
| **[NOAA Data.gov](https://data.noaa.gov/)** | Climate & weather | Real-time and historical climate data |
| **[NASA Open Data](https://data.nasa.gov/)** | Space & earth science | Satellite imagery, climate data |
| **[USGS Data Catalog](https://data.usgs.gov/)** | Earth sciences | Water, geology, natural hazards |

### **State & Local Government**
| **Portal** | **Coverage** | **Example Data** |
|:-----------|:-------------|:-----------------|
| **[Open Data Network](https://www.opendatanetwork.com/)** | Multi-jurisdictional | Unified search across 1,000+ portals |
| **[NYC OpenData](https://opendata.cityofnewyork.us/)** | New York City | 2,000+ datasets, real-time feeds |
| **[Chicago Data Portal](https://data.cityofchicago.org/)** | Chicago | 600+ datasets, APIs available |
| **[California Open Data](https://data.ca.gov/)** | California state | Budget, health, transportation |
| **[Texas Open Data](https://data.texas.gov/)** | Texas state | Education, criminal justice, health |
| **[DataSF](https://datasf.org/)** | San Francisco | 500+ datasets, data stories |

### **International & Global**
| **Portal** | **Scope** | **Key Datasets** |
|:-----------|:----------|:-----------------|
| **[World Bank Open Data](https://data.worldbank.org/)** | Global development | Economic indicators, poverty data |
| **[UN Data](http://data.un.org/)** | Global statistics | SDGs, population, environment |
| **[OECD Data](https://data.oecd.org/)** | Developed countries | Economic, social, environmental |
| **[European Data Portal](https://data.europa.eu/)** | European Union | 1M+ datasets from EU countries |
| **[Open Government Data](https://www.data.gov.uk/)** | United Kingdom | Government transparency data |
| **[Government of Canada Open Data](https://open.canada.ca/)** | Canada | Federal government datasets |

### **Academic & Research**
| **Platform** | **Specialization** | **Access** |
|:-------------|:-------------------|:-----------|
| **[Google Dataset Search](https://datasetsearch.research.google.com/)** | All domains | Free search engine for datasets |
| **[Kaggle Datasets](https://www.kaggle.com/datasets)** | Machine learning | Community-contributed datasets |
| **[Harvard Dataverse](https://dataverse.harvard.edu/)** | Research data | Peer-reviewed research datasets |
| **[ICPSR](https://www.icpsr.umich.edu/)** | Social sciences | Survey data, longitudinal studies |
| **[Zenodo](https://zenodo.org/)** | Open science | Research outputs, preprints |
| **[Registry of Open Data on AWS](https://registry.opendata.aws/)** | Cloud datasets | Large-scale public datasets |

### 🏢 **Private Sector & APIs**
| **Source** | **Type** | **Common Use Cases** |
|:-----------|:---------|:---------------------|
| **[Socrata Open Data](https://dev.socrata.com/)** | Government data platform | Municipal data APIs |
| **[Quandl](https://www.quandl.com/)** | Financial & economic | Market data, economics |
| **[OpenWeatherMap](https://openweathermap.org/api)** | Weather data | Current/forecast weather APIs |
| **[Reddit API](https://www.reddit.com/dev/api/)** | Social media | Posts, comments, community data |

## Contributing

Report broken links or suggest new datasets by opening an issue.
