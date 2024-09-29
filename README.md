#Project Summary

The goal of this project is to create district geometry from point data.
There are many district types in the state of New York,
such as Town, City, County, Ward, County Legislature, Village, Municipal Court, City Council,
Congressional, Senate, Assembly, and Election districts.
For now, I will focus on the latter four.

Our main data source is [GIS](https://gis.ny.gov/streets-addresses), who have geometry data for addresses and streets across the state.
Through my work, I also have access to the state-wide voter file.
Every line in that file is a registered voter, with their corresponding address and districts.
Election districts are the “basic political subdivision for purposes of registration and voting” in New York State.
By law, the boundaries of election districts must be the boundaries of other districts, streets, or rivers.
So, we will also be using geometry data for the shapes of Congressional, Senate, and Assembly districts, found [here](https://latfor.state.ny.us).
Given these data sources, it should be possible to construct the shapes of election districts.
