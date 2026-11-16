# Varun Nair

Software engineer focused on machine learning, simulation, and perception/sensing systems. I build end-to-end systems, from data collection and modeling through APIs and tested, deployed applications.

**Contact:** [varunnair120@gmail.com](mailto:varunnair120@gmail.com)

---

## Focus Areas

| Area | What I work on |
| --- | --- |
| Machine Learning & AI | Neural surrogate models, uncertainty quantification, LLM evaluation, classical computer vision |
| Software Engineering | Backend APIs, data pipelines, automated testing, CI/CD, cloud deployment |
| Robotics & Sensing | Multi-sensor data acquisition, real-time object tracking, simulation of physical systems |

---

## Selected Projects

### Panacea: Neural-Surrogate Epidemic Scenario Explorer
[Repository](https://github.com/Viharitejomurtula/Panacea) | [Live demo](https://panacea-40a16.web.app) | Team project, built in 24 hours at HackDavis 2026 (Most Technically Challenging Project)

Interactive tool for exploring how interventions such as masking, vaccination, and contact reduction change an outbreak over 365 days.

- Trained a PyTorch surrogate on 5,000 Latin Hypercube-sampled runs of a 30,000-agent Mesa ABM, reaching an MAE of 0.043 and roughly 300,000x faster inference than the simulator.
- Added Monte Carlo uncertainty bounds, Sobol sensitivity analysis (SALib), and decision-tree scenario discovery.
- Served through a FastAPI backend with automated backend and frontend test suites and CI.

**Stack:** Python, PyTorch, Mesa, SALib, FastAPI, pytest, GitHub Actions

### GR1D: Grid Ride-Through Compliance Testing for Data Centers
[Repository](https://github.com/Viharitejomurtula/GR1D) | Team project

Pipeline that turns a data center design into a compliance verdict against ERCOT NOGRR 282 by stress-testing it with thousands of simulated grid disturbances.

- Physics simulator in Modelica covering grid, transformers, PSU fleet, battery backup, cooling, and protection relays, graded against four requirements from the primary rule text.
- Scenario generator built on a Bayesian network so correlated conditions (temperature, load, equipment age) are sampled jointly.
- Neural surrogate trained on 9,771 simulator runs (92.0% pass/fail accuracy, AUC 0.955) to screen the scenario space, with Shapley attribution to rank failure drivers.

**Stack:** Python, Modelica, PyTorch, FastAPI, Docker, ngspice and PyBaMM cross-checks

### Harbor: Operating System for Local Businesses
[Repository](https://github.com/varunnair1234/HarborProject_CruzHacks26) | CruzHacks 2026

Full-stack platform that gives Santa Cruz small businesses early warning on cash flow, tourism demand, and rent changes.

- Four modules: cash-runway projection, 7-day tourism forecast, rent-increase tracking, and a local business directory.
- Trained a custom model on scraped Santa Cruz rent data and integrated open LLMs (DeepSeek, Gemini).
- FastAPI backend with JWT authentication, Supabase database, deployed on Render.

**Stack:** Python, FastAPI, Supabase, JWT, regression and classification models

### Epigenetic Clock Reasoning Bench
[Repository](https://github.com/varunnair1234/Epigenetic-Clock-Reasoning-Bench)

Benchmark and evaluation harness for testing how well AI models reason about epigenetic aging clocks, built on the GSE40279 methylation dataset.

- Scenario generator, model clients, and scorer with per-label metrics and baseline analysis.
- Tissue aging simulation core with tests, plus a FastAPI visualization backend deployed on Render.
- Technical documentation and pitch deck included in the repository.

**Stack:** Python, FastAPI, pytest

### ATMOS Lab Framework: Multi-Sensor Atmospheric Data Capture
[Repository](https://github.com/varunnair1234/ATMOS-Lab-framework)

Framework for capturing, logging, and analyzing weather data from an iMet-X4 radiosonde/UAS payload, a METER ATMOS 22 anemometer, and a Trisonica Mini 3D anemometer.

- Independent serial and SDI-12 readers with automatic reconnect, fused into one canonical data stream.
- Live Dash dashboard and post-flight reports (time series, wind rose, vertical profile, correlation analysis).
- Parser tests validated against real hardware output; CI runs tests and publishes a dashboard to GitHub Pages.

**Stack:** Python, Dash, matplotlib, pandas, pyserial, pytest, GitHub Actions

### Object Tracker: Real-Time Visual Tracking with Incremental PCA
[Repository](https://github.com/varunnair1234/object_tracker)

Classical visual tracker, with no neural network or training data, that learns an object's appearance subspace online and locates it by reconstruction error.

- Rolling buffer of winning patches feeds an SVD-based PCA appearance model that adapts to lighting and pose changes.
- Candidate search, scoring, and update loop running on a live webcam feed, based on Ross et al. (2008).
- Documents design decisions, failure modes (drift, occlusion, scale), and planned improvements.

**Stack:** Python, OpenCV, PyTorch, NumPy

---

## Technical Skills

**Languages:** Python, Modelica, SQL

**Machine Learning:** PyTorch, NumPy, pandas, OpenCV, surrogate modeling, uncertainty quantification, sensitivity analysis, Bayesian networks

**Backend & Data:** FastAPI, REST APIs, JWT authentication, Supabase, serial and SDI-12 sensor interfaces

**Tools & Practices:** Git, GitHub Actions, Docker, pytest, Plotly Dash, deployment on Render, Railway, and Firebase

---

## Connect

I'm looking for software engineering, ML/AI, and robotics roles. The best way to reach me is by email at [varunnair120@gmail.com](mailto:varunnair120@gmail.com).
