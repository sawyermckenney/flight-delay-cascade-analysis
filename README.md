# Flight Delay Analysis                                                                                                                 
                                                                                                                                    
## Overview
I plan to explore delay 
propagations in airline networks. Commercial airlines run on a very tight schedule trying their best 
to promise consumers on time departures and arrivals. With crews, aircraft rotations, and 
weather there are many factors that can affect a single flight that as a result cascade 
downstream and can affect travel for the rest of the day or in some cases the rest of the week all 
around the US. I plan to model domestic airlines in the United States as a directed graph and 
apply various methods from CSCI 4022 to identify what airports and routes are the most 
influential to delays, how delays propagate, and what combinations of conditions are reliable to 
predict large scale cascades.
                                                                                                                                        
## Data                                                                                                                                 
- Source: BTS On-Time Performance data                                                                                                  
- File: `bts_combined.parquet`
                                                                                                                                        
## Files
- `analysis.ipynb` — main analysis notebook                                                                                             
                                                                                                                                        
## Methods
- Data cleaning                                                                                                                         
- Route-level aggregation
- PageRank on flight network
- Apriori on cascade days                                                                                                               

## Key Findings                                                                                                                         
- Delays concentrate at a few key hubs (DFW, ORD, DEN)
- Some airports amplify delays beyond traffic, others absorb them (ATL, LAX)
- Late aircraft delay is the main driver of propagation
- Weather is the key trigger for cascade days
                                                                                                                                        
## How to Run   
1. Install dependencies
2. Open `analysis.ipynb`
3. Run all cells                                                                                                                        

## Requirements                                                                                                                         
- pandas        
- numpy
- matplotlib
- networkx
- mlxtend