# Equipment Preparation

Up to 50 new 25 mm Whatman Glass Microfiber Filters (GF/F) (Fisher catalog number 09-874-64) were placed in a 25 ml glass beaker covered with double-layered aluminum foil and combusted at 450 degC for at least 4 hours. GF/Fs were never combusted more than once. Aluminum foil squares to make packets for sample storage were combusted at the same time as GFFs. 
Brown polycarbonate sample bottles were filled with 10% hydrochloric acid and soaked for at least 4 hours, then triple-rinsed with water purified using a Millipore Milli-Q lab water system (MilliQ), thoroughly dried, and capped. A freshly acid-washed bottle was used for each sample collected.

# CTD Rosette Bottle Sampling on NES-LTER cruises

Samples were collected from the water column at multiple depths using Niskin bottles on a CTD rosette system. Surface and subsurface chlorophyll max (SCM) were collected at all stations L1 through L11 and MVCO, with a third depth sometimes collected. Approximately 10% replicate samples were collected on each cruise to check sampling precision. For each sample, the sample bottle was triple rinsed with sample water and filled. Sample volume collected was a half liter for inshore stations and depths with high fluorescence signal, and 1 liter for offshore and/or deeper more dilute waters. 

# Filtering Protocol

For each sample, a known volume was filtered through a combusted GF/F filter under low vacuum suction (~5 in. Hg). Upon filtering completion, using gloves and dedicated clean forceps, each filter was carefully folded in half with particle side facing in and placed in a pre-labeled combusted foil packet. Samples were stored at -80 degC until further processing for analysis. 

# Sample Analysis 

Samples were transferred from the freezer to a 60 degC drying oven and left overnight, then stored in a desiccator until further processing. Wearing gloves on a clean work surface, the samples were folded into a 30 mm ultra clean tin disk (Part no. CE Elantech Inc 25208015) using clean forceps, compressed into a pellet, and stored in a clean well plate in a desiccator until analysis.

Samples were submitted to the Woods Hole Oceanographic Institution's Nutrient Analytical Facility (https://web.whoi.edu/nutrient/current-rates/) where they were analyzed using a Flash EA1112 CHN analyzer with the operational detection limit based on the lowest detectable value of the standard processed with each analyzed batch of samples. The CHN analyzer manufacturer states detection limits of 0.01% or 100 ppm for carbon and nitrogen. The instrument measured organic carbon and nitrogen using 4 pairs of thermal conductivity detectors after high temperature combustion and separation through chemical traps. Certified reference material Acetanilide (Certificate#293514) was combusted with every run and an average recovery was provided with the sample results. 

One or more blanks were collected from each combusted batch of GF/Fs per analysis batch. Blanks were put on the filter manifold to mimic standard filtering protocol, but no liquid was filtered. Blanks were then folded into a combusted foil packet and stored at -80 degC with the samples. Sometimes if blanks were not collected in the field, blanks were put into clean labeled polystyrene Petri dishes back on land after the field work and put into a dessicator. Blanks were pelletized using ultra clean tin disks as the same method for samples. 

# Data Calculations and Quality Control

The lab group made adjustments to account for volume filtered and corrected for blanks. Blank values were inspected, averaged, and subtracted from initial results. If in the event no blanks were analyzed for a batch of samples, blank values were estimated based on adjacent blank values. Blank-corrected molar values were divided by volume filtered for a final concentration in micromoles per liter. Carbon and nitrogen atomic weights were used to calculate mass in micrograms per liter. The carbon to nitrogen ratio is reported as a molar ratio. 

We provide columns in the data table to indicate quality for carbon and nitrogen values. These use IODE Primary Level flags 1 good; 2 not evaluated, not available or unknown; 3 questionable/suspect; 4 bad; 9 missing data; as well as, the additional flag of 6 below detection limit. Samples with a flag of 4 (bad) are provided with a value of NaN. The carbon to nitrogen ratio is set to NaN when the ratio is unable to be calculated (missing data, sample below detection limit, flagged bad values). Factors considered in quality control were magnitude of sample, the carbon to nitrogen ratio, and any additional notes during sample collection or sample analysis. For suspicious samples, CHN analyzer output of carbon and nitrogen peaks were manually inspected by the analytical lab, and some peak integrations were manually adjusted.

# Data Cleaning

All values below the batch detection limit were set to zero, and their quality flags were set to 6.
CTD bottle metadata (time, latitude, longitude, depth) were added from the REST Application Programming Interface (API) of the NES-LTER data system. 

# Data Package Assembly

Data package assembly with metadata templates was completed in R, with documentation available at https://github.com/WHOIGit/nes-lter-poc-transect

# Differences From Previous Version

Version 3 includes 5 more cruises as well as AR24A cast 1. Small adjustments to the methods write-up were made for version 3. 

# References

CE Instruments Flash EA 1112 CHN Analyzer Technical Manual. 1999.

M. Ehrhardt and W. Koeve. 1999. Determination of particulate organic carbon and nitrogen in Methods of Seawater Analysis (3rd edition), edited by K. Grasshoff, K. Kremling, and M. Ehrhardt. pp 437-444. Wiley. https://doi.org/10.1002/9783527613984.ch17

Sharp, J. H. 1974. Improved analysis for particulate organic carbon and nitrogen from seawater. Limnology and Oceanography, 19, 984-989.

