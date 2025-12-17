# Supply Chain Analytics in Power BI

## Overview  
Interactive Power BI case study that builds a **make‑versus‑buy decision tool** for a manufacturing company. The report evaluates internal production vs. multiple suppliers across different demand volumes.  

## Problem Statement  
The company must decide whether to **make parts in‑house or buy from external suppliers** while managing limited machine capacity and varying supplier quotes. Static spreadsheets make it hard to see cost trade‑offs across parts, suppliers, and volumes.    

## Objective  
- Combine supplier quotes and internal manufacturing cost data in a single Power BI model.  
- Compare **full costs** (unit + non‑recurring + capital) for make vs. buy by part and scenario volume.  
- Support quick, data‑driven sourcing and capital‑investment decisions with interactive visuals.  

## Dataset  
- **Supplier quotes**: supplier, part number, volume, unit cost, non‑recurring expenses (tooling/NRE).  
- **Internal manufacturing**: machine model, existing and required capacity, capital investment, make full cost.  
- **Scenario parameters**: volume slider and mapping tables for “what‑if” analysis.  

<p  align="center"><img width="80%" src="https://github.com/SatyamSingh1299/SupplyChain_PowerBi/blob/main/imgs/img1.png" /></a></p>  

<p  align="center"><img width="80%" src="https://github.com/SatyamSingh1299/SupplyChain_PowerBi/blob/main/imgs/img2.png" /></a></p>  

<p  align="center"><img width="80%" src="https://github.com/SatyamSingh1299/SupplyChain_PowerBi/blob/main/imgs/img3.png" /></a></p> 

## Data Analysis  
- Modeled **buy full cost** = unit cost × volume + non‑recurring expenses for each supplier–part–volume combination.  
- Modeled **make full cost** using capacity requirements, capital investment, and per‑unit production cost for each part.  
- Built interactive report pages:  
  - **Supplier Selection** – lowest‑cost supplier by part and volume with bar/line charts.  
  - **Scenario Analysis / Planner** – cost curves by supplier vs. scenario volume plus total NRE.  
  - **Make versus Buy** – side‑by‑side make vs. buy costs, cost avoidance, and final decision by part.  

## Insights  
- Optimal supplier **changes with volume**; lower‑NRE suppliers can become cheaper at higher volumes despite higher unit prices.  
- Some parts clearly favor **buying** (large cost avoidance vs. make), while others favor **in‑house production** once capital is justified.  
- Total buy cost and NRE increase in steps as volume grows, revealing **volume thresholds** where supplier switches or make decisions become attractive.  

## Recommendations  
- Define **volume‑based rules per part** (e.g., buy at low volume, consider make at high volume) using the make‑vs‑buy summary.  
- Prefer suppliers whose **cost curves scale well with volume** and have moderate NRE, not just the lowest starting unit cost.  
- Align **capital investments** with parts where make costs are consistently below best supplier quotes across realistic demand ranges.  
