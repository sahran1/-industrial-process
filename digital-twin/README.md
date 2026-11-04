# FactoryTwin — Bottling Line Digital Twin

This folder contains an educational, browser-based digital twin of a PET beverage packaging line. The simulation represents a virtual production process, calculates performance indicators, estimates equipment risk, and compares lifecycle choices for packaging.

## What the prototype includes

- Five connected production stages: depalletizer, bottle filler, capper, labeler, and case packer.
- Simulated throughput, WIP, good output, rejects, energy use, and equipment condition.
- OEE, calculated as availability × performance × quality.
- Fault injection for equipment and supplier scenarios.
- Predictive maintenance estimates based on condition trend, fault rules, and buffer pressure.
- Product lifecycle comparisons for virgin PET, a 50% recycled PET blend, and lightweight PET, including illustrative cost, carbon, and recovery assumptions.
- Contextual action recommendations and an event log.

## Run

Open `index.html` in a modern web browser. The app has no external dependencies or build step.

## Model and limitations

The simulation advances one virtual minute per real second. All initial values, station capacities, material costs, emissions factors, recovery rates, and fault effects are synthetic coursework assumptions. OEE uses availability, performance, and quality factors. Predictive maintenance uses an explainable rules-and-trend indicator; it is not trained or validated machine learning. The app is not connected to PLC, MES, ERP, suppliers, or physical factory equipment. Lifecycle estimates are directional only and require validated supplier and lifecycle assessment data before operational use.