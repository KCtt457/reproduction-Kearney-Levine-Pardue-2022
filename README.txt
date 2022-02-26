*README for Kearney, Levine, Pardue (2021) "The Puzzle of Falling US Birth Rates Since the Great Recession"
*Updated 2/7/2022
*Project ID: openicpsr-144981

These files provide the underlying data to produce the figures, tables, and other statistics presented in Kearney, Levine, Pardue (2021).
 
0_setup.do will install all necessary STATA packages
main_prog.do will run all files below that produce all the .csv and .log files where results can be found. The outline below with detail which programs produce specific results. 

Programs Folder:

fig_1.do - reads in birth rates rates from CDC Final Births Reports to produce figure 1 - birth rates overall.
figs_2a_2b.do - reads in birth rates rates from CDC Final Births Reports to produce figures 2a and 2b - birth rates by mother's age group and birth rates by mother's race/ethnicity.
fig_2c.do - reads in births data from CDC WONDER and population data from the CPS to create figure 2c, births among hispanic women by nativity and mexican origin.
fig_2d.do - reads in aggregated births data and population data from the CPS to create figure 2d, births by mother's educational level.
fig_2e.do - reads in birth rate data from the CDC Final Births Reports to produce figures 2e - birth rates by marital status.
fig_2f.do - reads in aggregated births data and population from CDC SEER to create figure 2f, birth rates by parity.
fig_3.do - reads in aggregated births data and population from CDC SEER to create figure 3, a map displaying percent change in average birth rates from 2004-2008 to 2015-2018.
fig_4.do -  generates data presented in figure 4, relationship between changes in birth rates and potential explanatory factors, and that section. Relates changes in states birth rates (2004-2008 to 2015-2018) to changes in economic/social characteristics described in the data appendix. Produces scatterplot data, regression output, and presents average changes in economic/social x-variables over this time period.

sec_2_a_stats.do - uses ACS data to produce various statistics cited in section 2a: percent of hispanic women native-born, percent of women unmarried, and percent of women by education level.

table_1_population.do - calculates population bases of 63 age X education X race/ethnicity groups for table 1. Calculates population shares using CPS data, and applies these to total population counts from CDC SEER data.
table_1.do - creates table 1: largest groups contributing to birth rate decline. Merges CDC Wonder births data with annual CPS population counts of women across 63 age X education X race/ethnicity groups 

annual_regressions.do - generates statistics presented in Section 3a, annual regression of policy variables on birth rates from 15-44, using aggregated biths data, SEER population data, and policy variables described in data appendix.  


agecomp_seer.do - cleans CDC SEER single-age population estimates, 1969-2019, for use in cohort analysis.
age_race_comp_seer.do - cleans CDC SEER single-age by race/ethnicity estimates, 1990-2019, used as population base in calculating birth rates.
aggregate_nchs_microdata.do - (included for reference) cleans nhcs microdata used in estimating birth rates by education attainment, by hispanic origin and nativity, by parity, long-term regressions, and cohort analysis.
