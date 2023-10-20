# EDA-with-SQL-covid-data

## COVID-19 Data Exploration 

This repository contains SQL queries used for exploring COVID-19 data. The queries utilize various SQL skills, including Joins, Common Table Expressions (CTE), Temporary Tables, Window Functions, Aggregate Functions, and creating Views. The data used in these queries is sourced from the `PortfolioProject..CovidDeaths` and `PortfolioProject..CovidVaccinations` tables.

## Queries Explanation

### Query 1: Selecting Data for Analysis
This query selects data from the `CovidDeaths` table, filtering records where the continent is not null, and orders the results by the third and fourth columns.

### Query 2: Initial Data Selection
This query selects specific columns (Location, Date, Total Cases, New Cases, Total Deaths, Population) from the `CovidDeaths` table, filtering records where the continent is not null, and orders the results by location and date.

### Query 3: Total Cases vs Total Deaths
This query calculates the death percentage based on total cases and total deaths for locations containing the field 'india'.

### Query 4: Total Cases vs Population
This query calculates the percentage of the population infected with COVID-19 for each location.

### Query 5: Countries with Highest Infection Rate per Population
This query identifies countries with the highest infection rate compared to their population.

### Query 6: Countries with Highest Death Count
This query identifies countries with the highest death count.

### Query 7: Breaking Down Data by Continent
This query groups data by continent and identifies continents with the highest death count per population.

### Query 8: Global Numbers
This query provides global COVID-19 statistics, including total cases, total deaths, and death percentage.

### Query 9: Total Population vs Vaccinations
This query joins the `CovidDeaths` and `CovidVaccinations` tables and calculates the percentage of the population that received at least one COVID-19 vaccine dose.

### Query 10: Using CTE for Vaccination Calculation
This query uses a Common Table Expression (CTE) to perform calculations on the vaccination data obtained from the previous query.

### Query 11: Using Temporary Table for Vaccination Calculation
This query uses a temporary table named `PopulationPercentVaccinatedTable` to store intermediate results and performs calculations on the vaccination data.

### Query 12: Creating View for Visualization
This query creates a view named `PercentPopulationVaccinated` to store the calculated vaccination data for later visualizations.

## Note
- The data used in these queries is sourced from the `PortfolioProject` schema.
- Some queries include specific filters, such as locations containing the word 'india'. Adjust these filters based on your analysis requirements.
- Queries involving rolling calculations use Window Functions for efficient data processing.
- The use of views, temporary tables, and CTEs demonstrates different approaches to performing complex calculations and storing intermediate results.

