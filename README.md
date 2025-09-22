# Air Quality - Modeling concentration of PM2.5 across counties in California

This is an accompanying notebook for a talk given at the __[Summer School on Machine Learning for Scientific Research
](http://psi.petnica.rs/2025_ml/description.php), presented as an example use case of Bayesian Hierarchical Models in environmental sciences.

__[Particulate matter (PM)](https://www.epa.gov/pm-pollution/particulate-matter-pm-basics)__ refers to tiny particles of solid or liquid suspended in the air. Particles with a diameter of 2.5 micrometers or smaller (PM2.5) are __[particularly concerning](https://ww2.arb.ca.gov/resources/inhalable-particulate-matter-and-health)__ because they can reach deep into the lungs and even the bloodstream. Exposure to PM2.5 has been linked to stroke, cardiovascular and respiratory disease, cancer, and other serious health outcomes. 

While daily concentrations above 35 μg/m³ are considered extremely hazardous, there is no known safe level of PM2.5 exposure.

PM2.5 comes from a wide range of sources, either emitted directly from vehicles, industrial activity, or fires, or formed in the atmosphere through chemical reactions involving pollutants like sulfur dioxide or nitrogen oxides. In California, wildfires are a major source. Ash and smoke contain __[high levels of PM2.5](https://www.epa.gov/wildfire-smoke-course/why-wildfire-smoke-health-concern)__, and wildfire events have become more frequent and intense with climate change.

In this notebook, we’ll build Bayesian hierarchical models to predict average monthly PM2.5 concentrations at the county level in California. We will use publicly available data provided by the U.S. __[Environmental Protection Agency (EPA)](https://www.epa.gov/outdoor-air-quality-data/download-daily-data)__. Our goal is to account for spatial and temporal variation and eventually quantify uncertainty in these predictions.
