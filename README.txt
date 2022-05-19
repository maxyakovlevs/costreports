***README FILE FOR USING $CHIME>MULTISTATE INPATIENT DATASETS FROM KELLOGG***
HCUP SID (State Inpatient Datasets) can be accesses via Kellogg upon request. Once the request
is approved, the researcher receives a link to the data host: \\ksmc15.kellogg.northwestern.edu\chime$.
The link is only accessible from within the Kellogg network.

Data host page organization: multistate inpatient datasets>`state'>raw//programs//dta

Multistate inpatient datasets contains 20 folders containing HCUP SID materials for 20 US states.

raw folders contain encrypted state-year .asc format data that can be transformed into Stata-friendly .dta format.
In order to achieve that, we have to utilize load programs.

SAS Files ready for extraction:
AZ - none
CO - 2011, 2014
MD - 2013,2014
NJ - 2014

programs folders include load program code files required to transform .asc format data to .dta and .sas format - .sas can be quickly translated into .dta. 
Also, available programs can be used for loading other years within the state.

Programs available(Stata):
CO-2011,2014
AZ-2011,2014
MD-2011,2014
NJ-2011,2014
**Note - 2011 program can be adjusted for 2012,2013 state-year datasets
Programs available - (SAS)
CO-2012,2013
AZ-2012,2013
NJ-2012,2013
MD-2012,2013

dta folders contain transformed .dta files that we can use if raw data is not readily available for some state-years.

1)Using .asc files from folder `state'>raw

2)Using load programs that are available from `state'>programs folder or HCUP website for 2014 from 
https://www.hcup-us.ahrq.gov/stataload/stataload_search.jsp
Result: .dta files that can be cleaned

3)Cleaning resulting .dta files using .do files we created.