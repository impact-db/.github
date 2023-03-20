## Welcome to ImpactDB

The Industrial Microbiology Publication and AI Crowd-sourced Toolbox (ImpactDB) is a platform for facilitating collaboration among synthetic biology researchers. Metabolic engineering knowledge is distributed in thousands of publications, so accessing relevant information is time-consuming. This database exists to centralize the currently distributed efforts of researchers who extract data from academic papers. The data is organized into fermentation result instances, which pair the bioprocess results (titer/rate/yield) of a strain with its bioprocess environment (e.g., temperature or pH) and its genetic background at a strain and gene level.

ImpactDB also contains web interfaces for open-sourced machine learning models for titer prediction and strain design. These user-friendly interfaces provide access to modern computational biology tools.

## Repositories

### [impact-db-client](https://github.com/impact-db/impact-db-client)
The front end of ImpactDB.
The website is a React app made using Vite. The styles are done using ChakraUI. It gets data from a Firebase backend, and client side state is managed using React Query.

### [impact-db-functions-js](https://github.com/impact-db/impact-db-functions-js)
Helper functions for interacting with the Firebase database. This repository contains code that allows read access to the Firebase database from an HTTP endpoint, and contains a scheduled functions that updates the number of papers and strains in the database to allow for the plot on the homepage.

### [impact-db-functions-python](https://github.com/impact-db/impact-db-functions-python)
Helper functions to allow for machine learning algorithms to available to the front end. Right now only the predict titers function in present in this repository
